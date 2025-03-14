---
layout: single
title: "2024 창의적 종합설계 경진대회"
categories: ExternelActivity
tag: [AI, RaspberryPi, Arduino]
date: 2024-09-27
typora-copy-images-to: ..\images\engineer
---

# 2024 창의적 종합설계 경진대회

2024.11.07

8월부터 진행했던 프로젝트를 완성하여 11월7일에 부경대학교에서 발표를 하였습니다.

팀 도담은 동서대학교 컴퓨터공학과 3명, 디지털미디어디자인전공 2명으로 이루어진 융합팀입니다.

서로 많은 의견을 공유하면서 우여곡절도 있었지만 협력하여 완성을 하였습니다.

초반 설계도입니다.

한글과 점자 동시에 학습할 수 있다는 점을 강조하였습니다.

![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcS51TUg2jG9KvykfoMaZet5MwRyRuraYzG4RlJmCMzJh3N_X1vil3ic88YxVyZeXztYgztPLXXlx-qkchpkGYTtmqDDATJ2FSQ_dSKROX91dpEhV-9Jhq-jaQnmOrHhtMu9MMyiSXqN81YFqb2VXdIN9k?key=Y4GgdiAtcR5dsCX8ouT4xw)

led 컨트롤 부터 시작하였습니다. 

<video src="..\images\engineer\IMG_8565.MP4"></video>

led를 잘 컨트롤 되었는데 솔레노이드는 안되어 문제점을 찾아보았습니다.

충분한 전류를 주지 못하는것을 판단했고 솔레노이드를 컨트롤할 점자기판이 필요하여 시제품을 가져와 해체를 해보았습니다.

<img src="..\images\engineer\IMG_8578.JPEG" alt="IMG_8578" style="zoom:25%;" />

[솔레노이드 테스트 영상](https://www.youtube.com/watch?v=DieOwPJsSt8&list=PLzauXyUl51GkUwtiQZNXpspz1cbQXL3Oz&index=8)

잘되는것을 확인하고 직접 제작을 하였습니다.

3D프린터를 통해 하우징 제작을 하였습니다.

<img src="..\images\engineer\IMG_8659.JPG" alt="IMG_8659" style="zoom:25%;" />

<img src="..\images\engineer\IMG_8671.JPEG" alt="IMG_8671" style="zoom:25%;" />

<img src="..\images\engineer\도담_동서대학교_작품사진1.JPEG" alt="도담_동서대학교_작품사진1" style="zoom:25%;" />

<img src="..\images\engineer\도담_동서대학교_작품사진2.png" alt="도담_동서대학교_작품사진2" style="zoom:50%;" />

하드웨어로는 아두이노, 점자와한글을 표현하는 솔레노이드, 솔레노이드를 제어하는 점자모듈기판, 전원공급장치(SMPS)와 연결선 등이 있습니다

구현방법으로 flask로 웹사이트를 구축하고 컴퓨터와 tcp/ip통신으로 기기 제어 신호를 주고 받습니다. 컴퓨터는 시리얼 통신을 통해 아두이노보드에 수신한 신호를 전달합니다. 신호를 받은 아두이노는 솔레노이드 액추에이터를 제어 하는 방식입니다.

시연영상입니다.

[작품시연영상](https://youtu.be/DieOwPJsSt8?list=PLzauXyUl51GkUwtiQZNXpspz1cbQXL3Oz)

해당 작품으로 창의적 종합설계 경진대회에 참여하여 은상을 수상하였습니다.

<img src="..\images\engineer\IMG_8786.JPG" alt="IMG_8786" style="zoom: 50%;" />

<img src="..\images\engineer\IMG_8787.JPG" alt="IMG_8787" style="zoom: 50%;" />

<img src="..\images\engineer\IMG_8783.JPG" alt="IMG_8783" style="zoom:50%;" />

작품 코드 : https://github.com/20201561KimGyeongHyeon/braille

