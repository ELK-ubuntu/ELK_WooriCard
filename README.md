# ELK_WooriCard


## 프로젝트 소개


- 우리카드로부터 제공받은 실제 사용자 데이터를 활용해 ELK를 기반으로 데이터 시각화 및 분석, 나아가 새로운 고객유치 및 이용량 증가를 위한 방안을 제시한다.
- Virtual Box 내에 Ubuntu 상에 설치한 ELK 내부에 카드 데이터 csv를 삽입해 새로운 Index를 생성하고 이를 활용한다.


## 사용 환경


## 데이터 시각화


### < 생애 주기별 체크/신용카드 사용 금액 현황 >
![LifeStage별](life_stage.png)

- 체크카드 최대 이용 고객군 : 대학생(UNI)
- 신용카드 최대 이용 고객군 : 의무교육 연령대 자녀를 둔 부모(CHILD_TEEN)

✅ 체크카드는 주로 소득이 제한적인 대학생 고객군에서 최대 이용량을 보이며, 이는 사회 초년생의 소비 성향을 반영한다.
<br>
✅ 신용카드는 자녀 교육비와 생활비 등 고정 지출을 관리하려는 초중고 자녀를 둔 부모 고객군에서 가장 많이 사용된다.

<br>

### < 거주 지역별 자동차 정비 및 유지 비용 - 분기별 >
![거주지역별](loc_car.png)

- 자동차 정비 및 유지 비용이 높은 고객 지역 : 전남, 전북
- 자동차 정비 및 유지 비용이 낮은 고객 지역 : 서울, 경기

✅ 전라남도와 전라북도는 상대적으로 교통 인프라가 부족하거나 차량 이동거리가 길어 정비와 유지가 자주 필요할 수 있다고 분석된다.
<br>
✅ 서울과 경기 지역은 교통 인프라가 잘 발달하고, 이동거리가 상대적으로 짧아 자동차 유지비용이 낮게 나타나는 경향을 보인다.

<br>

### 분기별 의류
<br>
![image](https://github.com/user-attachments/assets/102390fe-3562-42af-82f5-3c7858367c55)

### 나이대별 총소비량
<br>
![image](https://github.com/user-attachments/assets/bc37a418-520e-4ec6-8ede-7a0e8fc98f6c)

### 성별별 주방용품
<br>
![image](https://github.com/user-attachments/assets/69130e93-abbf-40ff-a3ae-c8320de494f8)

### 지역별 교육비
<br>
![image](https://github.com/user-attachments/assets/59c0cd1e-e639-4487-b206-a5cb729115c0)

### 나이대별 이용자수
<br>
![image](https://github.com/user-attachments/assets/57ffd3a5-9925-4467-b199-b59371504b04)



## 데이터에 대한 팀원들의 견해


팀원들의 공통된 예측과 다른 결과가 시각화를 통해 확인되었다. 


#### 1. 사람들은 2Q에 의류 소비를 가장 많이 할까?


겨울옷의 가격대가 더 높기때문에 당연히 4분기에 평균 옷 소비금액이 높을것이라는 예상과는 달리


#### 2. 평균 교육비가 가장 높은 지역은 제주도에 거주하는 사람들?

![image](https://github.com/user-attachments/assets/59c0cd1e-e639-4487-b206-a5cb729115c0)

#### 3. VVIP들의 총 소비 금액은 왜 적을까?




## 데이터를 통한 우리카드 사용자 예측하기
우리카드의 카드 중 **카드의 정석 포인트**는 우리카드의 새로운 유입을 이끌어가는 대표적인 카드다.


- 카드의 정석 포인트 혜택


![alt text](image.png)
출처: 카드 고릴라
<br>

- 사용자들의 1년 소비 금액 예측
<br>

기존 카드의 정석 point 혜택

![alt text](image-3.png)




## 우리카드 전략 제시

새로운 카드의 정석 point 혜택

![alt text](image-1.png)
![alt text](image-2.png)
