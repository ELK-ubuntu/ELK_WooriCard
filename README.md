# ELK_WooriCard


## 프로젝트 소개


- ㅇㅇ카드의 실제 사용자 데이터를 활용해 ELK를 기반으로 데이터 시각화 및 분석, 나아가 새로운 고객유치 및 이용량 증가를 위한 방안을 제시한다.
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

### < 분기별 의류 >
<br>

![alt text](IMG2.png)

- 의류가 가장 많이 소비된 분기 : 2분기

### < 나이대별 총소비량 >
<br>

![alt text](IMG_4.png)

- 총소비량이 가장 많은 나이대 : 40세
- 총소비량이 가장 적은 나이대 : 85세

✅ 가장 소득이 많은 나이대인 40대, 그중 45세가 총 소비량이 높은 경향을 보인다.
<br>
✅ 은퇴후 일정 수입이 끊긴 나이대인 80대, 그중 85세가 총 소비량이 낮은 경향을 보인다. 


### < 성별별 주방용품 >
<br>

![alt text](IMG3-1.PNG)

- 주방용품 소비가 가장 큰 성별과 나이 : 여성, 55세
- 주방용품 소비가 가장 낮은 성별과 나이 : 남성, 45세

✅ 가사 일을 가장 많이 하는 여성, 그중 55세가 주방용품에 가장 소비를 많이 하는 것으로 나타났다.
✅ 또한 나이가 많아질수록 소득 감소와 신체 노화로 인해 가사 노동의 절대적인 양이 감소하면서 소비량도 자연스럽게 줄어드는것으로 나타났다.

<br>
✅ 가사 업무의 비중이 낮은 남성은 45세에 가장 적은 소비를 하는것으로 나타났다.
✅ 나이가 많아질수록 직장 은퇴로 인해 가사업무의 비중이 늘어 주방용품 소비비용의 비중이 늘어나는 것으로 예상할 수 있다.
<br>
✅ 가사 일을 가장 많이 하는 여성, 그중 55세가 주방용품에 가장 소비를 많이 하는 것으로 나타났다.

### < 지역별 교육비 >
<br>

![image](https://github.com/user-attachments/assets/59c0cd1e-e639-4487-b206-a5cb729115c0)

- 평균 교육비가 가장 높게 나타나는 지역 : 제주, 세종



## 데이터에 대한 팀원들의 견해


팀원들의 공통된 예측과 다른 결과가 시각화를 통해 확인되었다. 


#### 1. 사람들은 2Q에 의류 소비를 가장 많이 할까?

겨울옷의 가격대가 더 높기때문에 당연히 4분기에 평균 옷 소비금액이 높을것이라는 예상과는 달리 데이터는 **2분기**에 가장 높은것으로 확인되었다. 일반적으로 생각해보았을때 겨울철 외투 비용과 여름철 옷 비용은 크게 차이가 나기 때문에 우리카드 데이터의 신뢰도 확인이 필요하다는 결론이 났다.


#### 2. 평균 교육비가 가장 높은 지역은 제주도에 거주하는 사람들?

서울이나 경기지역으로 갈수록 교육비가 가장 높을 것이라 예상했던 바와 달리 세종, 제주지역에 평균 교육비가 가장 높은것으로 확인되었다.

![alt text](교육비_기사.jpg)

[출처] : https://www.nextplay.kr/news/articleView.html?idxno=7261

뉴스기사와 실데이터의 분석내용이 일치하지 않는것으로 보아 실데이터의 신뢰도와 객관성 확인이 필요하다는 결론이 났다.


#### 3. VVIP들의 총 소비 금액은 왜 적을까?




## 데이터를 통한 ㅇㅇ카드 사용자 예측하기
ㅇㅇ카드의 카드 중 **🐝 포인트 카드**는 ㅇㅇ카드의 새로운 회원 유입을 이끌어가는 대표적인 카드다.


-  🐝 포인트 카드 혜택


<br>

기존 🐝 포인트 카드 혜택


![alt text](image.png)
출처: 카드 고릴라


![alt text](image-3.png)


🐝 포인트 카드를 삼성페이에 등록 후 결제 시 추가 3% 적립 혜택을 통해 총 3.8%의 적립이 가능해진다.



한달 최대 적립 금액인 5만점을 채우기 위해서는 130만원을 사용하면 된다.


1년 사용 금액 : **130만원 X 12달 = 1600만원** 이라 계산할 수 있다.


이는 1000만원 이상 2500만 미만의 소비를 하는 24 등급에 해당한다.


서브 카드로 🐝 포인트 카드를 사용하면서 혜택을 모두 채우기 위해 사용하는 사용자들이 많을 것이라 생각했으며 이로 인해 24 등급에 속한 사용자가 다수일 것이라 생각했다.


실제 주어진 csv 파일을 시각화 했을 때 24 등급이 총 소비 금액 7000억으로 가장 많이 분포하고 있음을 확인할 수 있다. 


그 다음 많이 분포하는 등급인 23의 경우도 🐝 포인트 카드의 최대 적립을 채우고도 조금 더 사용하는 사용자일 것이라 예상되었다.


보통 🐝 포인트 카드는 사용자들의 주 이용 카드로 사용되지 않으며 일명 서브 카드에 속한다.


이는 ㅅㅅ 카드의 더모아와 같은 적립 혜택이 더 좋은 카드가 존재하고 있기 때문이다. 


## ㅇㅇ카드 전략 제시

새로운 🐝 포인트 카드 혜택

![alt text](image-1.png)
![alt text](image-2.png)


이제는 🐝 포인트 카드의 혜택이 줄어든 것을 확인할 수 있다. 


적립율이 줄어들었으며 특히 적립 한도가 최대 2만 포인트로 절반 이상 줄어들게 되었다. 


![alt text](image-5.png)


카드 가맹점 수수료율은 시간이 지남에 따라 지속적으로 줄어들게 되었으며 이로 인해 카드 사용율을 증가시키는 전략을 통해 카드사 수익 극대화 전략은 어려움을 겪게 되었다.


특히 적립 혜택만을 채우고 사용하지 않는 사람들이 존재한다면 3.8%의 페이백을 이루어지며 카드 수수료를 통해 우리카드 가맹점인 최대 수수료인 3%를 거두어들인다 가정해도 0.8%의 손해가 발생하는 것이다.


그러나 가맹점의 높은 비율은 우대 수수료율을 적용받으며 연매출 30억 이하 중소 사업체의 경우 최대 1.5%의 수수료만 지불하면 된다.


이로 인해 3.8%의 페이백 혜택을 주는 것은 사실상 더 큰 손실을 불러일으킬 것이다.


#### 1. 수익성 전략


데이터를 통해 분석을 하면서 처음 생각했던 전략 중 하나는 vvip의 소비를 늘릴 수 있는 유도책을 마련하는 것이었다.


그러나 ㅇㅇ카드의 vvip의 기준은 1년간 1억 이상 소비를 한 사용자다.


이는 다른 카드사들에 비해 더 낮은 기준치를 보여준다.


![alt text](image-6.png)


ㅁㅁ 카드의 vip 선정 기준을 보면 비교적 높은 기준치를 확인할 수 있다.


만약 3000명만 VVIP로 선정한다면 ㅇㅇ카드의 vvip의 소비 금액에 대입했을 때 2년간 700억을 소비하게 되므로 1년간 350억, 1인당 연간 천만원의 소비를 한다는 결과가 나온다.


 따라서 ㅇㅇ카드의 vvip는 3000명보다 훨씬 못미친다 예상했다.


 이로 인해 타켓으로 해야하는 소비층은 23 ~ 24가 되어야 한다 생각했다.


카드사의 주 매출은 카드 단기 대출이 주력화 된지 오래다. 


카드 단기 대출 서비스의 금리 우대 혜택을 23 ~ 24에 존재하는 회원을 대상으로 

#### 2. ㅇㅇ카드를 메인 카드로!


데이터를 분석하면서 예상과 다른 결과가 나온 이유는 ㅇㅇ카드를 '주카드'로 사용하는 사람의 수가 적기 때문이라 생각했다. 


해외 결제
