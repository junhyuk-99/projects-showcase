# 김준혁
### Web MES · Equipment Monitoring Developer

제조 현장 데이터를 Web 기반으로 연결하고,  
설비·생산 데이터를 **운영에 바로 쓰일 수 있는 시스템 로직**으로 만드는 개발자입니다.

Java(Spring Boot)와 React 기반 Web MES 프로젝트를 중심으로  
설비 데이터 처리, 생산 실적 정합, 모니터링 대시보드 구축 경험을 쌓아왔습니다.

**Java · Spring Boot · React · SQL Server · MongoDB**

---

## Projects

- **NWM – Billet Tracking / Count Matching**  
  설비 카운트 기반 생산 실적 자동 집계 및 LOT Tracking 정합  
  👉 [/nwm](./nwm)

- **MGO – Equipment Operation Monitoring (MON)**  
  SCADA 설비 데이터를 Web에서 실시간으로 모니터링하는 설비 가동 화면  
  👉 [/mgo](./mgo)

- **In-house Dashboard (Ongoing)**  
  MongoDB 기반 설비·운영 데이터 대시보드 단독 설계·개발  
  👉 [/dashboard](./dashboard)

---

## Overview

본 저장소는 제조 현장 데이터를 Web 기반으로 연결하고 운영하기 위한  
MES 및 설비 모니터링 프로젝트들을 정리한 포트폴리오입니다.

실무 프로젝트를 기반으로 하되,  
보안 및 회사 정책을 고려하여 **소스 코드보다는 구조·설계·문제 해결 과정**을 중심으로 정리했습니다.

---

## Summary

- **NWM(능원금속)**  
  설비 카운트와 생산 실적 간 불일치 문제를 해결하기 위한  
  자동 집계 및 시간 스트림 기반 매칭 구조 설계

- **MGO(엠지오)**  
  SCADA 설비 데이터를 Web으로 연동해  
  설비 가동 상태를 실시간으로 확인할 수 있는 모니터링 화면 구축

- **In-house Dashboard**  
  기존 MSSQL 중심 구조 대신 MongoDB를 새롭게 도입해  
  설비 데이터를 수집하고 Java 서버와 연동한 대시보드 구조 설계 및 개발

---

## Architecture

PLC / SCADA  
→ Database (SQL Server, MongoDB)  
→ Spring Boot API  
→ React Web Client

- 업무일자(06:30), LOT, 설비 카운트 등 **현장 기준을 시스템 로직으로 구조화**
- 설비 데이터와 MES 실적 간 **정합성을 확보하기 위한 집계·매칭 구조 설계**

---

## Tech Stack

- **Backend**: Java, Spring Boot  
- **Frontend**: React  
- **Database**: SQL Server, MongoDB  
- **Domain**: MES, PLC / SCADA, Equipment Monitoring

---

## Notes

본 저장소는 **포트폴리오 목적의 공개 자료**입니다.  
실제 서비스에 사용된 소스 코드는 보안 및 회사 정책에 따라 공개하지 않으며,  
대신 **시스템 구조, 설계 의도, 문제 해결 방식**을 중심으로 정리했습니다.
