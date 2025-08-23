# 📜 이준희 포트폴리오 (Updating...)

Name : 이준희 (JunHee Lee) 

Date of Birth : 1995.02.27

--- 
## 📞 Contact
Mail : junheelee95@gmail.com

--- 
## 🎓 학력
- 한양대학교(서울) 비즈니스 인포매틱스학과 석사 졸업 (2023.02)

    → 석사학위논문 : 베이지안 딥러닝을 활용한 항만물동량 예측에 관한 연구 [논문 요약 및 핵심코드 저장소 바로가기](https://github.com/iureifjdkncd/2022-MS_Thesis)

- 세종대학교 경영학과 / 비즈니스 애널리틱스학과 학사 졸업 (2021.02)

--- 

## 📄 자격 및 교육사항

| 자격 & 교육증명                       | 발급기관                    | 취득일       | 비고                                         |
| ---------------------------- | ------------------------- | ---------- | ------------------------------------------ |
| TOEIC (970점)                | ETS                       | 2019.06.30 | LC 490 / RC 480, (만료: 2021.06.30) |
| OPIc (Advanced Low)          | ACTFL (YBM)              | 2019.08.11 | 영어 말하기 시험, (만료: 2021.08.10)      |
| ADsP (데이터분석 준전문가)     | 한국데이터산업진흥원           | 2020.09.29 | 데이터 분석 국가공인 자격증, 자격번호: ADsP-0261663 |
| 파이썬 프로그래밍 활용능력 1급    | 한국정보인재개발원             | 2020.08.11 | 자격번호: 2007-141-00325                      |
| Microsoft AI School 수료증 | 한국마이크로소프트 / 비알프레임 | 2020.01.31 | 기초 AI 교육 프로그램 수료                     |

---

### 📌 관심 분야
- 시계열 예측 
- 이상치 탐지
- 프로세스 최적화 및 추천

--- 
## 📌 Career
InterX (2023.03 ~ Present)

Position: Data Scientist / SDF R&D

주요 업무 : Time Series Forecasting, Anomaly Detection 

※ 이미지 기반 분석(CV), LLM분석은 직접 수행 경험 없음

### ⭐️ Skills
| 기술           | 실무 활용                                                                              | 내용 정리                                                    | 역량  |
| ------------ | ------------------------------------------------------------------------------------- | -------------------------------------------------------- | ---- |
| **Python**   | `pandas`, `numpy`로 데이터 분석 및 전처리 수행,<br>`scikit-learn`, `TensorFlow` 사용한 AI 모델 개발 및 실험 | 전체 파이프라인 경험 보유 (전처리~학습),<br>다만 PyTorch, OpenCV는 미경험            | 중\~상 |
| **FastAPI**  | 학습된 AI모델 `REST API`로 배포하여 시스템 구현 지원,<br>`.bat` 스크립트를 통한 `Uvicorn` 서버 자동 실행 환경 구성                                        | API 기반 시스템 구축 경험 보유,<br>개발팀 주도의 서비스 통합·배포 과정에서 협업 중심으로 참여             | 중    |
| **Docker**   | `Docker`를 활용한 환경 구성 스크립트 작성                              | 환경 구축은 개발팀이 주도,<br>API 운영·배포, 환경 테스트에 협업 중심으로 참여                 | 중    |
| **Database** | `MongoDB`,`PostgreSQL`에서 조건 필터링,정렬,`limit` 쿼리 등 수행,<br>Python 기반 조회 및 가공 경험                   | NoSQL(MongoDB)&RDB(PostgreSQL) 구조 이해,<br>설계,운영 경험은 없음 | 중    |
| **Git**      | GitLab에 업로드 및 commit/pull/push,<br>`master` 브랜치 관리 경험                                            | Git 기본 명령 및 협업 경험 보유,<br>전략적 브랜치 운영 경험 부족           | 중\~하    |

### 📌 AI 프로젝트 프로세스 담당 구분

| 단계 | 프로세스 | 주요 담당 |
|------|----------|-----------|
| 1 | Raw Data 수집·정제 | 개발팀 / 데이터 엔지니어 |
| 2 | DB 조회 | **본인 주도** |
| 3 | 학습용 데이터 전처리 | **본인 주도** |
| 4 | AI 모델 구축 | **본인 주도** |
| 5 | Docker/FastAPI 구축 | **본인 주도 + 개발팀 협업** |
| 6 | 서비스 통합·배포·활성화 | 개발팀 주도 + 협업 |
| 7 | 시스템 모니터링 | **본인 주도 + 개발팀 협업** |

```mermaid
flowchart LR
    A[Raw Data 수집·정제]:::dev
    B[DB 조회]:::me
    C[학습용 데이터 전처리]:::me
    D[AI 모델 구축]:::me
    E[Docker/FastAPI 구축]:::me
    F[서비스 통합·배포·활성화]:::meco
    G[시스템 모니터링]:::me
    A --> B --> C --> D --> E --> F --> G
    classDef me fill:#fef3c7,stroke:#f59e0b,stroke-width:2px;
    classDef dev fill:#dbeafe,stroke:#3b82f6,stroke-width:2px;
    classDef devco fill:#e0f2fe,stroke:#0284c7,stroke-width:2px;
    classDef meco fill:#ecfdf5,stroke:#10b981,stroke-width:2px;
```
---

### 📝 Project Experience [Archive](https://github.com/iureifjdkncd/B2B_AI_Projects/tree/main)

#### 1. 비지도학습 기반 사출 품질 예측 및 최적 세팅 추천 (2023.08 ~ 2025.07)

- 문제: 라벨링 부족·세팅 변동성으로 불량 탐지 어려움

- 접근: **K-Means** 기반 조건 분리, **IsolationForest/AutoEncoder** 활용, 유사 조건 기반 추론 및 통계 가중 임계값 적용

- 성과: 불량 탐지 정확도 약 **+16%**, 생산 불량률 약 **-5%**

- [프로젝트 상세 설명](https://github.com/iureifjdkncd/B2B_AI_Projects/tree/main/Project_A)

---

#### 2. 확률적 시계열 예측 기반 제당공정 품질 추론·조건 최적화 (2024.05 ~ 2025.03)

- 문제: 다변량 품질 예측 및 신규 조건 생성 불가 → 과거 조건 기반 추천 필요

- 접근: **Quantile ML Regression** + **MC Dropout-BiLSTM** 기반 확률적 예측, 과거 유사 조건 검색 및 다수 추적 경로 적용

- 성과: 예측 정확도 **87~91%**, 추천 조건 일치율 **85~90%**, 생산 품질 **+1%**

- [프로젝트 상세 설명](https://github.com/iureifjdkncd/B2B_AI_Projects/tree/main/Project_B)

---

#### 3.) 사출 설비 품질 예측·조건 추천 통합 시스템 (2023.05 ~ 2025.03)

- 문제: 라벨링 제약과 실시간 조건 추천 필요

- 접근: **AutoEncoder** + 통계 기반 적응형 추론, **K-Means** + 확률 샘플링 통한 조건 추천

- 성과: 불량 탐지 정확도 약 **+14%**, 조건 추천 오차 범위 **±3~5%**

- [프로젝트 상세 설명](https://github.com/iureifjdkncd/B2B_AI_Projects/tree/main/Project_C)

---

#### 4.) 사출 설비 불량 예측모델 개발 (TTA 인증) (2023.08 ~ 2023.09)

- 문제: 사출공정 불량탐지 모델 개발 및 TTA 인증 요구 대응

- 접근: **TreeML** 기반 모델링, 불균형 샘플링 + 교차검증

- 성과: F1 **95%** 이상, TTA 인증 확보

- [프로젝트 상세 설명](https://github.com/iureifjdkncd/B2B_AI_Projects/tree/main/Project_D)

---

#### 5.) Cogging Motor 조립·병렬 공정 불량 탐지 PoC (2024.07 ~ 2024.08)

- 문제: 모터 제조 품질 예측 AI 도입을 위한 PoC 수행

- 접근: **TreeML** + 불균형 샘플링, 공정별 임계값 설정

- 성과: F1 **75~91%**, AI 적용 가능성 검증

- [프로젝트 상세 설명](https://github.com/iureifjdkncd/B2B_AI_Projects/tree/main/Project_E)

---
#### 6.) 고속사출기 불량탐지 PoC (2023.11 ~ 2023.12)

- 문제: 고속사출기 생산 과정에서의 Raw Data 표준화 및 AI 도입을 위한 PoC 수행

- 접근: Raw Data 표준화, Optuna 기반 **TreeML** 모델

- 성과: F1 **+12%** , AI 도입 타당성 확보

- [프로젝트 상세 설명](https://github.com/iureifjdkncd/B2B_AI_Projects/tree/main/Project_F)

---

### 📝 Research Experience
[Archive](https://github.com/iureifjdkncd/Research)

#### 1.) Recipe Based Anomaly Detection with Adaptable Learning: Implications on Sustainable Smart Manufacturing(2025)

- 주제: 공정 세팅 변동 반영 및 새로운 세팅 생산에 강건한 추론 기법 연구
  
- 접근: **AutoEncoder** 분리학습 + 유사도 기반 추론

- 성과: 불량 탐지 정확도 **+30~50%**, **SCI급 논문(MDPI Sensors) 제1저자 게재**

- [Paper Link](https://doi.org/10.3390/s25051457)
   
---

#### 2.) Forecast-Aware Conditional Process Optimization: A Two-Stage Deep Learning Framework (2025)

- 주제: 목표값 기반 최적 다변량 시계열 공정 프로세스 생성 및 예측성능 기반 검증
  
- 접근: 예측·생성 모듈 융합, 조건부 시계열 생성 알고리즘 개발

- 문제: 품질 예측 정확도 **+20%** 이상, **SCI급 논문(MDPI Sensors) 제1저자 투고**

---


## 🏆 Contest 

#### 1.) 제10회 산업통상자원부 공공데이터 활용 BI 공모전  최우수상 (KOTRA 사장상 수상)

- 과제명 : 한국 수출금액 예측 모델 기반 기업수요 맞춤형 서비스
  
- 접근: 확률적 예측기반 통계 + DL기반 다변량 시계열 상호보완 

- 성과 : VECM(**정확도 97.1%**)& Monte Carlo Dropout Seq2Seq 병행, 품목수요 예측서비스에서 정확도, 불확실성 해석력, 비즈니스 활용 가능성 제안

- [공모전 정리](https://github.com/iureifjdkncd/2022_KOTRA_BI)

- [수상내역](https://datacontest.kr/board/view/97533073/3694)

- [학회 논문 링크](https://www.dbpia.co.kr/Journal/articleDetail?nodeId=NODE11207563)

---
