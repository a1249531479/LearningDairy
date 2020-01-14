# 第二天

### JavaScript

1、在标签中填写 onclick 事件调用函数时，不是 onclick=函数名， 而是 onclick=函数名+()，代码如下：

<script> 
    function myfunction(){
         document.getElementById("demo").innerHTML="onclick事件触发";
        }</script>
    </head>
<body>
    <h1 id="demo">一个段落</h1>
    <button onclick="myfunction()" type="button">点击这里</button>
</body>
2、外部 javascript 文件不使用 <script> 标签，直接写 javascript 代码。

3、HTML 输出流中使用 document.write，相当于添加在原有html代码中添加一串html代码。而如果在文档加载后使用（如使用函数），会覆盖整个文档。

使用函数来执行document.write代码如下：

<script>
function myfunction(){
    document.write("使用函数来执行doucment.write，即在文档加载后再执行这个操作，会实现文档覆盖");
}
document.write("<h1>这是一个标题</h1>");
document.write("<p>这是一个段落。</p>");
</script>
<p >
您只能在 HTML 输出流中使用 <strong>document.write</strong>。
如果您在文档已加载后使用它（比如在函数中），会覆盖整个文档。
</p>
<button type="button" onclick="myfunction()">点击这里</button>



JavaScript 显示数据
JavaScript 可以通过不同的方式来输出数据：

使用 window.alert() 弹出警告框。
使用 document.write() 方法将内容写到 HTML 文档中。
使用 innerHTML 写入到 HTML 元素。
使用 console.log() 写入到浏览器的控制台。



document.getElementById("demo") 是使用 id 属性来查找 HTML 元素的 JavaScript 代码 。

innerHTML = "段落已修改。" 是用于修改元素的 HTML 内容(innerHTML)的 JavaScript 代码。



### JavaScript 变量

在编程语言中，变量用于存储数据值。

##### JavaScript 使用关键字 var 来定义变量， 使用等号来为变量赋值：

var x, length

x = 5

length = 6

##### 变量可以通过变量名访问。在指令式语言中，变量通常是可变的。字面量是一个恒定的值。


var length = 16;                                  // Number 通过数字字面量赋值 
var points = x * 10;                              // Number 通过表达式字面量赋值
var lastName = "Johnson";                         // String 通过字符串字面量赋值
var cars = ["Saab", "Volvo", "BMW"];              // Array  通过数组字面量赋值
var person = {firstName:"John", lastName:"Doe"};  // Object 通过对象字面量赋值





##### 数字（Number）字面量 可以是整数或者是小数，或者是科学计数(e)。

3.14

1001

123e5

##### 字符串（String）字面量 可以使用单引号或双引号:

"John Doe"

'John Doe'


表达式字面量 用于计算：

5 + 6

5 * 10

#### 数组（Array）字面量 定义一个数组：

[40, 100, 1, 5, 25, 10]
对象（Object）字面量 定义一个对象：

{firstName:"John", lastName:"Doe", age:50, eyeColor:"blue"}
函数（Function）字面量 定义一个函数：

function myFunction(a, b) { return a * b;}



#### JavaScript事件

------

 

HTML 事件是发生在 HTML 元素上的事情。

 

当在 HTML 页面中使用 JavaScript 时， JavaScript 可以触发这些事件

事件可以用于处理表单验证，用户输入，用户行为及浏览器动作:



## HTML 事件

 

 HTML 事件可以是浏览器行为，也可以是用户行为。

 

以下是 HTML 事件的实例：

 

-  HTML 页面完成加载
-  HTML input 字段改变时
-  HTML 按钮被点击





 **JavaScript 可以做什么?**

- 页面加载时触发事件
- 页面关闭时触发事件
- 用户点击按钮执行动作
- 验证用户输入内容的合法性

# JavaScript 对象



JavaScript 对象是拥有属性和方法的数据。

一辆汽车是一个对象。 

 

对象有它的属性，如重量和颜色等，方法有启动停止等:

所有汽车都有这些属性，但是每款车的属性都不尽相同。

 所有汽车都拥有这些方法，但是它们被执行的时间都不尽相同。

## 对象属性

 

可以说 "JavaScript 对象是变量的容器"。

 

但是，我们通常认为 "JavaScript 对象是键值对的容器"。

 

键值对通常写法为 **name : value** (键与值以冒号分割)。

  

键值对在 JavaScript 对象通常称为 **对象属性**。



对象键值对的写法类似于：

- Python 中的字典
- C 语言中的哈希表

## 对象方法

  

对象的方法定义了一个函数，并作为对象的属性存储。 

 

对象方法通过添加 () 调用 (作为一个函数)。