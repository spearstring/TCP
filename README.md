# Study TCP/UDP

<br/>

TCP/UDP 소켓 통신 학습 리포지토리

<hr/>

<br/>

## 1. 네트워크 프로그래밍과 소켓의 이해
  - 네트워크 프로그래밍과 소켓의 이해
  - 리눅스 기반 파일 조작하기
  - 실습
      - "Hello world!" 서버 프로그램 구현
      -  리눅스 기반 파일 조작 - 파일에 데이터쓰기
      -  리눅스 기반 파일 조작 - 파일에 저장된 데이터 읽기
      -  파일 디스크립터와 소켓
      -  윈도우 기반 클라이언트 구현

<br/>

## 2. 소켓의 타입과 프로토콜의 설정
  - 소켓의 프로토콜과 그에 따른 데이터 전송 특성
  - 실습
      - TCP 소켓
<br/>

## 3. 주소체계와 데이터 정렬
  - 소켓에 할당되는 IP주소와 PORT번호
  - 주소정보의 표현
  - 네트워크 바이트 순서와 인터넷 주소 변환
  - 인터넷 주소의 초기화와 할당
  - 실습
      - 바이트 순서의 변화 - 리틀 엔디안
      - 문자열 정보를 네트워크 바이트 순서의 정수로 변환 - inet_addr(), iner_aton(), inet_ntoa()
<br/>

## 4. TCP 기반 서버/클라이언트 1
  - TCP와 UDP에 대한 이해
  - TCP기반 서버, 클라이언트 구현
  - lterative 기반의 서버, 클라이언트 구현
  - 실습
      - "Hello world" 서버/클라이언트 구현
      - lterative 에코 서버/클라이언트 구현

<br/>

## 5. TCP 기반 서버/클라이언트 2
  - 에코 클라이언트 구현
  - TCP의 이론
  - 실습
      - 에코 서버/클라이언트 수정
      - 계산기 서버/클라이언트 구현 

<br/>

## 6. UDP 기반 서버/클라이언트
  - UDP에 대한 이해
  - UDP 기반 서버/클라이언트의 구현
  - UDP의 데이터 송수신 특성과 UDP에서의 connect 함수호출
  - 실습
      - UDP기반 에코 서버/클라이언트 구현
      - 데이터의 경계가 존재하는 UDP 소켓
      - connected UDP 소켓 생성

<br/>

## 7. 소켓의 연결종료
  - TCP 기반의 Half-close
  - 실습
      - Half-close - shutdown 함수

<br/>

## 8. 도메인 이름과 인터넷 주소
  - Domain Name System
  - IP주소와 도메인 이름 사이의 변환
  - 실습
      - 도메인 이름을 이용해서 IP주소 받아오기
      - IP주소를 이용해서 도메인 정보 받아오기

<br/>

## 9. 소켓의 다양한 연결 옵션
  - 소켓의 옵션과 입출력 버퍼의 크기
  - SO_REUSEADDR
  - TCP_NODELAY
  - 실습
      - getsockopt, setsockopt
      - SO_SNDBUF, SO_RCVBUf
      - 주소할당 에러 발생, 주소 재할당
      
<br/>

## 10. 멀티프로세스 기반의 서버구현
  - 프로세스 이해와 활용
  - 프로세스 & 좀비(Zombie) 프로세스
  - 시그널 핸들링
  - 멀티태스킹 기반의 다중접속 서버
  - TCP의 입출력 루틴(Routine) 분할
  - 실습
      - fork 함수호출을 통한 프로세스 생성
      - 좀비 프로세스 생성
      - 좀비 프로세스 소멸 - wait함수, waitpid 함수
      - signal 함수
      - sigaction 함수를 이용한 시그널 핸들링
      - 시그널 핸들링을 통한 좀비 프로세스 소멸
      - 다중 에코서버 구현
      - 에코 클라이언트 입출력 루틴 분할
      
<br/>

## 11. 프로세스간 통신
  - 프로세스간 통신의 개념
  - 프로세스간 통신의 적용
  - 실습
      - 파이프(PIPE) 기반 프로세스간 통신
      - 파이프(PIPE) 기반 프로세스간 양방향 통신
      - 파이프를 두 개 생성하여 프로세스간 양방향 통신
      - 메시지를 저장하는 형태의 에코 서버
      
<br/>

## 12. IO 멀티플렉싱
  - IO 멀티플렉싱 기반의 서버
  - select 함수의 이해와 서버의 구현
  - 실습
      - select 함수 호출
      - 멀티플렉싱 서버 구현
      
<br/>

## 13. 다양한 입출력 함수
  - send & recv 입출력 함수
  - readv & writev 입출력 함수
  - 실습
      - MSG_OOB 긴급 메시지 전송
      - 입력버퍼 검사하기
      - readv & writev 함수 사용
      
<br/>

## 14. 멀티캐스트 & 브로드캐스트
  - 멀티캐스트
  - 브로드 캐스트
  - 실습
      - 멀티캐스트 sender, receiver 구현
      - 브로드캐스트 sender, receiver 구현

      
<br/>

## 15. 소켓과 펴준 입출력
  - 표준 입출력 함수의 장점
  - 표준 입출력 함수 사용하기
  - 실습
      - 표준 입출력 함수와 시스템 함수의 성능비교
      - fileno 함수를 이용한 파일 디스크립터로 변환
