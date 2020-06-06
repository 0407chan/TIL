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

# const
- const는 es6 문법
- block scope 가 **적용** 된다.
- const로 선언한 변수는 수정 불가능 하다.
```javascript
const x = 5;
x = 10; // 에러가 난다.
```
