## Intermediate Report

### Introduction ( 대상 기업 : PatientsLikeMe – “환자들의 페이스북” )
 - 세계 비만 인구는 2008년 기준 총 14억 명, 매년 약 280만 명이 비만 관련 질병으로 사망
 - 청소년기 비만은 성인으로 이어짐 ➔ 청소년 비만 사전 예측 및 비만 유발 요인 파악이 중요
 
### Methods
 - 국민건강영양조사 및 청소년 건강행태 조사에 참여한 청소년 대상으로 분석 수행
 - 기존에 발표된 청소년 비만 관련 논문을 바탕으로 Feature Selection
 - EDA (탐색적 분석) : 다중 공선성, 데이터 시각화를 통한 Feature의 Value 분포, 통계량 등 확인
 - 3개 데이터셋, 4가지 결측치 처리 방법, 2가지 데이터 스케일링, K=5/10인 K-fold 교차 검증 수행
 - 6가지 분류기법(NB Classifier, RF, LR, K-NN, SGD, SVM)사용
  > 모델 별 그리드 서치 수행하며 청소년 통합/남자/여자 데이터 각각에 대해 144개의 모델 수립.
  
### Results 및 Discussion
 ![image](https://user-images.githubusercontent.com/28617435/122832329-27824980-d326-11eb-9e74-3350b46a5f5d.png)

 - “결측치 처리 방법” 에는 각 데이터별로 가장 높은 성능을 보인 결측치 처리 방법을 기재함
  > ( 평균=평균값 대체, 중앙=중앙값 대체, 최빈=최빈값 대체, 완전=완전 제거법을 의미함)
 - △는 세 데이터 중 하나라도 K값을 증가시켰을 때 성능이 하락한 경우를 의미
  > 참고 : SGD는 파라미터 변경 시 사용하는 모델 기법이 달라져서 위 표에서 제외함
 - SGD가 남녀 통합 데이터/남자 데이터에서, NB Classifier가 여자 데이터에서 Recall이 우수
 
 ![image](https://user-images.githubusercontent.com/28617435/122832274-15081000-d326-11eb-9635-c80c9770afc5.png)

  > 청소년 남자 비만과 청소년 여자 비만에 유의미한 인자에 차이가 있음을 확인
 
### Limitation
 - 컴퓨팅 리소스의 한계, 가중치 적용의 한계, 결측치 처리 방법의 한계

