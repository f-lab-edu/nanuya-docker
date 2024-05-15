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