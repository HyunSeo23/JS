# 2025-04-25 - JavaScript 조건문 정리

## 조건문 (Conditional Statement)

조건문은 주어진 조건에 따라 코드 블록을 실행할지 결정하는 문법이다.  
프로그램 흐름을 제어할 때 필수적으로 사용된다.

---

## 1. if문

가장 기본적인 조건문. 조건이 `true`일 때만 코드 블록을 실행한다.

```javascript
let num = 10;

if (num > 5) {
  console.log("num은 5보다 큽니다.");
}
```

### if - else

조건이 `false`일 때 실행할 코드를 추가할 수 있다.

```javascript
let num = 3;

if (num > 5) {
  console.log("num은 5보다 큽니다.");
} else {
  console.log("num은 5 이하입니다.");
}
```

### if - else if - else

여러 조건을 차례로 검사할 때 사용한다.

```javascript
let score = 85;

if (score >= 90) {
  console.log("A");
} else if (score >= 80) {
  console.log("B");
} else if (score >= 70) {
  console.log("C");
} else {
  console.log("F");
}
```

---

## 2. switch문

여러 경우(case)를 분기 처리할 때 사용하는 조건문.  
비교 대상이 명확할 때 유용하다.

```javascript
let day = 2;

switch (day) {
  case 1:
    console.log("월요일");
    break;
  case 2:
    console.log("화요일");
    break;
  case 3:
    console.log("수요일");
    break;
  default:
    console.log("목요일 이후");
    break;
}
```

- `break`를 쓰지 않으면 다음 case로 넘어가는 "fall-through" 현상이 발생한다.
- `default`는 모든 case가 해당되지 않을 때 실행된다.

---

## 3. 삼항 연산자 (Ternary Operator)

간단한 조건식을 한 줄로 표현할 수 있다.  
형식: `조건 ? 참일 때 값 : 거짓일 때 값`

```javascript
let age = 18;
let access = age >= 18 ? "입장 가능" : "입장 불가";

console.log(access);
```

---

# ✨ 정리

- **if문** : 기본 조건 분기
- **if-else** : 참/거짓 두 갈래
- **if-else if-else** : 여러 조건 분기
- **switch문** : 여러 값 비교할 때 깔끔
- **삼항 연산자** : 간단한 조건식을 한 줄로

---
