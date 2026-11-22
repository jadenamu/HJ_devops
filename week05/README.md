-5주차 도커

-VM과 도커의 차이: VM은 호스트 OS위에 각각의 격리 공간마다 게스트OS를 깔아 사용한다. 반면 도커는 하나의 호스트OS로 필요한만큼만 격리시켜 VM에 비해 가볍고 효율적.
-이미지와 컨테이너: 이미지는 컨테이너를 만들기 위한 일종의 붕어빵 틀. 이미지 안에는 프로그램 실행에 필요한 파일과 설정등이 포함된다. 컨테이너는 이미지를 통해 탄생한 붕어빵.
-실습 내용: docker를 다운받아 ngnix이미지를 이용해 컨테이너를 생성하고, 수정하고, 삭제했다. docker 실습을 GitHub ISSUE로 정의했다.

curl 8091:	
  HTTP/1.1 200 OK
  Server: nginx/1.31.6
  Date: Sun, 22 Nov 2026 05:26:35 GMT
  Content-Type: text/html
  Content-Length: 28
  Last-Modified: Sun, 22 Nov 2026 05:21:17 GMT
  Connection: keep-alive
  ETag: "6b027bcd-1c"
  Accept-Ranges: bytes

curl 8092:
  HTTP/1.1 200 OK
  Server: nginx/1.31.6
  Date: Sun, 22 Nov 2026 05:28:25 GMT
  Content-Type: text/html
  Content-Length: 31
  Last-Modified: Sun, 22 Nov 2026 05:22:49 GMT
  Connection: keep-alive
  ETag: "6b027c29-1f"
  Accept-Ranges: bytes

curl 8093:
  HTTP/1.1 200 OK
  Server: nginx/1.31.6
  Date: Sun, 22 Nov 2026 05:30:03 GMT
  Content-Type: text/html
  Content-Length: 32
  Last-Modified: Sun, 22 Nov 2026 05:23:34 GMT
  Connection: keep-alive
  ETag: "6b027c56-20"
  Accept-Ranges: bytes
