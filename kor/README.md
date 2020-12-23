# Korean SA

오픈 소스 및 다른 소스 파일 참고 했습니다.(References에 링크 첨부)  
&nbsp;

# Data Description
"NSMC"는 네이버 영화 리뷰에 달린 별점을 긍정/부정으로 변환한 binary-class 데이터셋입니다.
주어진 문장을 긍정(1) 혹은 부정(0)으로 분류 합니다.

ratings_train.json 파일을 이용해 훈련 데이터로 만들었고, 외부의 테스트 데이터는 사용하지 않았습니다.
캐글에서 제공한 ko_data.csv 파일은 테스트 데이터로 사용하여 결과를 제출하였습니다.

|emotion|count|
|---|---|
|0|75173|
|1|74827|


|emotion|count|
|---|---|---|
|0|75173|
|1|74827|


&nbsp;

# Requirements
- torch
- pandas
- tqdm
- bs4
- sklearn
- transformers d
- numpy
- contractions 

&nbsp;
# Usage
1. 사전 준비
2. 전처리
3. KoBERT 모델 설정
4. 훈련
5. 테스트
   
- colab과 google drive를 이용합니다.
- colab 환경에서 GPU를 이용해 모델 훈련을 합니다.
- google drive는 모델 저장 및 훈련 데이터(ratings_train_train.txt)와 테스트 데이터(ko_data.csv)를 업로드 용도로 사용 합니다.
- 테스트는 캐글에서 제공한 테스트 데이터(en_data.csv)를 훈련 데이터와 동일하게 전처리 및 토크나이징을 하고 평가 결과(sample.csv)를 파일로 저장합니다.
- sa_kor.ipynb 파일에 실행을 위한 설명을 자세히 설명하였습니다.

&nbsp;
# References

https://github.com/kimwoonggon/publicservant_AI

https://github.com/monologg/KoBERT-Transformers
