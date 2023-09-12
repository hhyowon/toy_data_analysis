
 # 📋 Join_Collection_BND_M20
- 고혈압 환자 대상 분석(설명 변수 5개 이상)
- 상병 코드 SICK_SYM1 = I10 (고혈압)

 ###  분석 목적
-  고혈압 환자들 중 ~~ 

 ### DDA
 
 | 변수 | 정의 | 유형 | 변수타입  | 선택 이유 |
  |--- | --- | --- | ---- |-- |
 |OFIJ_TYPE(공상 등 구분) | --- |범주형 | ---- |고혈압을 가진 사람들 중 공무상상해 등 희귀질환자나 상해를 당한 사람들이 더 요양개시일자가 빠를거라고  예상하여 선택함|
 |OPRTN_YN(수술여부)   | --- | 범주형| ---- |수술한 경험이 있는 사람들이 면연력이 떨어져 더 요양개시일자가 빠를거라고 예상하여 선택함|
 |BTH_YYYY(출생년도) | --- | 연속형 | ---- |출생년도를 통해 어느년도에 태어난 사람들이 전체적으로 요양개시일자가 빠르고 많은지 판단하기 위해 선택함 +  시각화를 통해 점점 출생년도가 높은 사람들이 요양개시일자가 빨라지는중인지 분석하기 위해 선택|
 |MDCARE_STRT_DT(요양개시일자) | --- | 연속형 | ---- | 초진에 어떤일이 일어났는지 분석하기 위함 |
 |MCARE_SUBJ_CD(진료과목코드) | --- | 범주형 | ---- | 진료를 받기 시작한 일자에 따라서 실제 진료를 받은 진료과목이 차이가 있나?  |
 |ED_RC_TOT_AMT(심결요양급여비용총액) | 연속형 | --- | ---- | 진료를 받기 시작한 일자에 따라서 건강보험 총요양급여비용이 차이가 있나? |
 |--- | --- | --- | ---- |-- |
 
 ### EDA,시각화
-
-![MCARE_SUBJ_CD](http://localhost:8888/files/Develops/toy_data_analysis/Join_Collection_BND_M20/CDA/MCARE_SUBJ_CD.png?_xsrf=2%7C7f3cb031%7C14099bc6f80e062912602031901529ec%7C1691394389)

### 분석스토리 

| 변수명 | 분석자  | pvalue |성립 가설  
| --- |--- |--- |--- |
| --- | 조효원,김명곤 |--- |--- |
| --- | 조효원 |--- |--- |
| --- | 조효원 |--- |--- |
| --- | 조효원 |--- |--- |


### 📚 STACKS

<img src="https://img.shields.io/badge/python-3776AB?style=for-the-badge&logo=python&logoColor=white"> 
<img src="https://img.shields.io/badge/mongoDB-47A248?style=for-the-badge&logo=MongoDB&logoColor=white">
  <img src="https://img.shields.io/badge/github-181717?style=for-the-badge&logo=github&logoColor=white">


  
