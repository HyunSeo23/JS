# 📆 2025-04-23 JavaScript TIL - 조건문 & 반복문

## ✅ 조건문 (Conditional Statements)

### 1. if, else if, else

```js
let age = 20;

if (age < 18) {
  console.log("미성년자입니다.");
} else if (age >= 18 && age < 65) {
  console.log("성인입니다.");
} else {
  console.log("노년층입니다.");
}
```

### 2. switch

```js
let fruit = "apple";

switch (fruit) {
  case "apple":
    console.log("사과입니다.");
    break;
  case "banana":
    console.log("바나나입니다.");
    break;
  default:
    console.log("알 수 없는 과일입니다.");
}
```

## 🔁 반복문 (Loops)

### 1. for문

```js
for (let i = 0; i < 5; i++) {
  console.log(`i는 ${i}입니다.`);
}
```

### 2. while문

```js
let count = 0;
while (count < 5) {
  console.log(`count: ${count}`);
  count++;
}
```

### 3. do...while문

```js
let num = 0;
do {
  console.log(`num: ${num}`);
  num++;
} while (num < 5);
```

### 4. for...in (객체용)

```js
const user = { name: "Hyun", age: 25 };

for (let key in user) {
  console.log(`${key}: ${user[key]}`);
}
```

### 5. for...of (배열/이터러블용)

```js
const fruits = ["apple", "banana", "cherry"];

for (let fruit of fruits) {
  console.log(fruit);
}
```

---

📌 **요약**
- 조건문: `if`, `else if`, `else`, `switch`
- 반복문: `for`, `while`, `do...while`, `for...in`, `for...of`
- 상황에 맞는 반복문을 선택해서 쓰는 것이 중요!
