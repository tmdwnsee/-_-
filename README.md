# 개인프로젝트

## 프로젝트 명: 게임 개발을 위한 STEAM 플랫폼 유저들의 게임 선호도 분석 후 맞춤형 전략 기획

## 목차
### A. 프로젝트 개요
  - 프로젝트명
  - 프로젝트를 들어가며
  - 사용된 개발환경, 패키지
  - 프로젝트의 목표

### B. 작업 계획
  - gantt chart
  - 작업 순서도

### C. 데이터 처리 및 분석
  - phase 1. 데이터 수집/저장
    - 데이터 소스 설명
  - phase 2. 데이터 전처리
    - 스팀 게임 데이터 정제
      - 열 삭제
      - 누락값 처리 (삭제 / 웹크롤링)
      - 정규화
    - 설문조사 데이터 정제
      - 누락값 처리
  - phase 3. 통계학적 분석 및 시각화
    - 한글폰트 설치
    - 스팀데이터
      - Positive / Negative 상위 10개 데이터
      - 변수간 상관관계
      - 통계적 의미 분석
      - 정리 및 결론
    - 설문조사 데이터
      - 플레이 만족도와 특정 열간의 독립성 분석
      - 정리 및 결론

### D. 모델링 및 평가
  - phase 4. 머신러닝
    - 모델 선택
    - 스팀데이터
      - 전처리 / 인코딩
      - 학습
      - 로그스케일
      - 클러스터 결과
    - 설문조사 데이터
      - 전처리 / 인코딩
      - 모델 로드 / 학습
      - 예측
      - 하이퍼파라미터 튜닝
      - 모델 개선
      - 예측결과와 결론

### E. 전략 기획
  - 게임 기획
  - 마케팅 전략 (Funnel)

### F. 마무리
-----------
## 사용된 개발환경, 패키지
- 프로그래밍 언어: Python3
- 데이터 수집: Selenium, BeautifulSoup
- 데이터 전처리: pandas, numpy, matplotlib, seaborn
- 데이터 분석: pandas, numpy, matplotlib, seaborn
- 머신러닝 패키지: sklearn
- 머신러닝 알고리즘: k-mean clustering, XGBoost

## 분석내용:
- 리뷰 점수가 높은 게임 특징
- 게임들의 경향 파악
- 이용자들의 선호 경향 파악
- 어떤 방식으로 판매할 것인지 (구독제, 패키지, DLC, 패치 등)

## 결론:
- 플레이 만족도와 연령은 독립적이지 않다. -> 타겟팅: 게임을 가장 많이 이용하는 10대 ~ 30대
- 특정 장르와 게임 흥행 여부가 관련이 없다. -> 유저 유입에 집중해 장르 선정 -> 유저수가 가장 많은 'Action'으로 채택
- 플레이 만족도와 함께 즐기는 사람 여부가 독립적이지 않다 & 특정 군집에서 게임 내 업적수가 가장 높다. -> 'Single-player', 'Family-Sharing', 'Achievements'로 카테고리 선정
- 최대한 많은 유저 유입을 위한 여러 종류의 언어 지원 -> 언어: 영어, 중국어, 스페인어, 한국어 등
- 유저들이 가격과 OS에 신경을 쓰지 않는 경향, DLC 수량보다는 존재가 중요 -> 가격: 유료 (하이엔드로 제작), OS: Window, DLC 여부: 있음

## 프로젝트 성과 및 배운 점:
- 9만개 이상의 raw data를 가져와 정제, 분석, 머신러닝을 돌려 인기 게임의 요소를 확인할 수 있었다.
- 약 4천명의 설문조사 데이터를 가져와 e스포츠 이용자들이 어떤 점을 좋아하고 원하는 지 볼 수 있었고 플레이 만족도에 어떤 것이 가장 영향을 주는 지 확인할 수 있었다.
- 단순히 대형 개발사/배급사에서 출시한 게임이라 해서 무조건 흥행하는 것이 아니라 여러 요소가 합쳐져서 흥행이 될 수도 있다는 것과 의외로 무료/유료 여부가 흥행과 관련이 없다는 것을 알 수 있었다.

## 향후 개선 사항:
- 긍정적 평가와 개발사/배급사 외에 그래픽, 게임 배경, 캐릭터 등 다른 요소가 통계적인 의미가 있을 수 있는 지 추가 분석 필요
- 이스포츠 플레이 만족도와 연령 / 인지 경로 / 함께 즐기는 사람 여부외에 다른 요소가 관련이 있을 수 있는 지 추가 분석 필요
- 유튜브 시장조사를 통해 인기 게임 유튜버들의 평균 조회수, 구독자 수, 해외 반응 등 세밀한 조사 필요
- 머신러닝 결과의 추가적인 향상 필요

### 기간
2024.10.07 ~ 2025.02.14
