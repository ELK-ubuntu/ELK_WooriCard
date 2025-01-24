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
우리카드의 카드 중 **카드의 정석 포인트**는 우리카드의 새로운 회원 유입을 이끌어가는 대표적인 카드다.


- 카드의 정석 포인트 혜택


<br>

기존 카드의 정석 point 혜택


![alt text](image.png)
출처: 카드 고릴라


![alt text](image-3.png)


카드의 정석 포인트를 삼성페이에 등록 후 결제 시 추가 3% 적립 혜택을 통해 총 3.8%의 적립이 가능해진다.



한달 최대 적립 금액인 5만점을 채우기 위해서는 130만원을 사용하면 된다.


1년 사용 금액 : **130만원 X 12달 = 1600만원** 이라 계산할 수 있다.


이는 1000만원 이상 2500만 미만의 소비를 하는 Gold 등급에 해당한다.


서브 카드로 카드의 정석 포인트를 사용하면서 혜택을 모두 채우기 위해 사용하는 사용자들이 많을 것이라 생각했으며 이로 인해 Gold에 속한 사용자가 다수일 것이라 생각했다.


실제 주어진 csv 파일을 시각화 했을 때 Gold 등급이 총 소비 금액 7000억으로 가장 많이 분포하고 있음을 확인할 수 있다. 


그 다음 많이 분포하는 등급인 Platinum의 경우도 카드의 정석 포인트의 최대 적립을 채우고도 조금 더 사용하는 사용자일 것이라 예상되었다.


보통 카드의 정석 포인트 카드는 사용자들의 주 이용 카드로 사용되지 않으며 일명 서브 카드에 속한다.


이는 신한 카드의 더모아와 같은 적립 혜택이 더 좋은 카드가 존재하고 있기 때문이다. 


## 우리카드 전략 제시

새로운 카드의 정석 point 혜택

![alt text](image-1.png)
![alt text](image-2.png)
<<<<<<< HEAD
=======


이제는 카드의 정석 포인트의 혜택이 줄어든 것을 확인할 수 있다. 


적립율이 줄어들었으며 특히 적립 한도가 최대 2만 포인트로 절반 이상 줄어들게 되었다. 


![alt text](image-5.png)


카드 가맹점 수수료율은 시간이 지남에 따라 지속적으로 줄어들게 되었으며 이로 인해 카드 사용율을 증가시키는 전략을 통해 카드사 수익 극대화 전략은 어려움을 겪게 되었다.


특히 적립 혜택만을 채우고 사용하지 않는 사람들이 존재한다면 3.8%의 페이백을 이루어지며 카드 수수료를 통해 우리카드 가맹점인 최대 수수료인 3%를 거두어들인다 가정해도 0.8%의 손해가 발생하는 것이다.


그러나 가맹점의 높은 비율은 우대 수수료율을 적용받으며 연매출 30억 이하 중소 사업체의 경우 최대 1.5%의 수수료만 지불하면 된다.


이로 인해 3.8%의 페이백 혜택을 주는 것은 사실상 더 큰 손실을 불러일으킬 것이다.


#### 1. 수익성 전략


데이터를 통해 분석을 하면서 처음 생각했던 전략 중 하나는 vvip의 소비를 늘릴 수 있는 유도책을 마련하는 것이었다.


그러나 우리카드의 vvip의 기준은 1년간 1억 이상 소비를 한 사용자다.


이는 다른 카드사들에 비해 더 낮은 기준치를 보여준다.


![alt text](image-6.png)


하나 카드의 vip 선정 기준을 보면 비교적 높은 기준치를 확인할 수 있다.


만약 3000명만 VVIP로 선정한다면 우리카드의 vvip의 소비 금액에 대입했을 때 2년간 700억을 소비하게 되므로 1년간 350억, 1인당 연간 천만원의 소비를 한다는 결과가 나온다.


 따라서 우리카드의 vvip는 3000명보다 훨씬 못미친다 예상했다.


 이로 인해 타켓으로 해야하는 소비층은 Gold ~ Platinum이 되어야 한다 생각했다.


카드사의 주 매출은 카드 단기 대출이 주력화 된지 오래다. 


카드 단기 대출 서비스의 금리 우대 혜택을 Gold ~ Platinum에 존재하는 회원을 대상으로 

#### 2. 우리카드를 메인 카드로!


데이터를 분석하면서 예상과 다른 결과가 나온 이유는 우리카드를 '주카드'로 사용하는 사람의 수가 적기 때문이라 생각했다. 


해외 결제
>>>>>>> Ryan
