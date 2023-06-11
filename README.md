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
react-router-dom의 outlet 컴포넌트를 사용하여 로그인, 회원가입 페이지에서는 nav바와 footer가 포함되지 않도록 구현하였습니다. <br/>
![signup-성공시](https://github.com/woong3e/46-1st-BestFriend-frontendGw/assets/86347667/ac69409e-45bb-4307-85e7-6c3f4f3293ec)
![signup-실패시](https://github.com/woong3e/46-1st-BestFriend-frontendGw/assets/86347667/1f97e149-e37a-486d-a6d3-7ae6447a47c8)
- map메서드를 사용하여 유저정보를 입력하는 input과 유효성검사에 따른 메시지를 담는 p태그를 만들었고, 상수데이터를 활용하여 키값을 부여했습니다. 유효성검사하는 객체를 선언하였고 그 반환값에 따라 다른 텍스트를 보여주는 객체를 선언하였습니다. 각 input의 유효성검사를 통과하면 아래 p태그 값과 색이 바뀌도록 하였습니다. 모든 유효성검사를 통과하고 체크박스를 체크한뒤 버튼클릭하면 API요청하도록합니다.  통신이 성공하면 로그인 페이지로 이동해 바로 로그인을 할 수 있도록 구현했습니다. <br/>
![login-성공시](https://github.com/woong3e/46-1st-BestFriend-frontend/assets/86347667/e9178ee7-be40-4e6a-b318-097d21042453)
![login-실패시](https://github.com/woong3e/46-1st-BestFriend-frontend/assets/86347667/865fb416-16ba-49bc-a5c8-83803a7bac7a) <br/>
- 로그인 유효성 검사에 따라 값이 입력되지 않았을 때, ‘로그인에 실패했다’라는 토스트팝업 유저에게 띄워주고, 성공시에는 API 요청하도록 했습니다. API요청후 데이터가 일치하지 않았을 때에도 실패했다는 토스트팝업을 띄어 유저가 쉽게 알 수 있도록 했습니다.

4. 상품 카테고리, 필터, 정렬, 페이지네이션, 검색
5. 상품 상세페이지 동적 라우팅
6. 위시리스트, 장바구니
7. 결제 <br/>
![checkout-성공시](https://github.com/woong3e/46-1st-BestFriend-frontendGw/assets/86347667/26289f30-d612-45c5-a55e-115942866d7d)
![checkout-실패시](https://github.com/woong3e/46-1st-BestFriend-frontendGw/assets/86347667/cb02dbd3-2e66-4dfd-93c2-a471108f4c9c) <br/>
- API요청후에 서버에서 유저정보와 장바구니에서 담은 리스트들을 get메서드를 사용하여 나타냅니다. 포인트가 충분할 때 결제API요청후 통신 성공시 모달창에 API통신후의 데이터 정보를 담았고 결제창의 정보를 blur처리 한 후 setTimeout 함수를 사용하여 5초후 메인페이지로 이동하도록 하였습니다. 포인트가 부족할 때는 토스트팝업을 띄워 함수를 종료시킵니다.
9. 기타: 캐러셀, 토스트 팝업
- 토스트팝업은 API통신에 실패할 경우, 유효성 검사에 실패했을 경우에 UX개선을 위해 사용하였습니다. setTimeout 함수를 사용하여 일정시간 후 사라지도록 하였습니다.

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
