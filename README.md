# 2023년 제3회 K-인공지능 제조데이터 분석 경진대회
이 프로젝트는 "제2023년 제3회 K-인공지능 제조데이터 분석 경진대회"에서 183팀 중 ~~상을 수상한 데이터 분석 프로젝트입니다. 프로젝트의 목적은 인공지능 중소벤처 제조플랫폼(KAMP) 내 등재된 제조AI데이터셋을 활용하여 중소 제조기업이 직면할 수 있는 문제를 해결하거나 개선할 수 있는 우수한 인공지능 분석 모델을 개발하는 것입니다.

저희 팀, 'Absolute A'는 시계열 딥러닝 예측 모델을 사용하여 불량 공정의 시간표현을 탐지하고 요인분석을 진행했습니다. LSTM, GRU, TCN, Transformer 등의 모델을 사용하고, 이들 모델에서 도출된 변수의 중요도(Shapley Value 기반)를 분석했습니다. 

본 프로젝트는 실시간 데이터 분석을 가능하게 하여, 공정 중 발생하는 문제에 신속하게 대응할 수 있는 방법을 제시했습니다. 이러한 접근 방식은 제조업의 설비 운영에서 데이터 기반 의사결정의 중요성을 강조하며, 품질 유지 및 생산 효율 향상에 직접적으로 기여합니다. 결과적으로 이는 비용 절감 및 운영 효율성 증진으로 이어질 수 있음을 시사합니다.

이 README 문서는 프로젝트의 개요와 목적, 사용된 기술 및 도구, 결과 요약 등을 제공하여 프로젝트에 대한 간략한 소개를 제공하고자 합니다. 본 프로젝트는 인공지능 및 데이터 분석 분야에서의 딥러닝 접근을 보여주며, 유사한 문제를 해결하고자 하는 다른 분석가들에게 유용한 참고 자료가 될 것입니다.

## 공모전 개요
  - <b>공모전 명칭</b>: 제2023년 제3회 K-인공지능 제조데이터 분석 경진대회
  - <b>목적</b>: 인공지능 중소벤처 제조플랫폼(KAMP) 내 등재된 제조AI데이터셋을 활용하여 중소 제조기업이 직면할 수 있는 공통문제*를 해결 또는 개선할 수 있는 우수한 인공지능 분석 모델 개발 
  - <b>주최</b>: 중소벤처기업부, 스마트제조혁신추진단, KAIST
  - <b>대회 일정</b>:
    - 대회 공지 : 2023/9/25
    - 참가팀 모집 : 2023/10/10 ~ 2023/10/20
    - 문제발표 및 과제해결:  2023/10/23 ~ 2023/11/03
    - 1차 서면평가 및 결과발표 : 2023/11/10
    - 2차 발표평가 : 2023/11/21
    - 시상식 : 2023/11/28
  - <b>제공되는 데이터</b> 
    - 인공지능 중소벤처 제조플랫폼(KAMP) 내 등재된 제조AI데이터셋(총 50종) 중 무작위 1개 선정
  - <b>공모전 사이트</b> : https://www.kamp-ai.kr/cptContestInfo?cptSeq=20 
  - <b>개최안</b> : [공모전 개최(안).pdf](https://github.com/passion3659/2023_Crime_Safety_Data_Analysis_Competition/files/11648459/default.pdf)

## 공모전에서의 팀의 역할과 기여
- <b>팀 구성</b>
  - 팀명 : Absolute A
  - 팀장 : 배소희
  - 팀원 : 박정원, 양정열
- <b>분석 배경</b>
  - 설비 고장으로 인한 불량 제품의 증가
  - 설비 검사 기간 동안 생산 중단으로 인한 손실
  - 장비 운용을 경험에 의존하는 경향으로 인해 운영의 효율성과 최적화가 저해됨
- <b>본 팀에서의 기여</b>
  - 하나의 공정을 불량 공정, 정상 공정으로 간주하여 labeling 후 60초의 time series에 대해서 분류를 진행함
  - LSTM, GRU, TCN, Transformer의 모델을 사용하였고 최고의 성능을 내는 모델을 채택함
  - 가장 성능이 좋은 모델을 기반으로 shapely value를 계산해 불량에 기여하는 변수를 파악함
