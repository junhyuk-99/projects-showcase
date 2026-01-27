# Web MES Projects Showcase (NWM / MGO)

제조 현장 데이터를 **Web 기반으로 연결하고 운영**하기 위한  
MES 및 설비 모니터링 프로젝트들을 정리한 저장소입니다.

본 저장소는 **실무 프로젝트를 기반**으로 하되,  
보안 및 회사 정책을 고려하여 **구조·설계·문제 해결 방식 중심**으로 재구성했습니다.

---

## TL;DR

- **NWM(능원금속)**  
  설비 카운트 기반 생산 실적 자동 집계 및 LOT Tracking 정합 구조 설계
- **MGO(엠지오)**  
  SCADA 설비 데이터를 Web에서 실시간으로 모니터링하는 MON 구축

---

## Architecture (Common)

PLC / SCADA
↓
DB (SQL Server)
↓
Spring Boot API
↓
React Client



- 현장 기준(업무일자 06:30, LOT, 설비 카운트)을 시스템 로직으로 구조화
- 설비 데이터와 MES 실적 간 정합성을 확보하기 위한 집계·매칭 로직 설계

---

## What this repository focuses on

- 시스템 구조(다이어그램) 및 핵심 설계 의도
- 현장 기준을 시스템 로직으로 녹여낸 설계 방식
- 민감정보를 제거한 SQL 구조 및 집계 로직 예시
- 운영 관점에서의 UI·데이터 흐름 개선 포인트

> ⚠️ 실제 서비스에 사용된 전체 소스 코드는 포함하지 않습니다.

---

## Projects

### 1) NWM – Billet Tracking / Count Matching

**Context**
- 설비 카운트와 MES 생산 실적 간 불일치
- LOT 입력 지연·누락으로 인한 데이터 신뢰도 저하

**Solution**
- 설비 카운트 기반 자동 집계 로직 설계
- 시간 스트림(RN) 기준 매칭 구조로 데이터 정합성 확보

**Result (Example)**
- 수기 입력 및 검증 업무를 설비 데이터 기반 자동 집계로 전환
- 설비 데이터와 MES 실적 간 불일치 빈도 감소

📁 Details: [`/nwm`](./nwm)

---

### 2) MGO – Equipment Monitoring (MON)

**Context**
- 설비 상태 파악 및 공유가 현장·구두 중심으로 이루어짐
- 관리자/운영자 간 실시간 정보 공유 한계

**Solution**
- SCADA 연동 데이터를 기반으로 Web 실시간 모니터링 화면 구성
- 설비 상태 및 주요 지표를 한 화면에서 확인 가능한 구조 설계

**Result (Example)**
- 설비 상태 확인 및 이상 판단 흐름을 Web 기반으로 전환
- 설비 정보 공유 및 대응 속도 개선

📁 Details: [`/mgo`](./mgo)

---

## Tech Stack

- **Backend**: Java, Spring Boot  
- **Frontend**: React  
- **Database**: SQL Server  
- **Domain**: MES, PLC, SCADA

---

## Notes

본 저장소는 **포트폴리오 목적의 공개 자료**입니다.  
실제 서비스에 사용된 소스 코드는 보안 및 회사 정책에 따라 공개하지 않으며,  
대신 **시스템 구조, 설계 의도, 문제 해결 방식**을 중심으로 정리했습니다.
