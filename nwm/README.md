# NWM – Billet Tracking / Count Matching
(Long / Short Billet)

## Context
PLC/SCADA에서 수집되는 **설비 카운트 데이터**를 기준으로  
MES 생산 실적과 **LOT 단위로 정확히 정합**시키는 문제가 있었습니다.

특히,
- **Long Billet(주조)**: 설비 연속 투입으로 카운트는 발생하지만 LOT 확정이 늦어짐
- **Short Billet(절단)**: 개별 이벤트는 명확하나, 카운트·순번 불일치 발생

이로 인해 **LOT 입력 지연·누락 상황에서 생산 이력 공백**이 발생할 수 있었고,  
이를 구조적으로 해결할 필요가 있었습니다.

---

## My Role
- 설비 카운트 기반 **생산 실적 자동 집계 구조 설계**
- **업무일자 06:30 기준**을 포함한 집계·정합 로직 정의
- SQL Server Stored Procedure 설계 및 운영 안정화
- Web MES 연동을 위한 **LOT/카운트 조회 구조 정리**

---

## Key Design

### 1. 시간 스트림 기반 매칭 구조
- 설비 이벤트를 **시간 순서(RN)** 기준으로 정렬
- 카운트 슬롯과 이벤트를 순차적으로 매칭하여 **순번 어긋남 방지**

### 2. Long / Short Billet 트레킹 분리 설계
- **Long Billet**
  - 설비 카운트 기준으로 슬롯을 선 생성
  - LOT 정보 지연 입력 시에도 이후 자동 보정 가능하도록 설계
- **Short Billet**
  - 개별 이벤트 단위 매칭
  - 중복/노이즈 이벤트 제거 후 유효 데이터만 반영

### 3. 외부 시스템 지연 대응
- SCADA → MES 연계 지연을 고려한 보완 경로 설계
- 초기 LOT 정보 오류를 사후 정합으로 수정 가능하도록 구성

---

## Result (Example)
- 설비 카운트 기반 자동 집계로 **수기 입력·검증 작업 감소**
- LOT 누락/중복으로 인한 **생산 이력 공백 문제 해소**
- 생산 실적 데이터의 **신뢰도 및 재현성 향상**

---

## Files
- Architecture: `./architecture/`
- SQL Samples: `./sql-sample/`
- Screenshots & Logs: `./screenshots/`
