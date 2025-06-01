---
layout: single
title: "2024 창의적 종합설계 경진대회"
categories: ExternelActivity
tag: [AI, RaspberryPi, Arduino]
date: 2024-09-27
typora-copy-images-to: ../images/engineer
---

2024-08 ~ 2024-11

# 프로젝트명  
**도담(Dodam): 시각장애인을 위한 점자-한글 동시 학습기기**

---

## 1. 프로젝트 개요

> **도담**은 시각장애인을 위한 **촉각 기반 점자-한글 동시 학습기기**입니다.  
> 단순한 점자 교재를 넘어, 전자식 솔레노이드 모듈을 활용해 점자와 한글을 동시에 촉각으로 제공하며, 학습자 스스로 글자를 선택하여 직관적으로 학습할 수 있도록 설계되었습니다.

---

## 2. 문제 인식 및 주제 선정 이유
<p align="center">
  <img src="/images/engineer/슬라이드14.PNG" alt="도담 시스템 구조도" width="900">
</p>
- 국내 등록 시각장애인: 약 **25만 명**
- 그중 **점자 사용 가능자 비율은 9.6%**에 불과
- 주요 문제점:
  - 점자 교과서 제작 기간 지연
  - 누락된 정보나 낙후된 인쇄 상태
  - 학습 접근성 저하

시각 정보에 의존할 수 없는 시각장애인에게 **촉각 기반 학습 장치의 필요성**이 제기되었습니다. 이에 따라 **촉각을 통해 점자와 한글을 함께 익힐 수 있는 기기 '도담'**을 개발하게 되었습니다.

---

## 3. 시스템 설명


  ![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcS51TUg2jG9KvykfoMaZet5MwRyRuraYzG4RlJmCMzJh3N_X1vil3ic88YxVyZeXztYgztPLXXlx-qkchpkGYTtmqDDATJ2FSQ_dSKROX91dpEhV-9Jhq-jaQnmOrHhtMu9MMyiSXqN81YFqb2VXdIN9k?key=Y4GgdiAtcR5dsCX8ouT4xw)


### 🎯 핵심 아이디어
- **촉각 기반 직관적 학습**: 점자 + 한글을 동시에 촉각으로 제시
- **솔레노이드 액추에이터**: 전기 신호로 특정 점을 밀어올려 점자 구현
- **사용자 선택형 학습**: 웹 UI에서 글자를 선택하면 해당 글자 출력

### 🛠 사용 기술 및 구조
<p align="center">
  <img src="/images/engineer/슬라이드12.PNG" alt="구조" width="900">
</p>
| 구성 요소 | 설명 |
|-----------|------|
| Arduino Uno | 솔레노이드 제어 |
| Solenoid (총 76개) | 점자(12개), 한글 구성(초성·중성·종성 총 64개) |
| SMPS | 12V 40A 전원 공급장치 |
| Flask Web UI | 글자 선택 및 시리얼 통신 |
| 점자 기판 | 직접 설계한 PCB 기반의 점자/한글 출력 모듈 |

---

## 4. 작동 방식

1. 웹 UI에서 학습자가 글자를 선택  
2. Flask 서버가 아두이노로 시리얼 데이터 전송  
3. 아두이노가 해당 글자에 맞는 솔레노이드를 제어하여 점자/한글 출력  
4. 학습자는 손가락으로 만져보며 점자 및 글자 학습 가능

<p align="center">
  <img src="/images/engineer/슬라이드11.PNG" alt="도담 시스템 구조도" width="900">
</p>

---

## 5. 기대 효과

### 학습 흥미 및 지속성 향상
- 점자와 실제 한글을 **직접 매칭**하면서 학습자 스스로 발견의 재미를 느낌  
- 반복 학습 및 커스터마이징 가능

### 비용 효율성과 지속 가능성
- 교재처럼 **1회성 사용이 아니라 반영구적 사용 가능**  
- 원하는 글자만 출력 가능해 **재료 낭비 없음**

### 교육 격차 해소
- 전문 교사 없이도 독립적인 학습 가능  
- 점자에 대한 심리적 장벽 제거

---

## 6. 향후 발전 방향

1. **단어 학습 기능** 추가 (여러 글자를 순차적으로 출력)
2. **음성인식 기능** 적용 (보조자 없이 말로 글자 입력 가능)
3. **무선 통신 기능** 탑재 (Bluetooth, Wi-Fi 연동으로 공간 제약 해소)
4. **모바일 앱 연동** 확장 가능성 검토

---

## 7. 팀 소개 및 역할

| 이름     | 역할                           |
|----------|--------------------------------|
| 김경현   | 하드웨어 설계, 솔레노이드 제어, 웹 통신 설계 |
| 고태희   | UI 디자인, 사용자 피드백 구조 설계 |
| 김주형   | 회로 납땜, 기기 구조물 제작       |
| 김혜인   | 사용자 시나리오 설계, 발표자료 제작 |
| 석채경   | 발표 기획 및 프로젝트 구성 지원    |

---

## 8. 실물 사진

<p align="center">
 <img src="/images/engineer/도담_동서대학교_작품사진1.JPEG" alt="도담_동서대학교_작품사진1" width="900" />  
 <img src="/images/engineer/도담_동서대학교_작품사진2.png" alt="도담_동서대학교_작품사진2" width="900" /> 
</p>

---

## 9. 결론 및 향후 확장성

**도담(Dodam)**은 단순한 보조공학을 넘어, 시각장애인의 **학습 권리를 보장하고 흥미를 이끌어낼 수 있는 학습 플랫폼**입니다.  
기기 자체의 물리적 상호작용성은 AI 학습, 음성인식, 모바일 연동 등의 소프트웨어 확장성과도 잘 결합될 수 있어,  
향후 **디지털 점자교육의 핵심 솔루션**으로 발전할 수 있습니다.

> _누구나 읽고 배울 권리가 있다는 믿음,_  
> _도담은 그 믿음을 기술로 실현합니다._

<p align="center">
<img src="/images/engineer/IMG_8786.JPG" alt="IMG_8786" width="900" />
<img src="/images/engineer/IMG_8787.JPG" alt="IMG_8787" width="900" />
<img src="/images/engineer/IMG_8783.JPG" alt="IMG_8783" width="900" />
</p>

---
# 해결과정

팀 도담은 동서대학교 컴퓨터공학과 3명, 디지털미디어디자인전공 2명으로 이루어진 융합팀입니다.

서로 많은 의견을 공유하면서 우여곡절도 있었지만 협력하여 완성을 하였습니다.

초반 설계도입니다.

한글과 점자 동시에 학습할 수 있다는 점을 강조하였습니다.

![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcS51TUg2jG9KvykfoMaZet5MwRyRuraYzG4RlJmCMzJh3N_X1vil3ic88YxVyZeXztYgztPLXXlx-qkchpkGYTtmqDDATJ2FSQ_dSKROX91dpEhV-9Jhq-jaQnmOrHhtMu9MMyiSXqN81YFqb2VXdIN9k?key=Y4GgdiAtcR5dsCX8ouT4xw)

**1. led 컨트롤**  
<video src="/images/engineer/IMG_8565.MP4"></video>

led를 잘 컨트롤 되었는데 솔레노이드는 안되어 문제점을 찾아보았습니다.

충분한 전류를 주지 못하는것을 판단했고 솔레노이드를 컨트롤할 점자기판이 필요하여 시제품을 가져와 해체를 해보았습니다.

**2. 솔레노이드 액추에이터 적용**  
<p align="center">
<img src="/images/engineer/IMG_8578.JPEG" alt="IMG_8578" width="900" />
</p>

[솔레노이드 테스트 영상](https://www.youtube.com/watch?v=DieOwPJsSt8&list=PLzauXyUl51GkUwtiQZNXpspz1cbQXL3Oz&index=8)

잘되는것을 확인하고 직접 제작을 하였습니다.

**3. 외부 프레임 제작**
3D프린터를 통해 하우징 제작을 하였습니다.

<p align="center">
<img src="/images/engineer/IMG_8659.JPG" alt="IMG_8659" width="900" />  
<img src="/images/engineer/IMG_8671.JPEG" alt="IMG_8671" width="900" />  
<img src="/images/engineer/도담_동서대학교_작품사진1.JPEG" alt="도담_동서대학교_작품사진1" width="900" />  
<img src="/images/engineer/도담_동서대학교_작품사진2.png" alt="도담_동서대학교_작품사진2" width="900" />  
</p>

하드웨어로는 아두이노, 점자와한글을 표현하는 솔레노이드, 솔레노이드를 제어하는 점자모듈기판, 전원공급장치(SMPS)와 연결선 등이 있습니다

구현방법으로 flask로 웹사이트를 구축하고 컴퓨터와 tcp/ip통신으로 기기 제어 신호를 주고 받습니다. 컴퓨터는 시리얼 통신을 통해 아두이노보드에 수신한 신호를 전달합니다. 신호를 받은 아두이노는 솔레노이드 액추에이터를 제어 하는 방식입니다.

_[작품 코드](https://github.com/20201561KimGyeongHyeon/braille)_

