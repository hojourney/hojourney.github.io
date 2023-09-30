---
layout: default
title: Javascript 기초-바닐라 JS로 크롬 앱 만들기
parent: PM story-tech
nav_order: -8
last_modified_date: 2022-09-25
---
# {{page.title}}
<span style = "color: #A39FAD">Last modified: {{page.last_modified_date}}</span>


Google tag manager에서 심화된 기능을 사용하려면 javascript에 대한 기초지식이 있으면 좋다. 그래서 바닐라 javascript를 학습하기로 마음을 먹고 바로 스타트. [노마드 코더](https://nomadcoders.co/?gclid=CjwKCAjwp9qZBhBkEiwAsYFsb9c91IQPeZtbyq9OsO5MqestIcvZg-ObwWFFK2sn69LCSVPWIdqArRoCaWcQAvD_BwE)에서 무료 강의를 제공한다.

여기서 바닐라 javascript는 완전 순수한 버전의 javascript를 뜻한다.

- Javascript는 기본적으로 camel case를 사용한다. camel case는 myNameIs 처럼 소문자로 시작해서 단어 별로 띄어쓰기가 아닌 대문자로 구분을 하는 것이다. 다른 예로는 파이썬은 기본적으로 my_name_is 처럼 snake case를 사용한다. 

Javascript는 배우고 보니 파이썬이랑 아주 비슷하다는 생각이 든다. 솔직히 그래서 정말 쉽게 느껴졌다. 파이썬을 잊어갈 쯤에 javascript를 배우니 파이썬도 상기되고 javascript도 배우는 일석이조의 느낌.



## 데이터타입
- string: 문자열으로 "안녕" 같은 형태로 사용
- integer: 숫자열으로 13처럼 그냥 숫자를 사용하면 됨(1.5 같은 float 또한 사용 가능)
- boolean: true 나 false 를 지칭하는데 0이랑 1처럼 on/off 같은 게념
- null: variable 안에 아무것도 없다는 것을 지칭할 때 사용(비어있음을 뜻함)
- undefined: value가 없을 때 등장. (undefined는 다른 언어들엔 흔하지 않음. 파이썬에서는 None으로 지칭됨)


## const & let
변수를 설정할 때 var을 사용할 수도 있지만, const와 let을 사용하기를 권장. const는 앞으로 변할 일이 없는 값을 설정할 때 사용되고, let는 변할(update) 수도 있는 값을 위해 사용.
예)
```
const country = "대한민국";
let myAddress = "경기도";
```

let으로 설정한 변수를 업데이트하고자 한다면, 아래처럼 let을 또 사용하지 않아도 됨.
```
let myName = "julie";

myName = "alice";
```

## array
- 요일의 종류처럼 하나의 속성 안에 여러 항목이 들어가야 할 때가 있다. 아래의 형태를 사용하여 array를 생성할 수 있다. 
```
const day = [mon, tue, wed, thu, fri, sat];
```
- 하나를 console에서 호출하고자 한다면 아래처럼 호출할 수 있다.
```
console.log(day[2]);
```
- array 안의 값을 변경하고 싶다면 단순히 아래처럼 변경하면 된다.
```
day[5] = "saturday";
```
- array에 값을 추가하고 싶다면 아래처럼 추가할 수 있다. 추가한 데이터는 array의 가장 끝으로 붙게 된다.
```
day.push("sun");
```

## object
- 하나의 object 아래에 다른 속성들을 하위로 사용하고 싶다면 아래처럼 만들 수 있다.  아래처럼 만들고나면 console.log처럼 object를 만들어냈다고 보면 된다.

``` 
const player = {
	name: "nico", 
	points: 10,
	fat: true,
	
};

console.log(player);
console.log(player.name);
```

- 위와 같은 형태로 사용할 수 있음
- 아래처럼 사용할 수도 있음

```
console.log(player["name"]);
```

- 업데이트 할 수도 있음

```
console.log(player);
player.fat = false;
console.log(player);
```

- constant object의 값은 변경할 수 없지만 constant object 아래에 있는 것은 바꿀 수 있다.
- constant object 아래에 항목(property)을 추가할 수도 있다.

```
player.lastName = "potato";
```

- 혹은 아래처럼 값을 변경할 수도 있다.

```
player.points = player.points + 15;
```
<br><br>

## function
- function의 예시는 `console.log(어쩌구)`.
- function은 반복되는 작업을 한 번에 쉽게 할 수 있도록 하는 기능으로 아래의 예시에서 sayHello를 사용하면 그 안에 있는 것들이 4번 실행되는 것

```
function sayHello(){
	console.log("Hello!");
}

sayHello();
sayHello();
sayHello();
sayHello();
```

<br>
- 하지만, Hello my name is "어쩌구"로 어쩌구만 입력되는 데이터에 따라 계속 바꿔서 호출하고 싶다면? 아래처럼 (괄호) 안에 바꿔줄 argument를 명명해주면 된다.

```
function sayHello(nameOfPerson) {
	console.log(nameOfPerson);
}

sayHello("nico");
sayHello("dal");
sayHello(""lynn);
```

<br>
- argument는 두개를 받을 수도 있다.

```
function sayHello(nameOfPerson, age) {
	console.log("Hello my name is " + nameOfPerson + " and I'm " + age); 
}

sayHello("nico", 10);
sayHello("dal", 23);
sayHello("lynn", 21);
```

<br>
- 계산기를 만들려면 아래처럼 function을 만들 수 있다.

```
function plus(firstNumber, secondNumber) {
	console.log(firstNumber + secondNumber);
}

function divide(a, b) {
	console.log(a / b);
}

plus(60, 8);
divide(98, 20);
```

- object가 console.log("어쩌구")처럼 작동하게 하려면?

```
const player = {
	name: "nico",
	sayHello: function(otherPersonsName) {
		console.log("hello!" + otherPersonsName + "nice to meet you");
	},
};

player.sayHello("lynn");
player.sayHello("nico");
```


## return
- function을 통한 데이터를 밖으로 받아오기 위해 사용(console.log는 alert처럼 일회성 데이터 추출 같은 느낌)

```
const age = 96;
function calculateKrAge(ageOfForeigner) {
	return ageOfForeigner + 2;
}

const krAge = calculateKrAge(age);

console.log(krAge)
```
<br>
- return을 활용한 계산기 만들기

```
const calc = {
	add: function (a, b) {
		return a + b;
	},
	minus: function (a, b) {
		return a - b;
	},
	multiply: function (a, b) {
		return a * b;
	},
	divide: function (a, b) {
		return a / b;
	},	
}

const addResult = calc.add(1, 4);

console.log(addResult);
```

## Conditionals
- if와 else에 대하여..!
```
const age = prompt("How old are you?");

console.log(age);
```

- prompt는 우선 못생겼고, 몇 브라우저는 prompt를 제한하기 때문에 이제 사용하지 않음.
- 아래처럼 typeof를 사용하면 어떤 타입인지 확인할 수 있음
```
const age = prompt("How old are you?");

console.log(typeof age);
```

- parseInt를 사용하면 string(문자)로 들어온 입력값을 int(숫자)로 변경할 수 있다.
```
console.log(typeof "15", typeof parseInt("15"))
```