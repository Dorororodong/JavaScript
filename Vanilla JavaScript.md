## Vanilla JavaScript

브라우저(매끈한 면)

HTML (접착제)

CSS와 JS (짜잔)

---

const (변하지 않는)

```javascript
const myName = 'June';
// camelCase
```

---

let (변할 수 있는)

```javascript
let myName = 'June';
.
.
.
myName = 'JuneJune';
```

**const `항상`**

**let `가끔`**

**var `절대X`**

---

= true 켜짐

= false 꺼짐

= null 비어있음

```javascript
let something;
// undefined 메모리에 변수는 만들어졌고 컴퓨터가 이 변수에 대해서 인지하고 있는데, 값이 없음
```

---

```javascript
const daysOfWeek = ['mon', 'tue', 'wed', 'thu', 'fri', 'sat' ];

// Get Item from Array
console.log(daysOfWeek); 

// Add one more day to the array
daysOfWeek.push('sun');

console.log(daysOfWeek);

console.log(daysOfWeek[12345]);
// undefined
```

---

### Object : property를 가진 데이터를 저장하도록 해줌

```javascript
const player = {
  name: 'June',
  points: 123,
  fat: true,
};
console.log(player);
console.log(player.name);
console.log(player['points']);

player.fat = false;
player.lastName = 'Hou';
player.points = player.points + 12;
console.log(player);
// player 자체를 통으로 바꾸는게 아니라 그안(object)의 무언가를 업데이트 하는 것이어서 문제 X
// 추가하고 싶으면 그냥 작성해주면 됨
```

---

### Function

```javascript
function sayHello(nameOfPerson, age) {
  console.log("Hello my name is " + nameOfPerson + " and I'm " + age);
};

sayHello('June', 234)

const player2 = {
  name: 'niconiconi',
  sayHello: function (otherPersonName) {
    console.log('hello ' + otherPersonName + ' nice to meet you!');
  },
};

console.log(player2.name);
player2.sayHello('muyaho');
```

---

### Conditionals

```javascript
const age1 = prompt('How old are you?');
const age2 = parseInt(prompt('How old are you?'));
// 구식이라 쓰지 않음(prompt), 디자인 변경도 안되고 딱딱함!

console.log(age2);

console.log(typeof age1);

console.log(age1, parseInt(age1));

console.log(isNaN(age1));

if (isNaN(age1) || age1 < 0) {
  console.log('Please write a real positive number');
} else if (age1 < 18) {
  console.log('You are too young!');
} else if (age1 >= 18 && age1 <= 50) {
  console.log('You can drink!');
} else {
  console.log("You can't drink!");
}

// === (같다면)
// !== (같지 않다면)
```

---

### The Document Object

![image-20220108011324342](Vanilla JavaScript.assets/image-20220108011324342.png)

![image-20220108011633088](Vanilla JavaScript.assets/image-20220108011633088.png)
