# git

## 버전 관리란?
“버전 관리” 는 무엇이고 우리는 왜 이것을 알아야 할까? 버전 관리 시스템은 파일 변화를 시간에 따라 기록했다가 나중에 특정 시점의 버전을 다시 꺼내올 수 있는 시스템이다. 이 책에서는 버전 관리하는 예제로 소프트웨어 소스 코드만 보여주지만, 실제로 거의 모든 컴퓨터 파일의 버전을 관리할 수 있다.

## 분산 버전 관리 시스템 (DVCS)

![DVCS](./assets/distributed.png)

## 세가지 상태

![areas](./assets/areas.png)

## 명령어

```shell
git init
```
- `.git directory`를 생성하는 명령어




```shell
git add .
```

- `working directory`에 있는 파일, 폴더를 `staging area`에 추가
- add 하기전엔 파일이 저장이 되었는지 확인하기



```shell
git commit -m 'message'
```

- `staging area`에 올라간 파일들을 저장



```shell
git remote add origin <remoteurl>
```

- 원격저장소 주소를 `origin`이라는 별명으로 저장



```shell
git push origin master
```

- `master` 브랜치를 `origin` 원격저장소로 업로드




# 2023-07-25

```shell
git clone <remote url>
```

- 원격 저장소에 있는 레포를 현재 폴더에 복제



```shell
git pull origin master
```
- 원격 저장소에 마지막 코드 상태를 다운로드



branch 관련

```shell
git branch
```

- branch의 위치를 확인



```shell
git branch -c ~~~
```

- branch 생성



```shell
git branch switch ~~~
```

- ~~~로 이동



```shell
git push origin master ~~~
```

- master로 push


그 후 pull request 기능과 fork 기능으로 기여하는 것에 대해 배움