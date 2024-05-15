# 도커 사용해보기

## 도커 이미지 만들기

```shell
$ yarn create next-app --typescript

$ yarn build

$ touch Dockerfile

# bm-first-app 이라는 태그로 이미지 빌드
$ docker image build -t bm-first-app

# 컨테이너 실행해보기
$ docker container run -d -p 3000:80 bm-first-app
```

> Q) 컨테이너 실행해보기 했을 때 아무 오류 발생하지 않고 yarn start 까지 정상적으로 실행됨. 하지만 http://localhost:3000 으로 접근 시 "사이트에 연결할 수 없음" 뜨고 "http://localhost:3000:80" 으로 접근 시 구글 검색화면으로 연결됨 ㅠㅠ

## 애플리케이션 실행하기

```shell
# dev mode
$ yarn
$ yarn dev

# prod mode
$ yarn
$ yarn build
$ yarn start
```