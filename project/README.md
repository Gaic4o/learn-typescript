## 코로나 세계 현황판 만들기

최종 프로젝트 폴더입니다

## 참고 자료

- [존스 홉킨스 코로나 현황](https://www.arcgis.com/apps/opsdashboard/index.html#/bda7594740fd40299423467b48e9ecf6)
- [Postman API](https://documenter.getpostman.com/view/10808728/SzS8rjbc?version=latest#27454960-ea1c-4b91-a0b6-0468bb4e6712)
- [Type Vue without Typescript](https://blog.usejournal.com/type-vue-without-typescript-b2b49210f0b)

## 자바스크립트 프로젝트에 타입스크립트 적용하기.

0. 자바스크립트 파일에 JSDoc 으로 타입 시스템 입히기.


1. 타입스크립트의 기본 환경 구성.
    - [x] NPM 초기화 
    - [x] 타입스크립트 라이브러리 설치.
      npm init -y, npm i typescript --save-dev 

    - [x] 타입스크립트 설정 파일 생성 및 기본 값 추가. 
      tsconfig.json 

    - [x] 자바스크립트 파일을 타입스크립트 파일로 변환. 
       // npm run build 를 치면 -> 모든 스크립트는 tsc 로 변환
    - [x] `tsc` 명렁어로 타입스크립트 컴파일 하기.


2. 명시적인 `any` 선언하기
    - `tsconfig.json` 파일에 `noImplicitAny` 값을 `true` 로 추가. 
      이런 식 으로 해주면 type error 가 +39 개 추가된다. 
    - 가능한한 구체적인 타입으로 타입 정의. 


3. 프로젝트 환경 구성.
  - bable, eslint, prettier 등의 환경 설정.


4. 외부 라이브러리 모듈화. axios 등. 
  axios 라이브러리 설치 및 타입 에러 확인 - npm i axios 
  axios 에러가 나타나지 않음. axios 설치 해 import 해서 타입 문제가 해결 되는 것은 axios 잘 만들어지면서 잘 관리 가 되기 떄문에 .

  오픈소스에선 잘 이렇지는 않음.

  chart.js 설치 

라이브러리 임포트 구문에서 나는 타입 에러 방식.



Definitely Typed 소개.







바벨 추가.

바벨은 -> Javascript compiler.
최신 자바스크립트 문법의 여러 브라우저에서 호환 해 주는 도구.



ESLint -> 코드 문제를 알려 줌.
- 저장하면 자동으로 var -> const 로 바꿈 .
자바스크립트 코드를 에러가 덜 나는 방향으로 작성하도록 와주는 문법 보조 도구.


ESLint 규칙 및 설정 파일 소개.



Rules - ESLinst 어떤 규칙을 가지고 파일을 검증할 지 하는 속성 입니다.
-> extends: eslint:recommended


 extends: [
    'eslint:recommended', // 검증하는 옵션을 가지고 파일을 검증하겟다.


rules: { prettier 
-> 기본적 eslint 설명 그리고 왜 typescript 왜ㅑ eslint 을 먹어야 할 가?





옵션 . 

print - width 한 줄의 길이. 몇 자까지 한 줄로 칠 것인지 줄바꿈 등 설정할 수 있음.

Tab width 

세미콜론 - 붙인다 안붙인다. 등 
이런 값들을 이용해 설정 할 수 있음.


타입스크립트 프로젝트 환경 구성.
1. 프로젝트 폴더 생성.
2. npm init -y 로 package.json 파일 생성.
3. 아래 명령어로 타입스크립트 및 문법 검사, 코드 정리 도구 라이브러리 추가.
4. npm i -D babel...

.eslintignore 이 파일안에 있는 node_modules  이것은 무시하겠다. 






외부 라이브러리 모듈화 진행을 위한 사전 작업.






