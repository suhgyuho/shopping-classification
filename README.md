# Kakao-Shopping-Classification

쇼핑 상품의 상품명, 브랜드명, 모델명, 가격, 이미지 정보들을 이용해 쇼핑 상품을 2000여개의 카테고리로 분류하는 연구

## Introduction

실제 카카오에서 진행했던 "쇼핑몰 상품 카테고리 분류" 대회는 코드를 실행하기 위해 최소 450GB 용량이 필요했기 때문에 수업 조교분들이 Google Colab에서 돌릴 수 있는 정도의 수준으로 데이터를 줄여 진행하였음.

카카오 대회에서는 쇼핑몰 상품 데이터를 57개의 대분류, 552개의 중분류, 3190개의 소분류, 404개의 세분류 카테고리로 분류해야하지만 이 프로젝트에서는 쇼핑몰 상품 데이터를 52개의 대분류, 463개의 중분류, 2070개의 소분류, 183개의 세분류 카테고리로 분류함.

## Idea
상품명, 브랜드명, 모델명 같은 경우에는 인접한 단어들의 정보를 함께 Embedding 하도록 preprocessing함.
그러나 Unique한 데이터가 너무 많아졌기 때문에 문자열 알고리즘을 통해 비슷한 단어들을 한 분류로 묶이게 하여 Embedding함.
인공신경망 구조는 다 똑같기 때문에 전처리 작업만으로 성능을 끌어올림

## Result
Test Score 1.11923을 얻으며 수강생 50여명 중 가장 정확한 쇼핑 상품 분류 모델을 구현함
<br/><br/>
![image](https://user-images.githubusercontent.com/87184009/127636091-1dd2562d-9d7b-4812-beab-06475731f00d.png)


## References

KAIST CoE202: Fundamentals of Artificial Intelligence \
http://kalman.kaist.ac.kr/coe202/

쇼핑몰 상품 카테고리 분류\
https://arena.kakao.com/c/5 \
https://github.com/kakao-arena/shopping-classification
