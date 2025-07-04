# T-Box: Terminal box
ELEC462 시스템 프로그래밍 프로젝트 – 21조 `턴왔조`

## 프로젝트 소개
T-Box는 두 개의 터미널 간에 실시간 통신을 통해 사용자가 틱택토 게임을 즐길 수 있도록 구현한 멀티스레드 게임 플랫폼이다.
- 실시간 채팅
- 제한시간(10초) 타이머
- 게임 기록 저장
- 추후 다양한 게임으로 확장 가능

## 주요 기능
- 터미널 간 통신
- `pthread`를 사용한 멀티스레드 구조로 서버와 게임 분리
- 실시간 입력 처리 + 채팅 기능
- 10초 제한 타이머 (입력 없으면 자동 패배)
- 게임 결과 서버에 저장
- 틱택토 외 게임 모듈 분리 구조 설계

## 스크린샷
![KakaoTalk_Photo_2025-06-24-19-12-19.png](attachment:0243a908-3119-4011-be36-60f1c1c06630:KakaoTalk_Photo_2025-06-24-19-12-19.png)

![KakaoTalk_Photo_2025-06-24-19-17-04.png](attachment:436586e1-b998-45f1-9e53-39f6053151ac:KakaoTalk_Photo_2025-06-24-19-17-04.png)

## 빌드 및 실행
빌드: make 할시 자동으로 빌드됩니다.
코드 수정 시 make clean 후 다시 make합니다.
실행 방법
./main ->
1.실행 시 메뉴가 나타납니다.
2.서로 다른 두개의 터미널에서 ./main을 실행한 뒤
틱택토 실행, 한명은 O,한명은 X를 선택하면 정상 작동됩니다.

## 디렉토리 구조
project_21/
-main.c
-makefile
-game_result.txt
-common.h
-games/
 -record.c
 -record.h
 -player1.c
 -player2.c

## 팀원 정보
글로벌소프트웨어융합전공 이상재
글로벌소프트웨어융합전공 권보민
미디어커뮤니케이션 임선아
