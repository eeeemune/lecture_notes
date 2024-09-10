[0_2_Git 소개 및 버전 관리.pdf](https://prod-files-secure.s3.us-west-2.amazonaws.com/a4573303-efcb-4d09-951c-bb564c5fbb6e/18452c7a-4860-4cd7-9799-2df820bbaea0/0_2_Git_%EC%86%8C%EA%B0%9C_%EB%B0%8F_%EB%B2%84%EC%A0%84_%EA%B4%80%EB%A6%AC.pdf)

<aside>

# Git 소개 및 버전 관리

</aside>

## Git 소개

<aside>

**Git**

소스 코드를 효율적으로 관리하고 협업하기 위한 툴

</aside>

- 리눅스의 창시자인 리누스 토발즈가 만들었다고 한다,,,

## Git과 GitHub

![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/a4573303-efcb-4d09-951c-bb564c5fbb6e/9c0bfda3-a1b4-4a1a-a5b2-dc886d5aa5b1/image.png)

### Git과 GitHub의 차이

- 김영호 교수님께서 강조해 달라고 부탁했다고 말씀하심

| Git | GitHub |
| --- | --- |
| 소프트웨어 | 웹 서비스 |
| 소스코드 관리를 위해 사용 | Git 저장소를 호스팅하기 위해 사용 |
| 로컬 환경에서 사용 | 웹 상에서 활용 |
| CLI 환경 | GUI 환경 |

## Git을 사용하면 유리한 점

### 버전관리

- 새로 기능을 추가할 때는 이전 버전을 저장해 둘 필요가 있다.
- 이 때 새로운 파일을 copy해서 만들곤 하는데, 이건 좀,,, 짜친다.
- 소스코드의 현재 상태를 버전으로 관리할 수 있게 하는 것이 Git

### 백업

- 에러 등을 대비해 소스코드를 백업해 두어야 함
- 이 때 GitHub에 Git repository를 Hosting해서 소스를 백업해 둠

### 협업

- GitHub를 활용하면 여러 명의 개발자가 협업 가능함
- 네트워크 방식이므로 쉽게 접근 가능
- 버전이 남기 때문에 쉽게 관리 가능

<aside>

# Git 버전 관리

</aside>

## Git이 저장소를 관리하는 방법

- 시험에 나올 가능성이 높다고 말씀하심

![image.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/a4573303-efcb-4d09-951c-bb564c5fbb6e/44a7aa46-9f9a-44b5-81db-7eadf78c6c44/image.png)

### Working tree

소스코드를 직접 수정 및 저장

### Stage

버전관리를 수행할 대상 이 되는 파일들이 모인 공간

### Repository

각 버전이 저장되어 있는 공간. 저장소라고도 한다. 

![이 그림을 기억하라고 말씀하신다… Git 버전 관리에서 시험이 출제된다면 여기서 출제된다고 말씀하심.](https://prod-files-secure.s3.us-west-2.amazonaws.com/a4573303-efcb-4d09-951c-bb564c5fbb6e/77bdb9cc-1e1c-467d-b2bc-2ba863fa2f50/image.png)

이 그림을 기억하라고 말씀하신다… Git 버전 관리에서 시험이 출제된다면 여기서 출제된다고 말씀하심.

## Stage 공간의 필요성

- 이 부분도 시험에 나올 수 있다고 하심.

### 1. 수정된 부분 중 일부분만 commit 가능

일부 파일은 수정이 완료되고 일부는 아직 수정 중일 때 , 특정 파일만 골라서 commit 할 수 있음.

### 2. commit 전 코드 리뷰 및 테스트 가능

commit 전에 stage 공간의 코드들을 이용하여 테스트를 진행 하고 문제 없을 시 commit 하는 방식으로 실수가 포함된 commit 을 줄일 수 있음