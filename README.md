# 작품명
* 메타트윈 데이터를 활용한 재난경보 민방위 교육
* 팀 LET's GO BOOGIE(LGB)

## 시연 영상

<div align="center">
  <a href="https://www.youtube.com/watch?v=wRqbwZSn-LA"><img src="https://img.youtube.com/vi/wRqbwZSn-LA/0.jpg" alt="IMAGE ALT TEXT"></a>
</div>

## 개요
* 최근, 우리나라에서는 다양한 재난 상황이 발생하고 있다. 하지만 교육에 대한 참여도와 관심은 여전히 낮은 상황이다. 이러한 상황에 맞춰 메타 트윈 데이터를 활용하여 재난 안전 교육 콘텐츠를 개발하고자 한다.

## 개발 배경 및 목적
* 최근, 우리나라에서는 화재, 태풍, 홍수와 같은 자연재해와 공습경보가 발령되었었다. 하지만 사람들 사이에서는 이러한 상황에 대한 교육에 흥미와 관심은 적다. 또한, 훈련에 참여하려면 모여서 훈련하거나 대피소로 이동해야 하는데, 이러한 실질적인 실천이 어려운 경우가 많다. 따라서 이러한 문제점들을 해결하기 위한 필요성이 대두되고 있다.

* 이러한 배경 아래, 디지털 기술과 메타 트윈 데이터를 활용하여 훈련 교육 콘텐츠를 개발하고자 한다. 이 프로젝트의 주요 목표는 아래와 같다.
  * 가상 세계에서 현실 세계와 같은 공간에서 훈련과 교육을 수행함으로써 교육을 받기 위해 이동하는 시간을 절약할 수 있도록 한다.
  * 디지털 트윈 데이터를 활용하여 현실에서 재현하기 어려운 재난 상황을 가상으로 생성한다. 이는 실제 상황에서 어떻게 대응해야 하는지에 대한 교육과 훈련을 실제처럼 체험할 수 있다.
  * 시뮬레이션 과정 중 수행한 행위에 따라 점수를 낮추거나 증가시켜 일정 점수 미만이면 교육을 다시 수행하도록 하여 재난 상황 시 수행해야할 행동 강령을 반복 숙달할 수 있는 프로그램을 개발한다.
  * 디지털 트윈 데이터를 통해 시물레이션 과정 중 현실과 거의 유사한 경험을 제공함으로써 훈련과 교육의 현실성과 효과를 높인다.

## 개발환경 및 개발언어
* 개발환경
  * Window 10, Unreal Engine 5, Visual Studio
* 개발언어 
  * C++, BluePrint

## 시스템 구성 및 아키텍처
<img src="https://github.com/wannaseoji/Metaverse_Developer_Contest/assets/105718365/39f9dbee-42f2-428f-b119-abfce69cdd51"/>

[프로젝트 구성도]
1. 시작시 사용자는 폭격 및 화재 상황을 선택할 수 있다. </br>
  1.1 난이도(상, 중, 하)와 성별(남, 여)를 선택한다.
2. 피교육자는 메타 트윈 데이터를 사용한 가상공간에서 실제 재난이 발생한 것 처럼 느낀다.
3. 재난 상황에서 발생할 수 있는 상황에 대한 대처를 하거나 임무를 수행할 수 있다.
4. 재난 대피 활동이 끝난다.</br>
   4.1. 성공시, 수료증을 확인할 수 있다.</br>
   4.2. 교육의 종류를 다르게 할 수 있다.</br>
   4.3. 실패시, 재교육을 시행한다.</br>
   4.4. 종료.

## 프로젝트 주요기능 
* 난이도 선택 기능
  * 사용자가 난이도를 상, 중, 하로 나누어 교육을 진행할 수 있다.

<div align = "center">
  
|교육|시간(분)|유도선 제공 여부|시작 점수|
|:---:|:---:|:---:|:---:|
|화재 경보 교육 |상 : 1</br>중 : 2</br>하 : 3|상 : X</br>중 : X</br>하 : O|상 : 50</br>중 : 60</br>하 : 70|
|공습 경보 교육 |상 : 3</br>중 : 4</br>하 : 5|상 : X</br>중 : X</br>하 : O|상 : 50</br>중 : 60</br>하 : 70|

</div>
</br>

* 미션 기능
<div align="center"><img src="https://github.com/wannaseoji/Metaverse_Developer_Contest/assets/91694379/0bec80b0-877f-4999-84f3-14d1155abd21"/></div>
  * 선택한 상황에 맞는 행동을 통해 행동강령을 수행하는 기능. 소화기를 집거나, 라디오를 챙기는 등의 행위를 상호작용을 통해 구현하였다.

</br>

* 점수 기능
<div align="center"><img src="https://github.com/wannaseoji/Metaverse_Developer_Contest/assets/91694379/e0a44406-e45f-40ef-ac58-38fcd10f9bb6"/></div>
  * 난이도 별, 점수를 토대로 깜짝 퀴즈, 미션 별 점수를 초기점수에 가감하여 총 결과에 반영한다.

</br>

* 재난 선택 기능
<div align="center"><img src="https://github.com/wannaseoji/Metaverse_Developer_Contest/assets/91694379/4f2fe297-6e42-4593-9523-c1eda0a4250d"/></div>
  * 교육받을 재난 상황을 선택할 수 있으며, 이후 난이도 선택을 통해 더욱 현실과 같은 상황을 경험할 수 있다.
  * 공습 상황 대응 교육
    * 공습 상황 발생 시 수행할 행동 강령을 교육 받을 수 있도록 상황을 제공한다.
  * 화재 상황 대응 교육
    * 화제 상황 발생 시 수행할 행동 강령을 교육 받을 수 있도록 상황을 제공한다.
</br>

* 뉴스 기능
<div align="center"><img src="https://github.com/wannaseoji/Metaverse_Developer_Contest/assets/91694379/5944916e-679d-4af1-8313-483f2eb766d7"/></div>
  * 시뮬레이션 시작 시 뉴스 화면을 제공하여 현재 상황에 대해 사용자에게 효과적으로 전달할 수 있다.
</br>

* 휴대폰 기능
<div align="center"><img src="https://github.com/wannaseoji/Metaverse_Developer_Contest/assets/91694379/56b8de74-2be2-449c-805d-e3e2091f7f7b"/></div>
  * 시뮬레이션 속 휴대폰 기능을 통해 재난 상황 발생 시 수행하면 좋은 행동에 대한 힌트와 대피소 장소에 대한 힌트를 얻을 수 있다.
</br>

* 깜짝 퀴즈 기능
<div align="center"><img src="https://github.com/wannaseoji/Metaverse_Developer_Contest/assets/91694379/60c82002-3564-40d0-a251-39e7fe151ea2"/></div>
  * 시뮬레이션 중 일정 시간이 지나면 휴대폰을 통해 깜짝 퀴즈를 출력하여 재난 상황 발생 시 기억하면 좋을 지식을 얻을 수 있다.
</br>

* 사무실 기능

  * 시뮬레이션 시작 시 처음 움직일 수 있는 공간이다. 이 공간에서 재난이 시작되었음을 알 수 있으며, 실내 공간에서 해야 할 일과, 하지 말아야 할 일을 교육받을 수 있다.
</br>

* AI Human 기능
<div align="center"><img src="https://github.com/wannaseoji/Metaverse_Developer_Contest/assets/91694379/939bdbb8-efdf-41e4-9ee3-af62ce615855"/></div>
  * AI Human를 통해 대피소의 위치를 유추할 수 있고, 또한 가짜 대피소로 달려가거나 손짓하는 AI Human을 배치하여 사용자에게 올바른 대피소로 이동할 수 있도록 교육한다.
</br>

* 대피소 유도 기능
<div align="center"><img src="https://github.com/wannaseoji/Metaverse_Developer_Contest/assets/91694379/e291baab-0fac-4ed1-875d-dc20b712734f"/></div>
  * 도심으로 이동하였을 때 “하” 난이도의 경우 대피소로 이동할 경로에 대해 보여주어 장소에 대한 숙지가 되어 있지 않은 경우 도움을 줄 수 있는 기능이다.
</br>

* 타이머 기능
  * 시뮬레이션 시작 시 선택한 난이도에 따라 시간 제한을 두고, 모든 시간이 경과 하면 교육을 수료하지 못하게 한다.
</br>

* 결과표 기능
<div align="center"><img src="https://github.com/wannaseoji/Metaverse_Developer_Contest/assets/91694379/ac124758-4a3e-4b94-8e9e-ec3b39cf7fd9"/></div>
  * 마지막 화면에서 교육 결과에 대한 수행 여부를 한눈에 확인할 수 있습니다.

## 기대효과 및 활용분야
* 교육효과 증진 및 비용 감소
  * 현실과 유사한 디지털 트윈 데이터를 활용하여 교육 환경을 구성하여 교육 효과를 증진할 수 있다. 또한, 가상 현실 속에서 교육을 받을 수 있어 이동하는 비용과 교육 수행 시 필요한 인원에 대한 비용도 감소시킬 수 있다.

* 반복적 교육 시뮬레이션
  * 점수 시스템을 통해 일정 수준 이상 행동 강령을 지키지 못한다면 숙지할 때 까지 반복해서 교육을 받을 수 있다. "시간"과 "공간"을 넘어 "리얼공간"에서 교육 및 훈련을 할 수 있다. 행동 강령을 숙지할 때까지 반복하여 수행할 수 있다.

* 다양한 교육 경험 제공
  * 재난 상황 발생 시 챙겨야 할 물건을 집어 챙길 수 있고, 이용하지 말아야 할 장소에 접근 시 안내 메시지를 출력한다. 또한, 깜짝 퀴즈와 같은 요소를 통해 다양한 교육 요소를 시뮬레이션 속에 녹아들게 하여 사용자에게 다양한 교육 경험을 제공할 수 있다.
