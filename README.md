# [소검] CTIP 개발 환경 테스트 프로젝트

> 작성자: 전도현(IMRaccoon)

<br />

## 개발 환경

- Oracle JDK 13.0.2
  - [Download](https://www.oracle.com/java/technologies/javase/jdk13-archive-downloads.html)
- Gradle 6.8
  - [Download](https://gradle.org/releases/#6.8)
  - 'binary-only' 로 사용해도 무관합니다.

<br />

## 설치 방법

### Java

#### 1. 다운로드 받습니다.

- 버전 13.0.2 임을 확인합니다.

#### 2. 환경변수를 변경합니다.

- 새로 Java를 받은 경우 설치와 함께 자동으로 세팅되며 3번으로 이동합니다.
- 기존에 설치된 버전이 다른 경우 아래의 순서로 작업을 수행합니다.

```
A. 설치된 Java의 디렉토리를 확인합니다.
(C:\Program Files\Java\jdk13.0.2)
B. Win + Q키를 동시에 누르고 '시스템 환경 변수 편집' 검색
C. 시스템 속성 창의 우측 하단에 '환경 변수' 클릭
D. JAVA_HOME을 A단계에서 확인한 경로로 바꾸어 줍니다.
E. JAVA_PATH를 C:\ProgramData\Oracle\Java\javapath 로 바꾸어줍니다. (해당 경로에 바로가기가 있는 지 확인)
```

#### 3. CMD 에서 `java --version` 입력으로 설치를 확인합니다.

<br />

### Gradle

#### 1. 다운로드 받습니다.

- 버전 6.8을 확인합니다.
- binary-only 의 경우, sample과 docs가 없는 버전입니다.

#### 2. 환경변수를 설정합니다.

```
A. Win + Q키를 동시에 누르고 '시스템 환경 변수 편집' 검색
B. 시스템 속성 창의 우측 하단에 '환경 변수' 클릭
C. 아래의 '시스템 변수'에서 '새로 만들기' 클릭
D. 변수 이름: GRADLE_HOME, 변수 값: 2번의 폴더 경로 입력 후 저장
E. '시스템 변수'에서 'Path' 변수를 누르고 '편집' 클릭
F. 우측 상단의 새로 만들기 후 %GRADLE_HOME%\bin 입력
G. 확인 누르고 나와서 한번 더 확인 누르기
```

#### 3. CMD 에서 `gradle -v ` 입력으로 설치를 확인합니다.
