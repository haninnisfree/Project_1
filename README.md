# 변동성 예측 지표를 활용한 옵션 데이트레이딩 전략 수립

교수님은 이 발표의 PPT를 참고하여 평가할 것입니다.

## 📑 목차
- [프로젝트 개요](#프로젝트-개요)
- [연구 주제 및 배경](#연구-주제-및-배경)
- [워크플로우](#워크플로우)
- [데이터셋(EDA)](#데이터셋eda)
- [피처 선택](#피처-선택)
- [모델링 및 트레이딩 전략](#모델링-및-트레이딩-전략)
- [결과 및 결론](#결과-및-결론)

---

## 프로젝트 개요
- **팀 이름:** "ON"
  - **팀원 소개:**
    - 이승희: 팀장, 발표자료제작, 모델링
    - 한정윤: 큐레이터, 데이터 수집 및 전처리, 백테스팅
    - 위재욱: 데이터 수집 및 전처리, 백테스팅
    - 유신욱: 데이터 수집, 데이터 시각화
    - 한인희: 데이터 전처리, 모델링, 서기

---

## 연구 주제 및 배경

### 옵션에 대한 관심도 증가
- **현상:** 최근 옵션 거래에 대한 관심이 높아지고 있으며, 이는 거래량 증가와 함께 기사 및 보도 자료를 통해 확인할 수 있습니다.
- **의의:** 이러한 추세는 옵션 시장의 잠재적 성장 가능성을 나타내며, 투자자와 연구자 모두에게 새로운 기회를 제시합니다.

### 옵션 트레이딩의 변질 문제
- **문제점:** 옵션 트레이딩이 본래의 목적인 선물 시장의 헷지 도구로서의 역할에서 벗어나, 단기 수익 추구 수단으로 변질되고 있다는 지적이 있습니다.
- **연구 필요성:** 이러한 변질을 이해하고 올바른 옵션 트레이딩 전략을 수립하기 위한 연구가 필요합니다.

### 옵션 트레이딩의 위험성
- **사례:** 베어링스 은행의 파산 사례와 같이 옵션 트레이딩은 높은 수익률을 제공할 수 있지만, 그에 따른 위험도 역시 높습니다.
- **연구 목적:** 이러한 위험성을 줄이면서도 수익성을 추구할 수 있는 전략을 개발하기 위해 옵션 트레이딩에 대한 심도 있는 연구가 필요합니다.

### 베어링스 은행 파산의 교훈
- **배경:** 베어링스 은행의 파산에는 여러 원인이 있었으나, 결정적인 원인은 양매도 전략 사용 중 변동성이 급격히 커졌을 때 이를 적절히 예측하지 못했기 때문입니다.
- **중요성:** 이 사례는 옵션 트레이딩에서 변동성을 정확히 예측하는 것이 얼마나 중요한지를 잘 보여줍니다.
- **연구 목표:** 우리는 베어링스 은행의 사례를 바탕으로 변동성이 큰 날을 예측하고, 그런 날에도 수익을 낼 수 있는 모델을 개발하는 것을 목표로 합니다.

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

## 데이터셋(EDA)
- **기간:** 6월 12일부터 11월 3일까지
  - **train data:** 6월 12일 ~ 10월 6일
  - **test data:** 10월 10일 ~ 11월 3일
- **데이터 분류:** 트레이닝 데이터셋과 테스트 데이터셋
- **데이터 분포 및 이상치 탐색:** describe를 통해 데이터의 분포를 대략적으로 확인, 이상치는 유의미함

---

## 피처 선택
- 로지스틱 회귀 + 라쏘 방법과 상관계수 + 피처 중요도 비교

---

## 모델링 및 트레이딩 전략
- 변동성 예측 실패의 위험성 분석
- 트레이딩 전략의 백테스팅 결과
- 라벨링 변경의 이유와 방법
- 양매수, 양매도, 머신러닝 기반 전략 비교

---

## 결과 및 결론
- **베어링스 은행 사례:** 결정적인 파산 원인 분석
- **변동성 예측 모델:** 변동성이 큰 날을 예측하는 모델 개발의 중요성
- **전략 수립:** 위험성을 줄이고 수익을 극대화하는 전략 제안
- **백테스팅 결과:** 이론상 양매도 스트랭글 및 양매수 스트래들 전략의 안정성 분석
- **벤치마크 대비 성과:** 과거 데이터 기반의 매매 전략 수익율과 벤치마크 이긴 결과 비교
