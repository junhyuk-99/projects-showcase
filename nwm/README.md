# NWM - Billet Tracking / Count Matching

## Context
- PLC/SCADA 기반 설비 카운트를 MES 생산 실적과 정합시키는 문제를 해결했습니다.
- LOT 입력 지연/누락 상황에서도 이력 공백이 발생하지 않도록 설계했습니다.

## My Role
- 집계/매칭 로직 설계 (업무일자 06:30 기준 포함)
- SQL Server Stored Procedure 설계 및 안정화
- Web MES 연동을 위한 데이터 조회 구조 정리

## Key Design
- 시간 스트림 기반 매칭(RN)로 설비 이벤트와 슬롯을 정렬
- 중복/노이즈 제거 후 유효 데이터만 반영
- 외부 시스템 지연을 고려한 보완 경로 설계

## Files
- 아키텍처: ./architecture/
- SQL 샘플: ./sql-sample/
- 화면/로그 스샷: ./screenshots/
