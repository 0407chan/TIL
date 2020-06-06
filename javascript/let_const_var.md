# var
- var는 es6 이전 문법
- block scope 적용되지 않는다.
```javascript
{
  var x = "hello world"
}
console.log(x) // hello world가 찍힌다.

```
# let
- let은 es6 문법
- block scope 가 **적용** 된다.
- let으로 선언한 변수는 수정 **가능** 하다.
```javascript
{
  let x = "hello world"
}
console.log(x) //아무것도 찍히지 않는다.
```

- var와 let은 이런 차이가 존재한다. let은 block scope가 적용 되어 해당 블럭 안에서만 사용 할 수 있다.

```javascript
var i = 5;
for(var i =0; i< 10; i++){
  //작업
}
console.log(i) // i = 10 이된다.

let i = 5;
for(let 1 = 0 i< 10; i++){
  //작업
}
console.log(i) // i = 5이다.
```
- 이 예제에서 봐도 var 는 블럭에 상관없이 새로 선언하고 값을 주는 것이 다 반영된다.
- let은 block 밖에서 선언한 let i, 그리고 for문 안에서 선언한 let i가 block scope가 적용된다. for문이 끝나고 i를 출력하면 처음에 선언한 5가 출력된다. 

# const
- const는 es6 문법
- block scope 가 **적용** 된다.
- const로 선언한 변수는 수정 불가능 하다.
```javascript
const x = 5;
x = 10; // 에러가 난다.
```
