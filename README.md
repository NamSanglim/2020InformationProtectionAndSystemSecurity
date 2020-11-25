# :computer: 2020InformationProtectionAndSystemSecurity :computer:
>### Kookmin University 정보보호와 시스템보안 - AI 악성코드탐지 프로젝트 과제 

## :boy: Project Member  :girl:
- [20171594 김선우](https://github.com/sunwoopia)
- [20171726 황효빈](https://github.com/gyqls980)
- [20191584 남상림](https://github.com/Sanglim00)

## Project Goal
PE파일이 주어졌을 때, 주어진 파일이 악성파일인지 정상파일인지 판별하는 이진 분류기 모델을 만드는 것

## Period
2020/11/03 (Tuesday) ~ 2020/11/28 (Saturday)

## Problem
- 주어진 파일에서 어떤 특징이 악성의 근거가 되는 지 모른다.
- 분류기를 어떻게 만들 지 모른다.

👉 파일의 특징을 최대한 추출한 후, 이 특징들을 머신러닝으로 학습시켜 주어진 파일이 악성이 되는 조건을 찾자 !

## How :question:
1️⃣ 특징 추출 및 전처리
> 머신러닝 악성 코드 탐지 기술을 사용하여 json파일의 각 **특징**을 추출한다.
>
> 추출한 특징을 가공하여 고정 크기의 특징 벡터를 생성한다. (정상 파일 : 0, 악성 파일 : 1)
>
>⇨ 생성한 **특징 벡터는 주어진 파일을 대표**하게 된다 !

2️⃣ 학습시키기
>생성한 특징 벡터을 사용하여 해당 파일이 악성인지 정상인지를 판별하는 머신러닝 모델을 만들자!
>
>학습데이터를 구성하여 지도학습 방법으로 **머신러닝 모델을 학습** 할 것이다.
>
>우리가 사용한 머신러닝 모델 : RandomForestClassifier, SVC, LGBMClassifier

3️⃣ 성능 평가하기
>학습시킨 모델이 잘 학습이 되었는지 확인해야 하기 때문에 주어진 데이터 정답표를 이용하여 정확도를 예측한다.
