
 # 📋 고혈압 환자의 본인부담금에 대한 변수의 영향 분석
 <STRONG> Join_Collection_BND_M20 
- 고혈압 환자 대상 분석(설명 변수 5개 이상)
- 상병 코드 SICK_SYM1 = I10 (고혈압)
- 목표 변수 : 심결본인부담금 (EDC_SBA)
- 설명 변수 : 수술여부(OPRTN_YN), 입내원일수 (VSHSP_DD_CNT), 생년월일 (BTH_YYYY), 진료결과구분(MCARE_RSLT_TYPE), 요양일수(MDCARE_DD_CNT), 심결가산율(EDC_ADD_RT)

 ### 📌분석 목적
-  고혈압은 전 세계 수백만 명의 개인에게 영향을 미치는 광범위한 만성 질환입니다. 최근에는 의료비가 지속적으로 증가함에 따라 고혈압 환자의 본인부담금에 영향을 미치는 요인을 이해하는 것이 무엇보다 중요합니다. 본 분석은 고혈압 관리와 관련된 결정을 내릴 때 다양한 변수가 환자의 본인부담금에 미치는 영향을 종합적으로 분석하는 것을 목표로 합니다. 

-  목표변수로 잡은 심결본인부담금은 의료비 중 보험사가 보험금 청구를 검토, 처리한 후 수험자(환자)가 부담하는 부분을 나타냅니다

### 🙋🏻‍♀️ 분석가 : 조효원
 
### DDA 
    - 선택한 변수 중 분석을 맡은 컬럼을 추출 및 컬럼 별 데이터 타입과 확인
    - 연속형(int)에서 범주형(object)으로 변경하는 작업을 진행.
<details>  
<summary>변수 선택 이유 </summary>
    
| 변수 | 변수값 설명 | 유형 | 선택 이유 |
|--- | --- | --- | ---- |
| 심결본인부담금 (EDC_SBA) | 검토 결정 이후 수행자가 부담해야 할 금액 | 연속형 | 금전적 측면이 중요하므로 본인 부담 비용을 목표 변수로 선택했습니다. |
| 수술 여부 (OPRTN_YN) | 0: 미수술, 9: 수술 | 범주형 | 수술비용이 많이 들기 때문에 수술여부를 변수로  선택했습니다. |
| 입내원일수 (VSHSP_DD_CNT) | 환자의 총 치료 일수 (투약 일 포함),  ※ 입원의 경우 입원 중 투약 일수를 포함, 0일 경우: 협진 | 연속형 | 치료기간이 길 수록 비용이 증가할 것으로 예상되어 입내원일수를 변수로 선택했습니다. |
| 생년월일 (BTH_YYYY) | | 연속형 | 연령에 따라 회복속도와 건강상태가 드리기 때문에 심결본인부담금과 연관이 있을거라고 예상되어 변수로 선택했습니다. |
</details>
 
### EDA
    
    - 범주형/연속형에 따라서 그래프를 통해 시각화를하여 목표변수에 영향 여부를 예측해 봄.

### CDA 
    
    - 목표변수와 설명변수의 관계를 검증하여 p-value값을 통해 수치적으로 영향 여부를 판단함.

### 시각화
<수술여부>

<img src="images\.ipynb_checkpoints\수술여부-checkpoint.png" width="200"> 

### 분석스토리 

| 변수명 |  pvalue | 성립가설   
| --- |--- |--- |
|OPRTN_YN(수술여부)| 0.0027124705352598944  | 대립가설 참 : 본인부담금이 수술여부와 차이가 있다
|생년월일(BTH_YYYY)| 0.017230460044135053 | 대립가설 참 : 심결본인부담금과 출생년도와 관계가 있다. |


### 

<img src="images\분석.png" width="800"> 
----

### 🙋🏻‍♂️분석가 : 김명곤

<details>
<summary>분석정리</summary>



 ### < DDA >

| 변수 | 변수값 설명 | 유형 | 선택 이유 |
|--- | --- | --- | ---- |


 
### EDA
-
-

### 시각화

### 분석스토리 

| 변수명 |  pvalue |성립 가설  
| --- |--- |--- |

</details>

### 📚 STACKS

<img src="https://img.shields.io/badge/python-3776AB?style=for-the-badge&logo=python&logoColor=white"> 
<img src="https://img.shields.io/badge/mongoDB-47A248?style=for-the-badge&logo=MongoDB&logoColor=white">
  <img src="https://img.shields.io/badge/github-181717?style=for-the-badge&logo=github&logoColor=white">


  
