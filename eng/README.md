# English SA

오픈 소스 및 다른 소스 파일 참고 했습니다.(References에 링크 첨부)  
&nbsp;

# Data Description
"Friends"는 드라마 대본의 각 발화에 감정을 레이블링한 오픈 데이터셋입니다.

friends_train.json 파일을 이용해 훈련 데이터와 검증 데이터를 만들었고, 외부의 테스트 데이터는 사용하지 않았습니다.
캐글에서 제공한 en_data.csv 파일은 테스트 데이터로 사용하여 결과를 제출하였습니다.

|emotion|count|
|---|---|
|neutral|4752|
|non-neutral|2017|
|joy|1283|
|surprise|1220|
|anger|513|
|sadness|351|
|disgust|240|
|fear|185|

&nbsp;

# Requirements
- tensorflow
- numpy
- pandas
- transformers
- json
- numpy
- pandas
- tqdm

&nbsp;

# Usage
1. 사전 준비
2. 전처리
3. BERT pre-trained 모델 설정
4. 훈련
5. 모델 평가
6. 테스트
   
- colab과 google drive를 이용합니다.
- colab 환경에서 GPU를 이용해 모델 훈련을 합니다.
- google drive는 모델 저장 및 훈련 데이터(friends_train.json)와 테스트 데이터(en_data.csv)를 업로드 용도로 사용 합니다.
- 테스트는 캐글에서 제공한 테스트 데이터(en_data.csv)를 훈련 데이터와 동일하게 전처리 및 토크나이징을 하고 평가 결과(sample.csv)를 파일로 저장합니다.
- sa_eng.ipynb 파일에 실행을 위한 설명을 자세히 설명하였습니다.
  
&nbsp;
# References

https://nxrmrz.github.io/project/bert-emotion-classification

https://analyticsindiamag.com/how-i-used-bidirectional-encoder-representations-from-transformers-bert-to-analyze-twitter-data

https://www.secmem.org/blog/2020/07/19/Sentiment-Analysis
