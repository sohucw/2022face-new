# （京东）下面代码中 a 在什么情况下会打印 1？

```js
var a = ?;
if(a == 1 && a == 2 && a == 3){
 	console.log(1);
}
```

解答：

```js
var a = {
  value: 0,

  valueOf() {
    return ++this.value;
  }
};
```