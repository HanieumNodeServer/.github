# 인공지능(AI)기반 챗봇 주문·예약·예매 시스템, 불러부릉



![image](https://user-images.githubusercontent.com/79521972/215462121-739c08cf-af88-4ee9-b549-b6849c35b1bc.png)

### 

### 소개

- 음성인식을 통해 전국 시외버스 터미널의 버스를 예약할 수 있는 서비스입니다.
- 사용자의 음성을 인공지능을 통해 분석하여 핵심 정보를 추출하고, 해당 정보를 기반으로 맞춤 편의를 제공합니다.



### 기대효과

- 코로나19와 같이 예상치 못한 상황에서 예매를 비대면으로 진행하더라도 디지털 취약 계층이 소외되지 않고, 급격히 변화하는 상황에 유연하게 대응할 수 있습니다. 
- **대화형 서비스**이기 때문에 사용자가 이용하면서 편리하고 친숙하게 느낄 수 있습니다. 
- 기존의 터치식 UI/UX에서 사용자 음성 한 마디로, 모든 정보를 빠르게 간편하게 조회할 수 있습니다.



### 기록 

- [2022 한이음 공모전](https://www.hanium.or.kr/portal/subscription/info.do?trackSeq=8) 한국정보산업연합회 회장상 수상작입니다.
- 팀 노션 블로그: https://www.notion.so/d92b27a1f4c74d3092f48fc689a3ad9f?v=909eca2f00034caf95d76c0e222aeddf






## 기술 스택

|                           Frontend                           |                           Backend                            |                              DB                              |                            MODEL                             |                          TEST TOOL                           |
| :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
| <img src="https://img.shields.io/badge/react_native-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB"/> <img src="https://img.shields.io/badge/redux-%23593d88.svg?style=for-the-badge&logo=redux&logoColor=white"/> | <img src="https://img.shields.io/badge/-TmoneyAPI-purple"/> <img src="https://img.shields.io/badge/NodeJs-339933?style=flat-square&logo=Node.js&logoColor=white"/> <img src="https://img.shields.io/badge/Express-000000?style=flat-square&logo=Express&logoColor=white"/> <img src="https://img.shields.io/badge/PM2-2B037A?style=flat-square&logo=PM2&logoColor=white"/> <img src="https://img.shields.io/badge/Flask-000000?style=flat-square&logo=Flask&logoColor=white"/> <img src="https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=Amazon AWS&logoColor=white"/> <img src="https://img.shields.io/badge/JWT-000000?style=flat-square&logo=Json Web Tokens&logoColor=white"/> | <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white"/> | <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/> <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white"/> | <img src="https://img.shields.io/badge/Postman-FF6C37?style=flat-square&logo=postman&logoColor=white"/> |





## 서비스 구성도

![image](https://user-images.githubusercontent.com/79521972/215478809-1bf2bb82-f2c9-4561-90c3-dec658c53bdb.png)

## 서비스 흐름도

![img](https://www.hanium.or.kr/html/synap/20221119091651559.hwp.files/BIN0001.png)



- 배차 스케줄 저장 테이블에 저장된 데이터는 매일 00시00분에 Batch 프로그램을 통해 Tmoney API에서 정보를 가져와서 가공하고 저장합니다
- 당일 기준으로부터 약 30일까지의 데이터만 Tmoney 사에서 제공해주어서 약 한 달치의 정보만 예약만 접근 가능합니다.



## 어플리케이션 기능 시연

- 더 많은 사용자 요구에 유연하게 대응하기 위해 다양한 상황에도 동작할 수 있도록 설계했습니다. 아래 경우들이 그 예시입니다.
- 데모 및 설명은 다음 [데모 영상](https://www.youtube.com/watch?v=6zD_0TfGN8E)을 참고해 주세요. 


|                   모든 정보가 포함된 문장                    |                     중간에 리셋하는 경우                     |                     중간에 수정하는 경우                     |                      도착지만 말한 경우                      |                         승차권 확인                          |
| :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
| <img src = "https://user-images.githubusercontent.com/79521972/215475729-7b865432-7f2c-42f8-8998-3a3860094916.gif" width = 120vw height = 250vh> | <img src = "https://user-images.githubusercontent.com/79521972/215478237-0a4d4c60-2ddc-4810-9898-0d80fb14cf52.gif?raw=true" width = 120vw height = 250vh> | <img src = "https://user-images.githubusercontent.com/79521972/215477360-976ab9ca-cb6c-417e-a617-5e189da0e42f.gif?raw=true" width = 120vw height = 250vh> | <img src = "https://user-images.githubusercontent.com/79521972/215476950-c0b23b52-a4a1-44f0-9f4e-9ee3a8674b78.gif?raw=true" width = 120vw height = 250vh> | <img src = "https://user-images.githubusercontent.com/79521972/215476255-f412f81b-1783-4b64-9775-98252e4421dd.gif?raw=true" width = 120vw height = 250vh> |
| [크게 보기](https://user-images.githubusercontent.com/79521972/215475729-7b865432-7f2c-42f8-8998-3a3860094916.gif) | [크게 보기](https://user-images.githubusercontent.com/79521972/215478237-0a4d4c60-2ddc-4810-9898-0d80fb14cf52.gif) | [크게 보기](https://user-images.githubusercontent.com/79521972/215477360-976ab9ca-cb6c-417e-a617-5e189da0e42f.gif) | [크게 보기](https://user-images.githubusercontent.com/79521972/215476950-c0b23b52-a4a1-44f0-9f4e-9ee3a8674b78.gif) | [크게 보기](https://user-images.githubusercontent.com/79521972/215476255-f412f81b-1783-4b64-9775-98252e4421dd.gif) |





## 멤버 소개

|                                           |                                        | <img src="https://user-images.githubusercontent.com/79521972/215472852-665c36fd-1397-461e-aced-6380dc92f563.png" width="100px"> |                                      |
| :---------------------------------------: | :------------------------------------: | :----------------------------------------------------------: | :----------------------------------: |
| [최다솜](https://github.com/podongx2somm) | [황수현](https://github.com/suhyeon17) |           [강창룡](https://github.com/speardragon)           | [조준기](https://github.com/jknadan) |
|             Chatbot AI, Lead              |               Chatbot AI               |                  App Backend, App Frontend                   |      App Backend, App Frontend       |





## Reference





