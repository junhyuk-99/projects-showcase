# 김준혁 | 제조 현장 기반 Web MES 개발자

C# 기반 현장 시스템 경험을 바탕으로 Java(Spring Boot)·React 기반 Web MES로 확장해 온 개발자입니다.  
설비(PLC/SCADA) 데이터 처리와 생산 실적 정합, 모니터링 대시보드 구축에 집중해 왔습니다.

- Tech: Java · Spring Boot · React · SQL Server · MongoDB
- Domain: MES · PLC/SCADA · Equipment Monitoring
- GitHub: 본 저장소는 보안상 코드 대신 **구조·설계·문제 해결 방식** 중심으로 정리했습니다.

## Quick Links
- NWM – Billet Tracking / Count Matching: [`/nwm`](./nwm)
- MGO – Equipment Operation Monitoring (MON): [`/mgo`](./mgo)
- In-house Dashboard (Ongoing): [`/dashboard`](./dashboard)

---

## Web MES Projects Showcase (NWM / MGO)

제조 현장 데이터를 **Web 기반으로 연결하고 운영**하기 위한  
MES 및 설비 모니터링 프로젝트들을 정리한 저장소입니다.

실무 프로젝트를 기반으로 하되,  
보안 및 회사 정책을 고려하여 **시스템 구조와 설계 관점** 중심으로 구성했습니다.

---

## Summary

- **NWM(능원금속)**  
  설비 카운트 기반 생산 실적 자동 집계 및 LOT Tracking 정합
- **MGO(엠지오)**  
  SCADA 설비 데이터를 Web에서 실시간으로 모니터링하는 설비 가동 MON
- **In-house Dashboard (Ongoing)**  
  MongoDB 기반 설비·운영 데이터 통합 대시보드 설계 및 개발 중

---

## Architecture

PLC / SCADA → DB (SQL Server) → Spring Boot API → React Client



- 업무일자(06:30), LOT, 설비 카운트 등 **현장 기준을 시스템 로직으로 구조화**
- 설비 데이터와 MES 실적 간 **정합성을 확보하기 위한 집계·매칭 구조 설계**

---

## Projects

### NWM – Billet Tracking / Count Matching

- 설비 카운트와 생산 실적 간 불일치 문제 해결
- LOT 입력 지연·누락 상황에서도 이력 공백이 발생하지 않도록 설계
- 설비 카운트 기반 자동 집계 및 시간 스트림(RN) 매칭 구조 적용

📁 Details: [/nwm](./nwm)

---

### MGO – Equipment Operation Monitoring (MON)

- SCADA 설비 데이터를 기반으로 한 **설비 가동 상태 모니터링**
- 설비 상태 및 주요 지표를 Web에서 실시간으로 확인 가능한 구조 설계
- 현장·관리자 간 설비 정보 공유 및 대응 흐름 개선

📁 Details: [/mgo](./mgo)

---

### In-house Dashboard – Equipment & Operation Overview (Ongoing)

- 설비·운영 데이터 분산으로 인한 현황 파악 어려움 개선 목적
- MongoDB 기반 데이터 모델을 적용한 대시보드 구조 설계
- 설비 상태 및 주요 운영 지표를 통합 조회할 수 있는 Web 대시보드 개발 중

📁 Details: [/dashboard](./dashboard)

---

## Tech Stack

- **Backend**: Java, Spring Boot  
- **Frontend**: React  
- **Database**: SQL Server, MongoDB  
- **Domain**: MES, PLC, SCADA

---

## Notes

본 저장소는 **포트폴리오 목적의 공개 자료**입니다.  
실제 서비스에 사용된 소스 코드는 보안 및 회사 정책에 따라 공개하지 않으며,  
대신 **시스템 구조, 설계 의도, 문제 해결 방식**을 중심으로 정리했습니다.
