# JitPack 배포

## JitPack ?

안드로이드, JVM의 오픈소스 라이브러리 배포 플랫폼이다.

## JitPack의 사용 방법

### 라이브러리 생성

1. 새로운 모듈을 추가한다
    1. 만들 라이브러리를 구현한다
    2. 만들 라이브러리 모듈의 build.gradle 전역 스코프에 다음과 같은 코드를 추가한다
        
        `group = 'com.github.{github nickname}'`
        
2. github에 프로젝트를 push한다

### 라이브러리 github에 배포

- 리포지토리의 릴리즈 기능을 통하여 추적할 수 있는 태그를 부착한 후 배포한다
    - 태그는 버전 등을 예로 들 수 있다
- [https://jitpack.io/](https://jitpack.io/) 접속하여 유효성을 확인한다
    - 정상적으로 이용 가능한 라이브러리는 초록색 로그가 표시된다
        - 반대의 경우 빨간색 로그가 표시된다
    - 해당 사이트에서 제공하는 라이브러리 의존성을 추가한다

### JitPack 라이브러리 사용

1. 프로젝트의 build.gradle에 다음과 같은 코드를 추가한다
    
    `maven { url "[https://jitpack.io](https://jitpack.io/)" }`
    
2. [https://jitpack.io/](https://jitpack.io/에서) 에서 해당 라이브러리의 implementation 코드를 제공받을 수 있다

---

- 참고 자료
    - [https://docs.jitpack.io/](https://docs.jitpack.io/)
    - [https://selfish-developer.com/entry/jitpack-이란](https://selfish-developer.com/entry/jitpack-%EC%9D%B4%EB%9E%80)
