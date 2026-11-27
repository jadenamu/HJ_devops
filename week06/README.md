-6주차 도커파일 및 ghcr 배포

-이미지 주소: v1: ghcr.io/jadenamu/guestbook:v1
	      v2: ghcr.io/jadenamu/guestbook:v2

-방명록 커스터마이징: dockerfile의 APP_TITLE, THEME_COLOR를 수정하고, index.html의 안내 문구를 수정했다

-교수님 이미지 실행 결과: dockerfile.custom을 작성하여 교수님 이미지를 기반으로 새로운 이미지를 생성

-docker 명령어:
  -FROM: 기반 이미지를 지정
  -WORKDIR: 이미지 내부의 작업 디렉터리 설정
  -COPY: 호스트의 파일을 이미지 내부로 복사
  -RUN: 이미지 빌드 과정에서 명령어를 실행
  -ENV: 이미지에 환경변수를 설정
  -EXPOSE: 컨테이너가 사용하는 포트 정보를 명시
  -CMD: 컨테이너 실행 시 기본적으로 실행할 명령어 지정
