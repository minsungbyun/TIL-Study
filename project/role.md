프로젝트에서 담당했던 부분

로그인, 회원가입

- 로그인 폼 제작
- 로그인 했을 때
- 아이디, 비밀번호 디비에 있으면 세션등록하고 리다이렉트
- 로그인 실패했을 때 다시 로그인페이지로
- 로그아웃 구현
- session.invalidate()
- 개인회원가입
- Part를 통한 사진 추가, 썸네일 사용

[아이디 중복 구현]
- @ResponseBody

[아이디 저장 구현]
- 최초로 서버에서 쿠키 생성
아이디 저장 체크한다면?
- id넣은쿠키생성, 유효기간설정, path설정, 로그설정
아이디 저장 체크하지 않는다면?
- 빈쿠키생성, 유효기간0설정 

상수 클래스 지정 

봉사
- 봉사 리스트 
- 봉사 세부사항

관리자
- 회원 리스트
- 봉사 승인, 반려
- 모달 관리 