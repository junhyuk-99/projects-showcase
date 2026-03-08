# 김준혁
### Web 기반 제조 시스템 개발자

제조 현장의 설비·운영 데이터를 Web 시스템으로 연결하는 일을 하고 있습니다.
Spring Boot + React 기반의 생산관리 시스템, 설비 모니터링, 대시보드 개발이 주 업무입니다.

**Java · Spring Boot · React · SQL Server · MongoDB**

---

## Overview

본 저장소는 실무에서 진행한 프로젝트들을 정리한 포트폴리오입니다.
보안 및 회사 정책상 소스 코드는 포함하지 않으며, **시스템 구조와 설계, 문제 해결 과정** 위주로 작성했습니다.

---

## Projects

| 프로젝트 | 설명 | 링크 |
|---------|------|------|
| **NWM** – Billet Tracking / Count Matching | 설비 카운트 기반 생산 실적 자동 집계 및 LOT Tracking | [/nwm](./nwm) |
| **MGO** – Equipment Operation Monitoring | SCADA 설비 데이터 기반 실시간 설비 가동 모니터링 | [/mgo](./mgo) |
| **Dashboard** – Equipment & Operation Overview | MongoDB 기반 설비·운영 데이터 통합 대시보드 (단독 개발) | [/dashboard](./dashboard) |

---

## Architecture

```
PLC / SCADA
    ↓
Database (SQL Server, MongoDB)
    ↓
Spring Boot API Server
    ↓
React Web Client
```

---

## Tech Stack

| 구분 | 기술 |
|------|------|
| Backend | Java, Spring Boot |
| Frontend | React |
| Database | SQL Server, MongoDB |
| Domain | 설비 모니터링, 생산관리(MES) |
