一，new和Object.create()的区别
1，new的实现：
var o1 = new Base()

JavaScript 实际上执行的是：
（1）var o1 = new Object();
（2）o1.[[Prototype]] = Base.prototype;
（3）Base.call(o1);

2，Object.create()实现
Object.create =  function (o) {
    var F = function () {};
    F.prototype = o;
    return new F();
};

3，区别
比较     | new                   | Object.create
构造函数 |保留原构造函数属性       |丢失原构造函数属性
原型链   | 原构造函数prototype属性|原构造函数/（对象）本身
作用对象 |	function             |function和object
