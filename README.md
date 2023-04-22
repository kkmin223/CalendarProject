# CalendarProject

일정 관리 서비스
# 목표
- 테스트 코드 적용 해보기
- 인터페이스 사용(OOP 적으로 짜보기)
- 스프링 부트 기초 개념 복습
- 배포 

#  기능
- 일정 등록(우선순위 3)
    - 일정을 등록한다.
        - 일정 이름, 날짜, 시작 시간, 종료 시간, 장소(선택), 메모 입력할 수 있다.
    - 일정을 수정할 수 있다.
        - 일정이름, 날짜, 시작 시간, 종료 시간, 장소, 메모 수정 가능
    - 일정을 삭제할 수 있다.
- 일정 보기(우선순위 4)
    - 달력 형식으로 특정 월에 대한 달력으로 일정을 보여 줄 수 있다.
    - 일자 형식으로 특정 일에 대한 일정을 보여줄 수 있다.
- 그룹 기능(우선순위 5)
    - 그룹을 가입 가능
    - 그룹 일정 등록 가능
- 회원 가입(우선순위 1)
    - 회원 가입할 수 있다.
    - 회원 가입 시 닉네임 아이디, 비밀번호 입력
    - 회원 가입을 해야 일정 등록 가능
- 로그인(우선순위 2)
    - 로그인
    - 로그아웃
- 외부 API 연동
  - 카카오 API를 사용해 일정 알림 

# 2. 사용 기술

- 백엔드 : 스프링 부트, JPA, H2
- 프론트엔드: ThymeLeaf, CSS, JS
- Jenkins, Junit

# 3. 모델

사용자(User)

- userId
- loginId
- password
- nickname
- registerDate

일정(Schedule)

- scheduleId
- userId
- scheduleName
- memo
- startDateTime
- endDateTime
- address
- groupId
- registerDate
- updateDate

일정그룹(Group)

- groupId
- userId
