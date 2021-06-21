## 2020년 가을학기 고급데이터마이닝 프로젝트

## 주제: 청소년 비만 예측 및 패턴도출
 - ParentsLikeMe에 대한 Business Problem을 정의하고, 이를 Data Science Problem으로 전환하여 해결하고자함
 
### 프로젝트 세분화
 - Proposal - Intermediate - Final로 구성되어 있음. 
 
 (1) **Proposal**
  > Business Problem을 정의하고 Data understanding이 주가 되는 단계로 향후 청소년 비만 예측 및 패턴도출을 어떻게 적용할 것인지 큰 그림을 그리는 단계
 
 (2) **Intermediate**: 
  > 본격적인 분석을 수행하는 단계. 청소년 비만에 대해 가장 좋은 예측력을 시사하는 머신러닝 모델(SVM, RF, MLP 등)을 파악하기 위하여 데이터를 남자, 여자, 전체 청소년으로 구분하고 스케일링, KFOLD, 결측치 처리 방법을 고려하여 가장 좋은 모델을 휴리스틱하게 도출.
 
 (3) **Final**: 
  > RF, LR, SVM, MLP에 대하여 오버샘플링을 실시해보고 PCA, K-mean 등에 입각한 전처리 기법을 적용해보며 성능 향상여부를 파악한다. 더불어 변수중요도를 도출해 실제 비만에 가장 유의미한 인자가 무엇인지 파악한다.

### 활용데이터
 - 국민건강영양조사(16-18년): 데이터는 아래 사이트에서 받으실 수 있습니다! 저작권상 따로 첨부는 하지 않았습니다.
 https://knhanes.kdca.go.kr/knhanes/sub03/sub03_02_05.do
