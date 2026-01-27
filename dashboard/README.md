# In-house Dashboard – Equipment & Operation Overview (Ongoing)

설비 및 운영 데이터를 Web 기반으로 한눈에 확인할 수 있도록  
구성 중인 내부 대시보드 프로젝트입니다.

기존 MES 데이터와는 목적을 분리하여,  
실시간성 및 지표 확장성이 필요한 영역을 중심으로 설계하고 있습니다.

---

## Background

- 설비 및 운영 데이터가 여러 시스템에 분산되어 있음
- 현황 파악을 위해 데이터 취합 및 확인 과정이 반복됨
- 즉각적인 상태 확인을 위한 별도의 대시보드 필요

---

## Objective

- 설비 상태를 빠르게 파악할 수 있는 화면 구성
- 주요 운영 지표를 단일 화면에서 확인
- 실시간 지표와 누적 지표를 함께 표현할 수 있는 구조 설계

---

## Architecture (Draft)

Equipment Data → MongoDB → Java Backend (Aggregation / API) → Web Dashboard


- 설비 이벤트 및 상태 데이터를 MongoDB 컬렉션으로 관리
- Java 백엔드에서 집계·가공 후 API 제공
- 화면에서는 상태 및 지표 중심으로 시각화

---

## Current Work

- MongoDB 컬렉션 구조 및 데이터 모델 설계
- 설비 상태 판단 기준 정리
- 실시간 / 누적 지표 집계 방식 검토
- 대시보드 확장을 고려한 데이터 구조 정리

---

## Considerations

- 지표 추가 시 기존 구조에 미치는 영향 최소화
- 운영자 관점에서 빠른 상황 인지가 가능한 화면 구성
- 데이터 적재 및 집계 성능 고려

---

## Tech Stack

- Backend: Java
- Database: MongoDB
- Frontend: Web Dashboard
- Domain: Equipment Monitoring

---

## Status

- In Progress  
- 설계 및 구조 검토 단계이며, 기능은 순차적으로 확장 중입니다.
