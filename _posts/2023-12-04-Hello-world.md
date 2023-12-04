---
title: Java Hello, world 출력하기
author: hmmi
date: 2023-12-04 21:30
categories: [개발언어,Java]
tags: [개발언어,Java]
pin: true
toc: true
toc_sticky: true
---

## 소스

```java
class Hello{
	public static void main(String[] args){
		System.out.println("Hello, world."); // 화면에 글자를 출력
	}
}
```

## 실행 순서

1. Hello.java 작성
2. javac로 컴파일
3. Hello.class 생성
4. java로 실행
5. "Hello, world." 출력

## 소스 설명

### 클래스

- 모든 소스는 클래스 안에 존재한다.
- 서로 관련된 코드들을 그룹으로 나눠 별도의 클ㄹ스를 구성한다.
- 이 클래스들이 모여 하나의 .java 파일을 이룬다.

```java
class 클래스{
	...
}
```

### main 메서드

- `public static void main(String[] args)` 는 main 메서드의 선언부이다.
- java 인터프리터에게 호출될 수 있게 미리 약속된 부분이라 똑같이 작성.
- main 메서드의 중괄호 안의 코드를 마치면 java 애플리케이션은 종료된다.
- 하나의 java 애플리케이션은 바나의 하나 이상의 main 메서드를 포함한 클래스가 있어야 한다.

```java
class 클래스 이름{
	public static void main(String[] args){
		...
	}
}
```

## public 클래스는 하나만 존재해야 한다.

- 하나의 소스파일에 둘 이상의 클래스 정의도 가능하다.
- public 클래스는 하나만 존재할 수 있다.
- public 클래스의 이름과 소스파일명은 동일해야 한다.
- public 클래스가 없다면 소스파일명은 어떤 클래스명으로 해도 괜찮다.

```java
// 올바른 예
// java1.java
public class java1{}
class java2{}

// java1.java
class java1{}
class java2{}

// 틀린 예
// java1.java
// public 클래스가 두 개.
public class java1{}
public class java2{}

// java3.java
// public 클래스와 소스파일이 동명이 아님.
public class java1{}
class java2{}

// Java1.java
// public 클래스와 소스파일이 동명이 아님. (대소문자 구분)
public class java1{}
class java2{}
```

- 단, 클래스를 한 파일에 여러 개 만들 경우 각 클래스 명으로 .class 파일이 생성된다.
