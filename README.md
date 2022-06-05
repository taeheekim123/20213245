# 20213245

<리눅스 명령어>


-top : 시스탬 프로세스/메모리 사용 현황을 실시간으로 출력

가장 상단에 리눅스 시스템이 실행되고 난 후 부터 지금까지 시간과 로그인 사용자 수, 시스템 부하율을 표시하는 명령어 uptime 결과표시
그 아래엔 프로세스 수치, CPU 정보, 메모리 정보, 프로세스 별 부하율과 상태 표시

top[옵션]을 입력하여 사용 (-b옵션 : 순간의 정보 확인, -n옵션 : 살행 주기를 n번 반복)


-ps : ‘process status’의 약자로 현재 실행중인 프로세스 목록 확인

![ka38_241_i1](https://user-images.githubusercontent.com/104884855/172055530-7a980fd9-85d8-4807-99a3-7dc7f936b5e0.jpeg)


일정 주기를 합산하는 top과 다르게 ps는 ps 한 시점에 검색한 cpu 사용량을 출력

ps -e (모든 프로세서 출력), ps -f (풀 포맷으로 출력) 


-jobs : 작업이 중지된 상태, 백그라운드로 진행 중인 작업 상태, 변경되었지만 보고되지 않은 상태 등을 표시

사용법은 이러하며 세션의 상태값으로 현재 세션의 작업 상태를 출력

jobs[옵션][job ID]
Jobs -x command[args]

![ka38_241_i1](https://user-images.githubusercontent.com/104884855/172055645-b3ca1888-312c-4f2a-a64c-e7d8c465ac39.jpeg)



-kill : 프로세스 종료 명령어
지정한 프로세스에 지정한 시그널을 보냄
시스템에 문제가 생겨 해당 프로세스를 종료할 필요가 있을 경우 많이 사용
kill [옵션 or 시그널] [프로세스 번호] 로 해당 프로세스를 종료


<vim 에디터 매크로 사용방법(q, @)>


q<저장할 매크로 문자> 를 입력한다.

매크로 내용을 기록한 후 중립모드로 돌아온다.

q를 눌러 매크로를 끝낸다.


앞 단계를 실행 후 중립모드에서 @<저장한 매크로 문자> 를 입력하여 매크로를 실행한다.

매크로 반복실행은 반복횟수@<저장한 매크로 문자>

마지막 수행 매크로 실행은 @@를 입력한다.


매크로를 저장하려면 현재 편잡중 내용을 저장 후 ~/vimrc를 연다.(:r or :e)

저장할 매크로 이름을 변수로 하여 저장한다.

let@<변수명>=‘ctrl+r ctrl+r <마지막 사용 매크로 문자>’

