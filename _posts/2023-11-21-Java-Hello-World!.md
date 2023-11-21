---
title: Java Hello World!
author: hmmi
date: 2023-11-21 16:11
categories: [개발 언어,Java]
tags: [개발 언어,Java]
pin: true
toc: true
toc_sticky: true
---

자바에는 Main 클래스와, main 메소드가 필수적이다. Main 클래스는 클래스 파일 명(.java)와 일치시켜야 하고, main 메소드 명은 main이다.

## Main 클래스

- 자바는 Main 클래스부터 시작하기 때문에, 꼭 필요한 클래스다.
- Main 클래스의 클래스 명은 파일명 (.java)와 일치시킨다.

```java
public class Main {
	public static void main(String[] args) {
	// write your code here
	System.out.println("Hello Wolrd");
	}
}
```

## main 메소드

- main 메소드 또한 클래스에 꼭 필요한 요소

이 코드는 자바 프로그램에서의 진입점(entry point)을 나타내는 메소드입니다. 여기서 `main` 메소드는 프로그램이 시작될 때 처음으로 실행되는 부분

이 메소드는 다음과 같은 구조를 가지고 있다.

```java
public static void main(String[] args) {
    // 프로그램의 시작 부분
    // 코드 작성
}
```

**간단한 설명**

- `public`: 이 메소드가 어디에서나 접근 가능하다는 의미
- `static`: 해당 메소드가 특정 인스턴스에 속하지 않고 클래스 자체에 속해 있다는 의미
- `void`: 이 메소드가 값을 반환하지 않는다는 의미
- `main`: 이 메소드의 이름이며, Java 프로그램이 시작될 때 시스템에 의해 자동으로 호출
- `String[] args`: 문자열 배열 파라미터로, 프로그램을 실행할 때 전달되는 명령행 인수(arguments)를 저장
