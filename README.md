### 쇼핑몰 웹 로그 분석 프로젝트
![image](https://github.com/wbin0718/shoppingmall_weblog/assets/104637982/efa7a09d-a4b1-47d9-ab63-94a38afe3632)

### 분석 데이터
* 6000만개 이상의 행을 가지는 데이터
* 사용자아이디, 사용자 세션, 이벤트 타입, 시간등의 컬럼 포함
* [캐글 데이터](https://www.kaggle.com/datasets/mkechinov/ecommerce-behavior-data-from-multi-category-store)

### 분석 이유
* 빅쿼리를 통해 원하는 데이터 추출 능력 성장
* event 기반 funnel 분석 진행

### 분석 환경

데이터의 행 개수가 6000만개가 넘어 일반적인 RDBMS로는 빠른 분석 진행을 할 수 없었습니다.  
실제로 mysql을 사용하려고 시도하였으나 데이터 업로드가 되지 않고 튕기는 현상이 일어났습니다. 따라서 데이터를 GCS로 저장하고, 빅쿼리 및 파이썬을 사용했습니다.
