# 第一题

请给出如下代码的打印结果（答案在最下面）：

```js
function Foo() {
    Foo.a = function() {
        console.log(1)
    }
    this.a = function() {
        console.log(2)
    }
}
Foo.prototype.a = function() {
    console.log(3)
}
Foo.a = function() {
    console.log(4)
}
Foo.a();
let obj = new Foo(); 
obj.a();
Foo.a();
```



















打印结果： 4 2 1
