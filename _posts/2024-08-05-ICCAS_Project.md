---
layout: single
title: "ICCAS 2024 Project"
categories: Project
tag: [AI, unity]
date: 2024-08-05
---

# 📌 프로젝트명  
**Medical Posture Correction Game for Disc Prevention and Patients (P.O.S.E)**

---

## 1. 프로젝트 개요

**P.O.S.E**는 현대인에게 흔히 발생하는 허리 디스크(추간판 탈출증)를 예방하고, 재활을 도울 수 있는 **AI 기반 자세교정 게임**입니다. 물리치료 운동인 **McKenzie 운동법**을 게임으로 구현하여, 사용자에게 재미와 건강을 동시에 제공하는 것을 목표로 합니다.

---

## 2. 주제 선정 이유

현대인의 잘못된 자세 습관과 스마트폰·컴퓨터 사용 증가로 인해 요통 및 목 통증을 호소하는 인구가 증가하고 있습니다.  
<p align="center">
<img src="/images/ICCAS2024/slide4.PNG" alt="Statistics" style="zoom: 25%;" /><br>
</p>
- 2020년 디스크 환자 수: **272만 명**  
- 2021년 디스크 환자 수: **279만 명**  
(출처 : Korea Health Insurance Review & Assessment Service)

특히 젊은 세대에서도 디스크 유병률이 증가하는 만큼, **재미있는 방식으로 예방과 재활을 동시에** 실현할 수 있는 솔루션이 필요하다고 판단하였습니다.

---

## 3. 시스템 설명

### 핵심 기능  
<img src="/images/ICCAS2024/slide10.PNG" alt="function" style="zoom: 25%;" /><br>
- **AI 자세 분석**: ResNet-50 기반 모델을 활용하여 신체 주요 관절 위치와 각도를 분석
- **실시간 피드백**: 사용자 자세의 정확도를 실시간 점수화 및 시각화
- **게임 기반 운동 루틴**: 스테이지와 챕터로 구성된 다양한 McKenzie 운동 수행
- **보상 시스템**: 정확도에 따라 캐릭터 성장, 스킨 구매 등 보상 제공

### 개발 환경  
<img src="/images/ICCAS2024/slide8.PNG" alt="Dev.Env." style="zoom: 25%;" /><br>
- AI 모델: ResNet-50
- 게임 엔진: Unity
- DB: 사용자 정보, 자세 분석 데이터, 게임 내 진척도 저장

---

## 5. 인게임 화면

<img src="/images/ICCAS2024/slide13.PNG" alt="screen1" style="zoom: 25%;" /><br>
<img src="/images/ICCAS2024/slide14.PNG" alt="screen2" style="zoom: 25%;" /><br>
<img src="/images/ICCAS2024/slide15.PNG" alt="screen3" style="zoom: 25%;" /><br>
<img src="/images/ICCAS2024/slide16.PNG" alt="screen4" style="zoom: 25%;" /><br>
<img src="/images/ICCAS2024/slide17.PNG" alt="screen5" style="zoom: 25%;" /><br>
<img src="/images/ICCAS2024/slide18.PNG" alt="screen6" style="zoom: 25%;" /><br>
<img src="/images/ICCAS2024/slide19.PNG" alt="screen7" style="zoom: 25%;" />

---

## 4. 대상 고객

- 사무직 및 장시간 앉아 있는 직장인
- 운동 부족을 느끼는 학생 및 청년층
- 병원 방문이 어렵거나, 셀프 재활 운동을 원하는 사용자
- 자세 교정 및 디스크 예방에 관심 있는 일반인

---

## 5. 활용 방안 및 파급 효과

- **디지털 헬스케어 서비스로 확장 가능**  
- **리모트 재활 치료에 활용** (물리치료사의 가이드 없이도 셀프 진단 및 운동 가능)  
- **TV·스마트워치 등 IoT 연동 확장성**  
- **비대면 시대에 적합한 홈트레이닝 솔루션**  

---

## 6. 향후 발전 방향 (Future Works)

1. 다양한 운동 카테고리 추가 (요가, 스트레칭 등)
2. 사용자 간 커뮤니티 기능 추가
3. 전문가 피드백 기능 (정형외과, 물리치료사 연동)
4. TV 등 대형 화면 장비 연동으로 가시성 향상

---

## 7. 팀원 및 역할

| 이름         | 소속대학               | 역할                                      |
|--------------|------------------------|-------------------------------------------|
| 김경현       | 동서대학교             | AI 모델 연동, 자세 평가 알고리즘 개발     |
| 박신영       | 인제대학교             | 게임 UI 개발, 모션 인식 기능, DB 관리     |
| 유수호       | 인하대학교             | 게임 시스템 통합 및 테스트                |
| 이선주       | 충북대학교             | 데이터베이스 관리 및 인터페이스 지원      |
| **지도교수** | 김봉재 교수 (충북대학교) | 프로젝트 총괄 자문                         |

---

## 8. 요약 및 결론

**P.O.S.E**는 디스크 예방 및 재활을 위한 McKenzie 운동을 게임화하여, 사용자에게 **건강한 운동 습관과 재미**를 동시에 제공합니다.  
AI를 활용한 실시간 자세 분석과 피드백 기능은 향후 **디지털 치료제(DTx)** 또는 **홈트레이닝 서비스**로의 확장 가능성도 가지고 있습니다.

> *건강은 지키는 것보다 무너지지 않게 예방하는 것이 더 중요합니다.*  
> ***P.O.S.E**는 그 시작을 게임으로 만들어 갑니다.*

---


- *[프로젝트 코드](https://github.com/zachpaul7/ICCAS_4)*  
- *[발표자료](https://drive.google.com/file/d/1mciSA6k7jMiwEmd2MdGlWDDxnLXxcEWT/view?usp=sharing)*  
- *[EKC2024 포스터 세션](https://drive.google.com/file/d/14yUuSrNu6T3y3odnOtQFwmmDYyRWfyH4/view?usp=sharing)*