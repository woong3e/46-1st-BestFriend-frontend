# Project grön

![waving](https://capsule-render.vercel.app/api?type=waving&height=200&fontAlignY=40&text=grön&color=gradient)

#### \*Nike 웹사이트를 모델링한 프로젝트입니다.

## 🧚‍♂️ 개발 기간 및 인원

- 개발 기간 : 2023/05/26 ~ 2023/06/09
- 개발 인원 : 프론트엔드 3명 , 백엔드 1명
  - Product Manager: 김혜중(B)
  - Project Manager: 조혜진(F)
  - Teammates: 이재웅(F), 장건웅(F)
- 깃헙 레포지토리
  - [Frontend](https://github.com/wecode-bootcamp-korea/46-1st-BestFriend-frontend)
  - [Backend](https://github.com/wecode-bootcamp-korea/46-1st-BestFriend-backend)

## 🪴 서비스 소개

### 1. 기획의도

- 나이키처럼 건강한 라이프 스타일을 추구하는 고객을 타겟으로 선정
- 나이키 웹사이트 UX,UI 디자인의 강점을 살려 화면 구성
- 식물에 대해 잘 모르는 사람도 니즈에 맞는 식물을 쉽게 고를 수 있도록 기능 기획
- 식물에 대한 진입장벽을 낮추고 편리하게 식물을 구매할 수 있는 서비스

### 2. 서비스 개요

- 서비스명 : grön
- 판매상품 : 식물, 화분, 관리도구
- 고객 : 반려식물 집사가 되고 싶은 누구나

## ⚡️ 구현 기능

1. 내비게이션 바 드롭다운 메뉴
2. 회원가입/로그인 <br/>
![login-성공시](https://github.com/woong3e/46-1st-BestFriend-frontend/assets/86347667/e9178ee7-be40-4e6a-b318-097d21042453)![login-실패시](https://github.com/woong3e/46-1st-BestFriend-frontend/assets/86347667/aa8d6f7f-acf5-43a6-8f2e-9b4b15bd3d98)
![login-실패시](https://github.com/woong3e/46-1st-BestFriend-frontend/assets/86347667/865fb416-16ba-49bc-a5c8-83803a7bac7a)

- react-router-dom의 outlet 컴포넌트를 사용하여 로그인, 회원가입 페이지에서는 nav바와 footer가 포함되지 않도록 구현
- 로그인 페이지에서 유효성검사 통과시 API 요청.
- 백엔드 통신 후 분기처리
- 성공시 메인이동, 실패시 토스트팝업 알림


4. 상품 카테고리, 필터, 정렬, 페이지네이션, 검색
5. 상품 상세페이지 동적 라우팅
6. 위시리스트, 장바구니
7. 결제
8. 기타: 캐러셀, 토스트 팝업

## 📚 기술 스택

### Frontend

|                                             JavaScript                                             |                                                 React                                                 |                                              scss                                               |                                                 esLint                                                 |                                                 Prettier                                                 |
| :------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------: |
| <img src="https://techstack-generator.vercel.app/js-icon.svg" alt="icon" width="65" height="65" /> | <img src="https://techstack-generator.vercel.app/react-icon.svg" alt="icon" width="65" height="65" /> | <img src="https://techstack-generator.vercel.app/sass-icon.svg" width="65" height="65" /></div> | <img src="https://techstack-generator.vercel.app/eslint-icon.svg" alt="icon" width="65" height="65" /> | <img src="https://techstack-generator.vercel.app/prettier-icon.svg" alt="icon" width="65" height="65" /> |

### Backend

|                                             JavaScript                                             |                                                Node.js                                                |                                                    MySQL                                                     |
| :------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------: |
| <img src="https://techstack-generator.vercel.app/js-icon.svg" alt="icon" width="65" height="65" /> | <img src="https://techstack-generator.vercel.app/nginx-icon.svg" alt="icon" width="65" height="65" /> | <img src="https://techstack-generator.vercel.app/mysql-icon.svg" alt="icon" width="65" height="65" /> </div> |

## ⚙️ 협업툴

<div>
<img src="https://img.shields.io/badge/Git-F05032?style=flat&logo=Git&logoColor=white"/>
<img src="https://img.shields.io/badge/GitHub-181717?style=flat&logo=GitHub&logoColor=white"/>
<img src="https://img.shields.io/badge/Slack-4A154B?style=flat&logo=Slack&logoColor=white"/>
<img src="https://img.shields.io/badge/Trello-0052CC?style=flat&logo=Trello&logoColor=white"/>
<img src="https://img.shields.io/badge/Notion-000000?style=flat&logo=Notion&logoColor=white"/>
<img src="https://img.shields.io/badge/Figma-F24E1E?style=flat&logo=Figma&logoColor=white"/>
<img src="https://img.shields.io/badge/VSCode-007ACC?style=flat&logo=Visual Studio Code&logoColor=white"/>
</div>
