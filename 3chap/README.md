# Docker에서 'Hello world'

## docker container run 명령

```bash
docker container run <Docker 이미지명> <실행할 명령>
```

1. docker container run -> 컨테이너를 작성 및 실행
2. \<Docker 이미지\> -> 바탕이 되는 Docker 이미지
3. \<실행할 명령\> -> 컨테이너 안에서 실행할 명령

## Hello world의 실행

```bash
docker container run ubuntu:latest /bin/echo 'Hello world'
```

## Docker 버전 확인

```bash
docker version
```

## Docker 실행 환경 확인

```bash
docker system info
```

## Docker 디스크 이용 상황

```bash
docker system df
```

## Docker 이미지 다운로드

ngnix 다운

```bash
docker pull ngnix
```

## Docker 이미지 확인

```bash
docker image ls
```

## Nginx 작동

```bash
docker container run --name webserver -d -p 80:80 nginx
```

## ngnix 서버 상태 확인

```bash
docker container ps
```

## 컨테이너 가동 확인

```bash
docker container stats webserver
```

## 컨테이너 정지

```bash
docker container stop webserver
```
