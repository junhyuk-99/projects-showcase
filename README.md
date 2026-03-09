# 김준혁
### Web Application Developer

Spring Boot + React 기반 Web 시스템을 설계하고 개발하고 있습니다.
현재는 실시간 데이터 모니터링, 대시보드, 데이터 정합 시스템 등을 주로 다루고 있으며
백엔드 API 설계부터 프론트엔드 UI 구현까지 전반적으로 참여하고 있습니다.

**Java · Spring Boot · React · SQL Server · MongoDB**

---

## Overview

본 저장소는 실무에서 진행한 프로젝트들을 정리한 포트폴리오입니다.
보안 및 회사 정책상 소스 코드는 포함하지 않으며, **시스템 구조와 설계, 문제 해결 과정** 위주로 작성했습니다.

---

## Projects

| 프로젝트 | 설명 | 링크 |
|---------|------|------|
| **NWM** – Data Tracking / Count Matching | 실시간 데이터 기반 자동 집계 및 이력 Tracking 정합 시스템 | [/nwm](./nwm) |
| **MGO** – Operation Monitoring | 실시간 상태 모니터링 Web 시스템 | [/mgo](./mgo) |
| **WNEK** – CNC/MCT Analytics Server | MongoDB 기반 데이터 수집·분석 대시보드 (단독 개발, 저작권 등록) | [/dashboard](./dashboard) |

---

## Architecture

```
Data Source (PLC / SCADA)
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
| Domain | 실시간 모니터링, 데이터 대시보드 |
