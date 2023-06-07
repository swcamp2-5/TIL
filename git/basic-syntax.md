# Git

## 버전 관리란?

“버전 관리” 는 무엇이고 우리는 왜 이것을 알아야 할까? 버전 관리 시스템은 파일 변화를 시간에 따라 기록했다가 나중에 특정 시점의 버전을 다시 꺼내올 수 있는 시스템이다. 이 책에서는 버전 관리하는 예제로 소프트웨어 소스 코드만 보여주지만, 실제로 거의 모든 컴퓨터 파일의 버전을 관리할 수 있다.

## 분산 버전 관리 시스템(DVCS)

![distributed](./assets/distributed.png)

## 세 가지 상태

![areas](./assets/areas.png)


## 명령어

```shell
git init
```
- `init` : .git directory를 생성하기 위한 명령어


```shell
git add <filename>
git add <foldername>
git add .
```
- `add` : `working Directory` 에서 `Staging Area(Index)`로 추가
    - `.`은 현재폴더의 모든 폴더, 파일을 의미

```shell
git commit -m "message"
```

- `commit` : `Staging Area`에 올라간 파일들의 스냅샷을 찍어 `.git directory`에 저장 
    - 일반적으로 `-m` 옵션을 이용하여 커밋메세지를 같이 등록

```shell
git remote add origin https://github.com/sample.git
```

- `remote` : 원격저장소주소를 추가한다 origin이라는 별명으로, 실제주소는 `https://....`이다.


```shell
git push origin master
```

- `push` : 업로드한다 origin이라는 원격저장소로 master를