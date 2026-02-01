# 김준혁
### Web-based System & Equipment Monitoring Developer

제조 현장 데이터를 Web 기반으로 연결하고,  
설비·운영 데이터를 **운영에 바로 쓰일 수 있는 시스템 로직**으로 정리하는 개발자입니다.

Java(Spring Boot)와 React 기반 Web 시스템 프로젝트를 중심으로  
설비 데이터 처리, 생산 실적 정합, 모니터링 대시보드 구축 경험을 쌓아왔습니다.

**Java · Spring Boot · React · SQL Server · MongoDB**

---

## Projects

- **NWM – Billet Tracking / Count Matching**  
  설비 카운트 기반 생산 실적 자동 집계 및 LOT Tracking 정합  
  👉 [/nwm](./nwm)

- **MGO – Equipment Operation Monitoring (MON)**  
  SCADA 설비 데이터를 Web에서 실시간으로 확인하는 설비 가동 모니터링  
  👉 [/mgo](./mgo)

- **In-house Dashboard (Ongoing)**  
  MongoDB 기반 설비·운영 데이터 대시보드 단독 설계·개발  
  👉 [/dashboard](./dashboard)

---

## Overview

본 저장소는 제조 현장 데이터를 Web 기반으로 연결하고 운영하기 위한  
시스템 및 설비 모니터링 프로젝트들을 정리한 포트폴리오입니다.

실무 프로젝트를 기반으로 하되,  
보안 및 회사 정책을 고려하여 **소스 코드보다는 구조·설계·문제 해결 과정**을 중심으로 정리했습니다.

---

## Summary

- **NWM Project**  
  설비 카운트와 생산 실적 간 불일치 문제를 해결하기 위해  
  자동 집계 및 시간 스트림 기반 매칭 구조를 설계

- **MGO Project**  
  SCADA 설비 데이터를 Web으로 연동해  
  설비 가동 상태를 실시간으로 확인할 수 있는 모니터링 화면 구축

- **In-house Dashboard**  
  기존 MSSQL 중심 구조에서 벗어나 MongoDB를 새롭게 도입하고,  
  Java 서버와 연동한 API 기반 대시보드를 단독으로 설계·개발

---

## Architecture

PLC / SCADA  
→ Database (SQL Server, MongoDB)  
→ Spring Boot API  
→ React Web Client

---

## Additional Notes

단독 대시보드 프로젝트를 진행하며  
서버·데이터 구조뿐 아니라 화면 구성과 사용자 흐름까지 직접 고민하게 되었고,  
프론트엔드 구현 역시 운영자의 판단과 사용 맥락을 반영하는 중요한 영역이라는 점을 체감했습니다.

이를 통해 시스템 전체 흐름을 고려한 UI 구성과 개선 경험을 함께 쌓을 수 있었습니다.

---

## Tech Stack

- **Backend**: Java, Spring Boot  
- **Frontend**: React  
- **Database**: SQL Server, MongoDB  
- **Domain**: Equipment Monitoring, Manufacturing Systems

---

## Notes

본 저장소는 **포트폴리오 목적의 공개 자료**입니다.  
실제 서비스에 사용된 소스 코드는 보안 및 회사 정책에 따라 공개하지 않으며,  
대신 **시스템 구조, 설계 의도, 문제 해결 방식**을 중심으로 정리했습니다.
