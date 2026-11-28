-7주차 docker compose

-docker compose 실행 결과: docker compose를 이용해서 Reid 컨테이너 1개, Web 컨테이너 3개, Nginx 컨테이너 1개를 실행하였다.
docker compose up -d --scale web=3
docker compose ps

NAME                STATUS
guestbook-nginx-1   Up 4 seconds
guestbook-redis-1   Up 15 seconds (healthy)
guestbook-web-1     Up 9 seconds (healthy)
guestbook-web-2     Up 9 seconds (healthy)
guestbook-web-3     Up 9 seconds (healthy)

-redis와 web 컨테이너가 모두 healty 상태인 것을 확인하였다.

-docker compose down 후 up: docker compose down은 컨테이너와 프로젝트 네트워크를 제거하지만, redis-data 볼륨은 제거하지 않는다. 따라서 컨테이너를 다시 생성하더라도 기존 방명록 데이터가 유지된다.

-docker compose down -v 후 up: docker compose down -v는 컨테이너와 네트워크뿐만 아니라 Compose에서 관리하는 redis-data 볼륨도 제거한다. 따라서 다시 생성하면 기존 방명록 데이터가 사라진다.

-.env 파일을 git에 올리지 않는 이유: .env 파일에는 redis 비밀번호, api 키 등 민감한 정보가 포함되어 github에 업로드하지 않는다. 따라서 .gitignore에 .env를 추가하여 git의 추적에서 벗어난다.

