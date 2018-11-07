### ES6(ES2015)-IE10+、Chrome、Fireox、移动端、NodeJS

#### 编辑、转换
- 1.在线转换（browser.js）
- 2.提前编译（支持）

babel==browser.js

------------------------------------------------------------------------------------

#### ES6.0：
- 1.变量/赋值
- 2.函数
- 3.数组/json
- 4.字符串
- 5.面向对象
- 6.Promise(异步交互)
- 7.generator(同步操作拆成异步操作)
- 8.模块化
------------------------------------------------------------------

#### var：
- 1.可以重复生命
- 2.无法限制修改
- 3.没有块级作用于

- let      不能重复声明， 变量-可以修改，块级作用于
- const    不能重复声明， 变量-不能修改，块级作用于
------------------------------------------------------------------



#### 函数-箭头函数:
var show = function (a) {};
let show = a=>{};
- 1.如果只有一个参数，()可以省掉；
- 2.如果只有一个return, {}可以省掉；

函数-参数：



函数-解构赋值：
- 1.左右俩别结构必须一样；
  - let [{a,c},[n1,n2,n3],num,str] = [{a:12,c:13},[1,2,3],0,'hhh'] //ok
  - let [obj,array,num,str] = [{a:12,c:13},[1,2,3],0,'hhh'] //ok
- 2.右边必须是个东西；
  - let {a,b} = {12,13} //no,右边不是个东西啊，json不是，数组不是
- 3.声明和赋值不能分开（必须在一句话里面实现）；
  - let [a,b];
  - [a,b] = [1,2] //no,不可分开啊大哥
------------------------------------------------------------------



#### 数组：
- map        映射           一个对一个
- reduce     汇总           一堆出来一个
- filter     过滤器         消失一部分留一部分
- forEach    循环（迭代）
------------------------------------------------------------------



#### 字符串：
- 1.多了两个新方法 
  - startsWith
  - endsWith
- 2.字符串模板，字符串连接
  - 直接把东西塞到字符串里面   ${东西}
  - 可以折行
------------------------------------------------------------------
  


#### 面向对象：
- 1.class关键字、构造器和类分开了；
- 2.clss里面直接加方法；
#### 继承：
  super - 超类 = 父类
#### 应用：
  react 1.组件化-class;2.JSX(JSX==babel==browswe.js)
------------------------------------------------------------------





#### JSON对象：
  JSON.stringify()    字符串化 
  JSON.parse() 
  标准写法：只能用双引号；所有的名字都必须用引号包起来
  <p>{a: 12, b: 5}          × </p>
  <p>{'a': 12, 'b': 5}      √ </p>
  <p>{a:'abc', b: 5}        × </p>
  <p>{"a": "abc", "b": 5}   √ </p>
  简写：名字与值一样的话，留一个就行；function可以删掉 
------------------------------------------------------------------





#### promise - 承诺

- 异步：操作跟操作之间没啥关系，同时进行多个操作（代码更复杂）
- 同步：同时只能做一件事（代码简单）
<pre>var promise = new Promise(function(resolve, reject) { 
  if (/* 异步操作成功 */){ 
    resolve(value); 
  } else { 
    reject(error); 
  } 
}); </pre>
<pre>promise.then(function(value) { 
 // success 
}, function(value) { 
 // failure 
}); </pre>
<pre>Promise.all([

]).then(function() {

},function () {

});</pre> 
<p>Promise.race      竞速（同时都去5个，哪个快哪个先来） </p>
------------------------------------------------------------------





#### generator - 生成器(generator函数可以走走停停，啥时候想走就走；普通函数就是一路走到底) 
#### generat - 生成 
#### yield - 放弃 
------------------------------------------------------------------




#### yield传参、返回

- 1.yield可以传参 
<p>最后步骤需要return </p>
- 2.yield返回 
------------------------------------------------------------------





#### runner
<p>KOA基于Node.js平台下一代web开发框架</p>
