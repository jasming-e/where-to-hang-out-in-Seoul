# Where to hang out in Seoul
서울특별시 관광지 추천 대시보드


# Where-To-Hang-Out-In-Seoul : 서울 어디까지 가봤니?

## 1. 프로젝트 개요
- 기간
  - 21.11.03 - 21.12.05 
- 소개
  - 서울에서 놀고 싶지만 어디에서 놀아야 할지 모르겠을 때, 어디서 어떻게 정보를 얻어야 할지 귀찮고 어려웠던 경험이 다들 있으신가요? 특히 외국인은 더욱 낯설었을 것입니다. 이러한 어려움과 귀찮음을 해결할 수 있도록 서울시의 다양한 관광 정보를 여러 언어로 편하게 알 수 있는 대시보드를 소개합니다. 관광 명소/자연/문화/쇼핑 중 자신이 원하는 서울시의 구별 관광 정보를 얻을 수 있습니다. 더불어 날씨 정보를 따로 찾아야 하는 번거로움을 없애기 위해 관광 지수와 날씨 정보를 합쳐 편리하게 서울시의 다양한 놀거리 정보를 제공해 줍니다.

## 2. 데이터 수집
- 채널 : 공공데이터포털, 네이버 날씨(기상청 제공)
- 구성
  - [서울 관광 자연](https://www.data.go.kr/data/15083935/fileData.do)
  - [서울 관광 명소](https://www.data.go.kr/data/15083933/fileData.do)
  - [서울 관광 문화](https://www.data.go.kr/data/15083932/fileData.do)
  - [서울 관광 쇼핑](https://www.data.go.kr/data/15083934/fileData.do)
  - [관광지수/등급](https://www.data.go.kr/data/15007097/fileData.do)
  - [기온 정보](https://search.naver.com/search.naver?where=nexearch&sm=top_hty&fbm=1&ie=utf8&query=%EC%84%9C%EC%9A%B8+%EB%82%A0%EC%94%A8)

## 3. 데이터 소개
```
💃🏻 Where-To-Hang-Out-In-Seoul
 ┣ 📂 code
   ┣ 📄 seoul_attraction.ipynb
   ┣ 📄 seoul_entertainment.ipynb
   ┣ 📄 seoul_nature.ipynb
   ┣ 📄 seoul_shopping.ipynb
   ┣ 📄 seoul_touristic_whether.ipynb
   ┣ 📄 seoul_whether.ipynb
   ┣ 📄 seoul_preprocessing+eda.ipynb
   ┣ 📄 seoul_total.ipynb
 ┣ 📂 data
   ┣ 📄 seoul_attraction.xlsx
   ┣ 📄 seoul_entertainment.xlsx
   ┣ 📄 seoul_nature.xlsx
   ┣ 📄 seoul_shopping.xlsx
   ┣ 📄 seoul_tourism.xlsx
   ┣ 📄 seoul_touristic_whether.xlsx
   ┣ 📄 seoul_whether.csv
   ┣ 📄 gu_list.xlsx
   ┣ 📄 seoul_total.xlsx
 ┣ 📄 Where-To-Hang-Out-In-Seoul.twbx
 ┗ 📄 Where-To-Hang-Out-In-Seoul-Poster.pdf
```

1. code 설명
    - ```seoul_attraction.ipynb```, ```seoul_entertainment.ipynb```, ```seoul_nature.ipynb```, ```seoul_shopping.ipynb```, ```seoul_touristic_whether.ipynb```
      - 공공데이터포털에서 OPEN API를 활용하여 서울 관광 및 기상 정보를 크롤링하고 데이터에 맞는 기본 전처리를 진행한다.  
    - ```seoul_whether.ipynb```
      - 네이버 날씨(기상청 제공)에서 서울 날씨 중 현재일 기준 오늘/내일/모레의 최고/최저 기온을 크롤링한다.
    - ```seoul_preprocessing+eda.ipynb```
      - 서울 관광 명소/문화/자연/쇼핑 데이터를 통합하여 추가적인 전처리를 진행하고, EDA를 수행한다.
    - ```seoul_total.ipynb```
      - 대시보드 시각화를 위해 서울 관광 데이터와 관광지수 데이터를 전처리 후 하나로 합친다.
2. data 설명
    - ```seoul_attraction.xlsx```, ```seoul_entertainment.xlsx```, ```seoul_nature.xlsx```, ```seoul_shopping.xlsx```
      - OPEN API를 활용해 서울 관광 정보를 수집한 데이터
    - ```seoul_tourism.xlsx```
      - 서울 관광 명소/문화/자연/쇼핑 데이터를 통합하고 전처리를 완료한 관광지 관련 최종 데이터
    - ```seoul_touristic_whether.xlsx```, ```seoul_whether.csv```
      - 전처리를 완료한 서울시 기온 및 관광지수 데이터
    - ```gu_list.xlsx```
      - 언어별(한국어/영어/일본어/중국어) 정리한 구 리스트
    - ```seoul_total.xlsx```
      - 서울 관광 데이터와 관광지수 데이터를 합쳐 대시보드 시각화에 사용되는 최종 데이터

📌 더 많은 정보를 얻고 싶으면, ```Where-To-Hang-Out-In-Seoul-Poster.pdf```를 참고해 주세요.

## 4. 대시보드
   <p align="center"><img width="800" alt="Where-To-Hang-Out-In-Seoul?" align="center" src="https://user-images.githubusercontent.com/78864775/144639744-74548c79-f27b-4ea4-8fa1-920685cdef8f.png"></p>

   - [Tableau](https://public.tableau.com/app/profile/jimin.kang/viz/1126_16381024790430/1)에서 직접 대시보드를 이용할 수 있습니다.

## 5. 개발 환경
- Google Colab
- Tableau

## 6. 팀원
|이름|email|
|---|---|
|지다영|dys621124@gmail.com|
|류혜원|jg0149@sookmyung.ac.kr|
|강지민|jasmin2150@sookmyung.ac.kr|


© 2021 DaYeong Ji, Hyewon Ru, Jimin Kang,  <dys621124@gmail.com, jg0149@sookmyung.ac.kr, jasmin2150@sookmyung.ac.kr>
