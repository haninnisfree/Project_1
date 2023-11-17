# 🚀 Project1 - 변동성 예측 지표를 활용한 옵션 데이트레이딩 전략 수립

---

## 팀 소개 
- **팀 이름:** "ON"
    - Ubi : on 
    - Opti : on 
    - Predict : on 
    - Switch : on 🎚
- **팀원 소개:**
  * 이승희: 팀장, 발표자료제작, 모델링 
  * 한정윤: 큐레이터, 데이터 수집 및 전처리, 백테스팅
  * 위재욱: 데이터 수집 및 전처리, 백테스팅 
  * 유신욱: 데이터 수집, 데이터 시각화 
  * 한인희: 데이터 전처리, 모델링, 서기 

---

## 연구 주제 및 배경 🎯
* 연구 주제 : 변동성 예측 지표를 활용한 옵션 데이트레이딩 전략 수립
### 1. 옵션에 대한 관심도 증가 
* 최근 옵션 시장에서는 거래량이 상승하고 있으며, 이는 옵션에 대한 관심도가 증가하고 있음을 시사함. 이러한 추세는 옵션 시장의 잠재적 성장 가능성을 보여주며, 투자자와 연구자에게 새로운 기회를 제공할 것으로 예상됨.
### 2. 옵션 트레이딩의 변질 문제 
* 옵션 트레이딩이 본래의 목적인 선물 시장의 헷지 도구로서의 역할에서 벗어나, 단기 수익 추구 수단으로 변모하고 있음.이러한 변질을 이해하고, 올바른 옵션 트레이딩 전략을 수립하기 위한 연구가 필요함을 강조함.
### 3. 옵션 트레이딩의 위험성 
* 베어링스 은행의 파산 사례와 같이, 옵션 트레이딩은 높은 수익률을 제공할 수 있지만, 그에 따른 위험성도 매우 높음. 이러한 위험성을 줄이면서도 수익성을 추구할 수 있는 전략의 개발이 필요함을 시사함.
---
  
 ## 연구 목표
변동성을 예측함으로써 리스크 관리뿐만 아니라 적절한 매매 전략을 사용하여 수익을 낼 수 있는 모델 개발을 목표로 함

---
## 워크플로우 
1. 데이터 수집 
2. 데이터 전처리 
3. 스케일링 & 리샘플링 
4. 통계 검증 
5. 피처 선택 
6. 모델링 
7. 성능 평가 

---

## 데이터셋 📊
- **기간:** 6월 12일부터 11월 3일까지
  - **train data:** 6월 12일 ~ 10월 6일(7월물~10월물)
  - **test data:** 10월 10일 ~ 11월 3일(11월물)
- **데이터 분류:** 옵션 거래의 데이터 분석에 있어서, 선물의 표준 만기 주기인 3개월 간격을 맞추고자 하였으나, 7월부터 10월까지 공휴일로 인한 거래일 부족 문제를 해결하기 위해 1개월치 데이터를 추가함

---

## 데이터 분포 및 이상치 탐색
* describe를 통해 데이터의 분포를 대략적으로 확인
* 이상치는 유의미한 것으로 판단
  -> 변동성이 커질 때를 잘 예측해주는 중요 정보로 예상됨

---

## 피처 선택 🔍 
- 로지스틱 회귀 + 라쏘 방법과 상관계수 + 피처 중요도 방법 비교

---

## 모델링/백테스팅 🤖  
- 변동성 예측 실패의 위험성 분석
- 트레이딩 전략의 백테스팅 결과
- 라벨링 변경의 이유와 방법
- 양매수, 양매도, 머신러닝 기반 전략 비교

---

## 결과 및 결론 💡
- **베어링스 은행 사례:** 결정적인 파산 원인 분석
- **변동성 예측 모델:** 변동성이 큰 날을 예측하는 모델 개발의 중요성
- **전략 수립:** 위험성을 줄이고 수익을 극대화하는 전략 제안
- **백테스팅 결과:** 이론상 양매도 스트랭글 및 양매수 스트래들 전략의 안정성 분석


# 🚀 Project1 - Option Day Trading Strategy Using Volatility Prediction Indicators

---

## Team Introduction 
- **Team Name:** "ON"
    - Ubi : on
    - Opti : on
    - Predict : on
    - Switch : on 🎚
- **Team Members:**
  * Seung-hee Lee: Team Leader, Presentation Material Production, Modeling
  * Jeong-yun Han: Curator, Data Collection and Preprocessing, Backtesting
  * Jae-wook Wi: Data Collection and Preprocessing, Backtesting
  * Shin-wook Yu: Data Collection, Data Visualization
  * In-hee Han: Data Preprocessing, Modeling, Secretariat

---

## Research Topic and Background 🎯
* Research Topic: Development of an Option Day Trading Strategy Using Volatility Prediction Indicators
### 1. Increasing Interest in Options 
* There is a growing interest in options trading, evidenced by increasing trade volumes.
    -> This trend suggests potential growth in the options market, offering new opportunities for investors and researchers.
### 2. The Distortion of Option Trading 
* Option trading has deviated from its original purpose as a hedging tool in the futures market and has become a means for short-term profit pursuit.
    -> This change underscores the need for research to understand this distortion and establish proper option trading strategies.
### 3. The Risk of Option Trading 
* As illustrated by the Barings Bank collapse, option trading can offer high returns but also comes with high risk.
    -> There is a need to develop strategies that minimize risk while pursuing profitability.
### 4. Case Study Problem Statement: Lessons from the Collapse of Barings Bank 
The collapse of Barings Bank was primarily due to the failure to manage the significant risks that arose from unexpected increases in volatility while using a short-selling strategy.
    -> This case highlights the importance of accurately predicting volatility in option trading.

---
  
 ## Research Goals
Our goal is to develop a model that can predict days with high volatility, allowing for risk management and profit generation through appropriate trading strategies.

---

## Why Predict Volatility?
* Understanding Delta Neutrality through Greeks - additional content needed
* Reasons for predicting VKOSPI specifically - additional content needed
---
## Workflow 
1. Data Collection 
2. Data Preprocessing 
3. Scaling & Resampling 
4. Statistical Verification 
5. Feature Selection 
6. Modeling 
7. Performance Evaluation 

---

## Dataset 📊
- **Period:** June 12 to November 3
  - **Train data:** June 12 to October 6 (July to October contracts)
  - **Test data:** October 10 to November 3 (November contracts)
- **Data Classification:** While aiming for the standard 3-month maturity cycle of futures for options trading data analysis, we added an extra month of data due to a lack of trading days from July to October caused by holidays.

---

## Data Distribution and Outlier Exploration
* Data distribution was roughly reviewed through the 'describe' function.
* Outliers were considered meaningful.
  -> They are expected to provide significant information for predicting when volatility increases.

---

## Feature Selection 🔍 - additional content needed
- Comparison between logistic regression + LASSO method and correlation coefficients + feature importance method

---

## Modeling/Backtesting 🤖  - additional content needed
- Analysis of the risks of failing to predict volatility
- Backtesting results of the trading strategy
- Reasons and methods for changing labeling
- Comparison between long buying, short selling, and machine learning-based strategies

---

## Results and Conclusion 💡
- **Barings Bank Case Study:** Analysis of the critical cause of collapse
- **Volatility Prediction Model:** The importance of developing a model to predict days with high volatility
- **Strategy Establishment:** Proposal of strategies that maximize profit while reducing risk
- **Backtesting Results:** Analysis of the stability of theoretical short strangles and long straddles strategies
- **Benchmark Performance:** Comparison with past benchmark-beating results

![image](https://github.com/haninnisfree/Project_1/assets/144647781/ea5316d8-356a-4717-810a-7f556db3d9c3)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/05667bc2-2221-4974-8ce9-2b70567b72c6)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/b5608abe-af9b-46e3-b056-074a2aa8fcd2)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/36cbd955-678c-4ab5-adb1-ce0a12bb5c49)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/c86d5d59-320a-412c-8315-c8e793f62f25)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/7dc42fcc-b60e-4456-80ee-20367e692d1f)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/a6c9bc9f-3349-4e6b-b133-f58ac64a348d)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/0a0ce0da-62b8-45bf-8d4c-5c63728dd819)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/818cab0f-ff47-4832-8d9d-64fba77efa82)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/91240cad-708a-4ab3-9e59-176e2f1e5e75)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/6f912581-dbdf-4455-93de-450d67d7d8e5)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/8de1157e-310c-41c7-849f-883e2f9b8138)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/d905b826-fc94-4cd8-b344-89358ece462f)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/b2f66594-6ade-4878-9308-5d4af00a37d9)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/7ac7e60b-9fce-44a3-84b0-8938166fc384)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/ac04612c-54ad-4a09-8883-8ffaca2acde7)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/f50bb732-6b7a-4cf4-a6db-8cbfa2501305)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/995cc1e3-e0b5-41f5-bf26-453aa8304448)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/67a89c77-1780-4c00-8227-49c9a99ce953)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/623a1bfd-33b0-4622-865d-916dced5f994)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/6ca6122e-32dd-490f-bb95-a4addb1d4b94)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/5e478a96-0f73-411b-b257-74259d645a6a)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/83042e25-68bf-48d3-a250-9bf6dbbf183e)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/9aab48f9-41f4-49d7-9ba9-a2eade4bbb30)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/390508c2-b708-483b-940a-40c4c9a4bbb5)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/200467d2-26fa-4c44-855c-84d3da4b0dd1)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/ee34c591-d1b7-4e54-b09f-edf2717eb638)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/5bc9da2e-1f2e-4f30-baa0-648fb95ddec0)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/6044aa12-4b80-41a4-a488-74a03f9d5e3e)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/e69bae16-7d24-421c-a883-a0850bdf267d)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/6343d287-1260-44de-a322-426a4f121c26)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/f292e0ec-ebce-4c68-9b36-e89611d24764)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/6331335f-c00b-48fe-b009-5e9bdae9c0b3)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/3b64999a-f1a0-4bc2-86bb-890a948c7f85)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/2013aada-0c78-4364-9687-afa3e646dcfc)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/0bd85c79-5422-48ff-b408-d06c0ed27238)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/cf3e5d1d-917c-4232-8877-8f833ec15381)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/3b356d4b-9b70-4495-bbee-71212cff0bde)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/9b337404-42cd-4d6c-8251-53951a8f035d)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/d6f354fe-a5a1-492c-9195-067f243ddf1d)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/3fda318b-98c1-4626-a88d-88a7e8da8487)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/d352c8dc-119b-4048-afa8-87021f8c1170)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/5d5cf761-6bab-4a70-9dfc-c6626cbe4ab3)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/33e2726d-0e9c-4543-978a-43b41d9e49f0)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/e3cfc7c6-cb3b-465d-9698-b5c8fbd4673e)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/0eaa145b-e6ec-4a29-a946-68883bb0f1b3)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/44f8bc41-be42-4b90-88a3-b6e384a2b084)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/a22b62af-7a9a-4554-a66b-48644cb829a1)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/31697eac-7110-475c-9f28-999a4745f530)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/a9d7c202-69c7-4a10-adfc-acdc085025ff)
![image](https://github.com/haninnisfree/Project_1/assets/144647781/8659766a-c714-4d5c-914b-3f4412645111)





