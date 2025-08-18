# pjt-data-analysis
SeSAC LLM DA 프로젝트 1st


# 📊 브라질 이커머스 시장 분석 프로젝트


## 📌 프로젝트 소개
이 프로젝트는 Olist Store의 온라인 소매 데이터를 활용하여 브라질 이커머스 시장의 성장 동력과 개선점을 종합적으로 분석하고, 
비즈니스 성장을 위한 데이터 기반 전략을 제시하는 것을 목표로 합니다. 
특히 고객 리뷰, 배송 성과, 결제 수단 등 다양한 데이터를 교차 분석하여 실제 비즈니스 의사결정에 도움이 되는 인사이트를 도출합니다.

---


## 🛠️ 설치 및 실행 방법

### 1. 저장소 클론
```bash
git clone https://github.com/bse1120/pjt-data-analysis
cd pjt-data-analysis
```

### 2. 가상환경 생성 및 활성화
python -m venv venv
# Windows
venv\Scripts\activate
# Mac/Linux
source venv/bin/activate

### 3. 필요한 패키지 설치
pip install -r requirements.txt

requirements.txt 파일 내용

pandas
matplotlib
seaborn
numpy

### 4. 주피터 노트북 실행
jupyter notebook


## 📂 프로젝트 구조

프로젝트폴더/
│── README.md                # 현재 파일
│── requirements.txt         # 프로젝트에 필요한 라이브러리 목록
│── analysis.ipynb           # 데이터 전처리 및 분석 과정이 담긴 주피터 노트북
│── data/
│   ├── olist_orders_dataset.csv
│   ├── olist_order_reviews_dataset.csv
│   └── olist_order_payments_dataset.csv
│── output/
│   └── (분석 결과 시각화 이미지 파일)
└── venv/                    # 가상환경 (Git에는 업로드 X)


## 📊 데이터 설명

데이터 출처: 브라질 Olist E-commerce Public Dataset on Kaggle

주요 데이터셋:

olist_orders_dataset.csv: 주문 정보 (주문 상태, 구매/배송 시간)

olist_order_reviews_dataset.csv: 고객 리뷰 정보 (점수, 메시지)

olist_customers_dataset.csv: 고객 정보 (고유 ID, 지역)

olist_order_payments_dataset.csv: 결제 정보 (결제 수단, 금액)

olist_products_dataset.csv: 상품 정보 (카테고리, 무게, 크기 등)

데이터 크기: 다양한 데이터셋으로 구성되며, 수십만 건의 주문 및 고객 정보 포함.


## 🔎 분석 목표 및 주요 결과

1. 고객 세분화 및 RFM 분석
목표: 고객을 RFM(Recency, Frequency, Monetary) 지표를 기반으로 세분화하고, 각 그룹의 특성을 파악하여 맞춤형 마케팅 전략을 수립합니다.

결과: Best Customers, Loyal Customers, New & Active Customers 등 6개 고객 세그먼트를 정의했으며, 특히 상파울루(SP)와 리우데자네이루(RJ)에 고액을 자주 지출하는 최우수 고객층이 집중되어 있음을 확인했습니다.

2. 배송 성과 분석 및 물류 최적화
목표: 주문부터 배송까지의 시간을 분석하고, 배송 지연이 고객 만족도에 미치는 영향을 파악하여 물류 개선 방안을 제시합니다.

결과: 배송 지연이 고객 만족도(리뷰 점수)를 현저히 떨어뜨리는 것을 확인했으며, 배송 시간이 긴 지역을 식별하여 해당 지역의 물류 프로세스를 최적화하는 전략을 제안했습니다.

3. 상품 카테고리별 수요 예측 및 재고 관리
목표: 시간에 따른 상품 판매 트렌드와 계절성 패턴을 분석하여 수요를 예측하고 효율적인 재고 관리 전략을 수립합니다.

결과: 대부분의 상품 카테고리가 11월 블랙 프라이데이에 판매량이 급증하는 뚜렷한 계절성을 보였습니다. 이를 기반으로 bed_bath_table, health_beauty, computers_accessories와 같은 핵심 카테고리에 대한 성수기 재고 확보 전략을 수립했습니다.

4. 종합 분석 및 비즈니스 성장 전략
목표: 위 분석 결과들을 통합하여 브라질 이커머스 시장의 성장 동력과 개선점을 종합적으로 분석하고, 비즈니스 성장을 위한 데이터 기반 전략을 제시합니다.

결과: 신용카드 중심의 신뢰성 높은 결제 환경과 강력한 계절성 수요가 주요 성장 동력입니다. 이를 극대화하기 위해 RFM 기반 마케팅, 계절성 수요에 맞춘 재고 관리, 배송 지연을 줄이는 물류 개선 등 다각적인 데이터 기반 전략을 제안했습니다.