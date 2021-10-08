# 프로젝트 개요

## 목적

- Google Firebase와의 연동을 통해 Authentication 기능을 활용하고, 기본적으로 React App에서는 어떻게 user Authentication을 관리하는지 익히는 것을 목적으로 한다.
- JWT의 개념과 사용법을 익히고 실제로 적용해본다.

## 주요 기능(요구사항)

- Google Firebase DB와 연동하여 Identity Toolkit API사용을 통해 회원가입 및 회원 관리 기능을 구현
- 로그인, 로그아웃, 비밀번호 변경등이 주요 기능이고 firebase DB에서 실시간으로 회원내역들을 확인 가능하다.

## 주요 로직

- 세션 개념 및 세션을 응용한 자동 로그아웃 기능을 적용한다.
- Context로는 token, isLoggedIn(로그인 상태 체크), 로그인 함수, 로그아웃 함수를 만든다.
- Token은 localstorage에 저장함으로써, 현재 로그인한 유저가 해당 유저라는 것을 보증하고, 세션 만료 시간을 설정하는데 세션 만료 시간이 1분이 이하로 남으면 유저의 로그인 정보를 제거한다.
- useRef를 사용해 form의 input data를 가져와 submit하는 handler 함수를 구현한다.
- useHistory를 사용해 특정 url을 제어하는 기능을 구현한다.
