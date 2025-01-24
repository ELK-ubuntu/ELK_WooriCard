# ELK_WooriCard



## visualize👓


Kibana를 이용해서 ElasticSearch에 추가한 우리카드 데이터를 시각화 해보았다.<br>

## 1. 나이대별 이용자수



<br>

![나이대별이용자수](https://github.com/user-attachments/assets/57ffd3a5-9925-4467-b199-b59371504b04)

## 2. 지역별 교육비



<br>

![image](https://github.com/user-attachments/assets/59c0cd1e-e639-4487-b206-a5cb729115c0)

## 3. 성별별 주방용품



<br>

![image](https://github.com/user-attachments/assets/69130e93-abbf-40ff-a3ae-c8320de494f8)

## 4. 나이대별 총소비량



<br>

![image](https://github.com/user-attachments/assets/bc37a418-520e-4ec6-8ede-7a0e8fc98f6c)



## 5. 분기별 의류


<br>

![image](https://github.com/user-attachments/assets/102390fe-3562-42af-82f5-3c7858367c55)




온라인 커머스 플랫폼인 **'무신사'** 에서는 크롤링을 일부 허용해주는 것을 robots.txt를 통해 확인할 수 있었다. <br>
상품 데이터를 직접 크롤링하는 데 많은 시간이 소요되는 관계로, [해시스크래퍼](https://www.hashscraper.com/)의 무료 크롤링 기능을 활용했다. <br>
또한 테이블 스키마를 구성하기 위해 [Amazon Seller - Order Status Prediction](https://www.kaggle.com/datasets/pranalibose/amazon-seller-order-status-prediction) 데이터셋을 참고했다. <br>
