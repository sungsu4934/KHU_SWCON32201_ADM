## Proposal

### 1. Business Understanding
 - Business Problem(BP): 청소년 비만에 대한 예측 및 패턴도출
 
 - Data Science Problem(DSP): SGD, SVM, Random Forest, Logistic Regression, Naive Bayes Classifier, KNN Classifier 등 분류기법을 통한 청소년 비만 패턴 파악

 - 연구의 필요성 및 중요성
  > 1) WHO: "비만은 21세기 신종 전염병"
  > 2) 세계 비만 인구는 총 14억명
  > 3) 매년 280명이 비만관련 질병으로 사망
  > 4) 외모로 인한 사회적 낙인을 경험할 위험 존재
  > 5) 성인비만까지 지속될 높은 확률
  > 6) 각종 만성질환, 심혈관 질환, 정신적 질환에 노출 가능성

 - 연구의의
 
  > 1) 청소년 비만관리를 위한 프로그램 개선
  > 2) 청소년 전체가 아닌 각 성별에 따른 연구
  > 3) 한국을 넘어 국가별 청소년 비만예방 후속연구의 초석

### 2. Data Understanding

 - Strength
  > 1) 우수한 접근성 & 활용성
  > 2) 필요 데이터 추출 용이
  > 3) 공공 데이터 → 높은 신뢰도
 
 - Limitation
  > 1) 외부적 요인에 영향
  > 2) 연도별 다른 일부 설문항목
  > 3) 변수간 선후관계 파악이 어려움
  > 4) 자가 보고된 신장과 체중(과소추정의 가능성)
  
 - Benefit
  > 1) 대대적으로 공개된 공공데이터
  > 2) 비용이 발생하지 않으며 데이터 수집에 대한 시간소요가 적음
  
 - Cost
  > 1) 700개가 넘는 Attribute → 유의미한 변수선정 및 결측치 처리의 어려움
  > 2) 범주형 데이터와 수치형 데이터의 혼재 → 범주형 변수 파악 및 onehotencoding에 시간과 노력이 소요

### 3. (Expected) Data Preparation
 - 새로운 변수 및 파생변수 할당 (BMI, 하루평균 수면시간 등)
 - 결측치 방법론 구상
  > 1) 결측치가 포함된 OBS를 삭제, 결측치가 특정 %이상(ex. 10%, 20% 등)인 변수 삭제
  > 2) 결측치 대체(중앙값, 평균값, 최빈값 등)
 - 탐색적 데이터 분석(EDA): 기초 통계량, 데이터의 분포확인 및 이상치 파악
 - 데이터 스케일링: 표준화 또는 정규화
 - 층화 추출법: 모집단을 구분하는 2개 이상 class에 비례하게 '단순 무작위 추출방법'으로 표본 추출

### 4. (Expected) Modeling

 - 머신러닝 방법론
  > 1) SGD Classifier
  > 2) Support Vector Machine
  > 3) Random Forest
  > 4) Logistic Regression
  > 5) Naive Bayes Classifier
  > 6) KNN Classifier
  
 - Class Imbalance 해소 방법론
  > 1) Weight Balancing: 학습 데이터에서 loss를 계산 시 특정 클래스에 대해서는 더 큰 loss를 계산
  > 2) Upsamping
  > 3) Downsampling
  
 
### 5. (Expected) Evaluation
 - KFOLD 교차검증
 - Confusion matrix & AUC (Accuracy, Precision, Recall, F_b Score, AUC)
 - 분석 타당성
  > 1) 국민건강영양조사 데이터를 직접 추출 및 분석
  > 2) 필요 Attribute를 논문 바탕 선별
  > 3) 다양한 분류기법마다 적절히 변형된 Input data를 통해 도출된 Performance Measure로 높은 신뢰도
  
 - 분석 한계
  > 1) 국민건강영양조사 데이터에 기반한 분석은 국내 청소년에 국한되어 있기에 전세계적 적용에 한계
  > 2) 데이터의 부족으로 모델의 성능
 
 

