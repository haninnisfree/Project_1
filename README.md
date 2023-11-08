# 🚀 Project1 - 변동성 예측 지표를 활용한 옵션 데이트레이딩 전략 수립

---

## 팀 소개 
- **팀 이름:** "ON"
    - Ubi : on 
    - Opti : on 
    - Predict : on 
    - Switch : on 🎚
- **팀원 소개:**
  👩‍💼이승희: 팀장, 발표자료제작, 모델링 
  👨‍💼한정윤: 큐레이터, 데이터 수집 및 전처리, 백테스팅
  🕵️‍♂️위재욱: 데이터 수집 및 전처리, 백테스팅 
  🧑‍🔬유신욱: 데이터 수집, 데이터 시각화 
  👩‍🔬한인희: 데이터 전처리, 모델링, 서기 

---

## 연구 주제 및 배경 🎯
* 연구 주제 : 변동성 예측 지표를 활용한 옵션 데이트레이딩 전략 수립
### 1. 옵션에 대한 관심도 증가 
* 최근 옵션 거래에 대한 관심 증가와 거래량 상승하고 있음. 
    -> 이는 옵션 시장의 잠재적 성장 가능성을 시사하며, 이는 투자자와 연구자에게 새로운 기회를 제공할 것으로 보임
### 2. 옵션 트레이딩의 변질 문제 
* 옵션 트레이딩이 본래의 목적인 선물 시장의 헷지 도구로서의 역할에서 벗어나, 단기 수익 추구 수단으로 변질되고 있음
    -> 이러한 변질을 이해하고 올바른 옵션 트레이딩 전략을 수립하기 위한 연구의 필요성을 보여줌
### 3. 옵션 트레이딩의 위험성 
* 베어링스 은행의 파산 사례와 같이 옵션 트레이딩은 높은 수익률을 제공할 수 있지만, 그에 따른 위험 역시 높음
    -> 이러한 위험성을 줄이면서도 수익성을 추구할 수 있는 전략을 개발
### 4. 사례를 통한 문제제기 : 베어링스 은행 파산의 교훈 
베어링스 은행의 파산은 양매도 전략을 사용하던 중 예상하지 못한 변동성의 증가로 인한 큰 위험을 관리하지 못한 데에 주된 원인이 있음.
    -> 이 사례는 옵션 거래에서 변동성을 정확히 예측하는 것의 중요성을 잘 보줌

---
  
 ## 연구 목표
변동성을 예측함으로써 리스크 관리뿐만 아니라 적절한 매매 전략을 사용하여 수익을 낼 수 있는 모델 개발을 목표로 함

---

## 변동성 예측 이유
* 그릭스를 통한 델타중립의 이해 - 내용 추가
* 변동성 중에서도 VKOSPI를 예측하는 이유 - 내용 추가
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

## 피처 선택 🔍 - 내용추가
- 로지스틱 회귀 + 라쏘 방법과 상관계수 + 피처 중요도 방법 비교

---

## 모델링/백테스팅 🤖  - 내용추가
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
- **벤치마크 대비 성과:** 과거


# 🚀 Project1 - Option Day Trading Strategy Using Volatility Prediction Indicators

---

## Team Introduction 
- **Team Name:** "ON"
    - Ubi : on
    - Opti : on
    - Predict : on
    - Switch : on 🎚
- **Team Members:**
  👩‍💼 Seung-hee Lee: Team Leader, Presentation Material Production, Modeling
  👨‍💼 Jeong-yun Han: Curator, Data Collection and Preprocessing, Backtesting
  🕵️‍♂️ Jae-wook Wi: Data Collection and Preprocessing, Backtesting
  🧑‍🔬 Shin-wook Yu: Data Collection, Data Visualization
  👩‍🔬 In-hee Han: Data Preprocessing, Modeling, Secretariat

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

