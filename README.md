# Web MES Projects Showcase (NWM / MGO)

제조 현장 데이터를 Web 기반으로 연결하고 운영하기 위한 프로젝트들을 정리한 저장소입니다.  
(실무 프로젝트 기반이며, 보안상 **구조/설계/샘플 코드 중심**으로 재구성했습니다.)

## TL;DR (한 줄 요약)
- **NWM(능원금속)**: 설비 카운트 기반 생산 실적 자동 집계 및 LOT Tracking 정합
- **MGO(엠지오)**: SCADA 설비 데이터를 Web에서 실시간 모니터링하는 MON 구축

## Architecture (공통)
PLC/SCADA → DB(SQL Server) → Spring Boot API → React Client

- 현장 기준(업무일자 06:30, LOT, 설비 카운트)을 시스템 로직으로 구조화
- 설비 데이터와 MES 실적의 정합성을 확보하는 집계/매칭 로직 설계

## Projects
### 1) NWM - Billet Tracking / Count Matching
- 핵심 문제: 설비 카운트와 생산 실적 간 불일치, LOT 입력 지연/누락
- 해결: 카운트 기반 집계 로직 및 시간 스트림 매칭 설계
- 성과(예시): 수기 입력/검증 업무량 감소, 데이터 신뢰도 향상  
📁 상세: [/nwm](./nwm)

### 2) MGO - Equipment Monitoring (MON)
- 핵심 문제: 설비 상태 파악/공유의 지연
- 해결: SCADA 연동 데이터 기반 실시간 모니터링 화면 구성
- 성과(예시): 설비 상태 확인/판단 시간 단축  
📁 상세: [/mgo](./mgo)

## What you can see here
- 시스템 구조(다이어그램) 및 핵심 설계 의도
- 민감정보 제거 후 재구성한 SQL 샘플
- 화면 구성 및 운영 관점의 개선 포인트

## Tech Stack
- Backend: Java, Spring Boot
- Frontend: React
- DB: SQL Server
- Domain: MES, PLC, SCADA

## Notes
본 저장소는 포트폴리오 목적의 공개 자료로, 회사 자산/민감정보는 포함하지 않습니다.
