# 前段笔记
---
### javascript的基础<br>
#### 概述<br>
学习所有编程语言编写第一个程序的时候，都习惯性地编写“hello world”程序，学习JavaScript也是一样。作为我们编写的第一个JavaScript程序，我们将代码写在html文档中，body标签的结尾处<br>
JavaScript首先要学会使用调试工具中的控制台选项，可以先打开chrome浏览器，然后按F12可以打开调试工具，点击console按钮，可查看控制台信息<br>
#### 变量与数据类型<br>
1. 变量概念：变量可以理解为是存储数据的容器。如代码所示，我们可以通过var声明一个变量，var后面的英文字母就是变量名，变量名是自定义的，在一定的规则下我们可以随意命名<br>
2. 变量包括：字母 数值 下划线 美元符号 年龄用age 价格price<br>
3. "="是赋值的意思<br>
4. 六种数据类型：数字 字符串 布尔 对象 null underfined<br>
5. 四则运算：<br>
var num1 = 10 + 20; 加法
var num2 = 10 - 20; 减法
var num3 = 10 * 20; 乘法
var num4 = 10 / 20; 除法
console.log(num1);
console.log(num2);
console.log(num3);
console.log(num4);<br>
6. 连接字符：<br>
var str1 = "hello";
var str2 = "world";
var str3 = str1 + str2;
console.log(str3)
#### 表达式与运算符<br>
1. 表达式概念:表达式是JavaScript语言中的一个短语，就像我们自然语言中说的一个词或一句话一样。浏览器会将这个短语计算出一个结果，这个结果我们叫它表达式的返回值，下列代码列举了最简单的表达式<br>
2. 运算符概念：运算符可以将简单的表达式连接成复杂的表达式，例如我们上节课学到的字符串连接就是一个带有“+”运算符的表达式。<br>
3. 算术运算符<br>
4. 运算符：加 减 乘 除 求余 自增1 自减1<br>
i  求余表达式的返回值是两个数相除的余数
   var result = 10 % 3;  //10除以3，得3与1 所以10 % 3表达式的值是1；
   console.log(result);  //输出结果为1
ii  自增表达式可以使一个变量在原值的基础上加1
   var num1 = 0;
   num1++;  
   console.log(num);
iii  自减表达式可以使一个变量在原值的基础上减1
   var num2 = 0;
   num2--;
   console.log(num2);<br>
5. 比较运算符：大于 大于等于 小于 小于等于 判断等于 判断不等 判断恒等 判断非恒等<br>
6. 逻辑运算符：逻辑与 逻辑非<br>
7. 赋值运算符：赋值 加并赋值 减并赋值 乘并赋值 除并赋值<br>
#### 条件语句<br>
1. 程序执行顺序有三种：按顺序执行、按条件执行、循环执行，<br>
2. if语句：f语句是最基本的条件控制语句，它让JavaScript程序可以选择执行顺序，我们可以通过一个布尔值来控制一行语句是否执行，if语句有多种形式，<br>
  if(true)  
    console.log("执行代码");
3. 通过控制运算符来实现数学运算<br>
    var num1 = 10;<br>
    var num2 = 20;<br>
    var sign = "+";  //通过修改操作符，输出不同的结果<br>
    var result = 0;  //result用来存储计算的结果，现在设置一个初始值0<br>
    if(sign === "+"){<br>
    result = num1 + num2;<br>
    console.log(result)<br>
}<br>
else if(sign === "-"){<br>
    result = num1 - num2;<br>
    console.log(result)<br>
}<br>
else if(sign === "*"){<br>
    result = num1 * num2;<br>
    console.log(result)<br>
}<br>
else if(sign === "/"){<br>
    result = num1 / num2;<br>
    console.log(result)<br>
}<br>
else{<br>
    console.log("请输入正确的运算符")<br>
}<br>
#### switch语句<br>
 1. 概述：if语句在程序执行的过程中创建一条分支，并且可以使用if...else if...语句来处理多条分支，然而当所有的分支都依赖于同一个表达式的值时，重复计算多条if语句中的条件是非常浪费时间的做法，switch语句正合适处理这种情况<br>
#### 条件运算符<br>
1. 如果是简单的判断，我们可以使用条件运算符：表达式?第一个值:第二个值<br>
2. 如果表达式为true,表达式的返回值是第一个值，如果表达式为false,那么表达式的返回值是第二个值,示例代码如下所示:
   var num1 = 10;<br>
   var num2 = 20;<br>
   var result = num1 > num2 ? 100 : 200;<br>
   //如果num1大于num2，条件表达式的值为100，若num1小于等于num2时，条件表达式的值为200；<br>
   console.log(result);<br>
 #### 循环语句<br>
 1. 概念：条件语句的代码可以被想象成是一条条分支的路径，而循环语句的代码则是程序路径的一个回路，可以让一部分代码重复执行。JavaScript中的循环语句有for语句和while语句。<br>
 ##### for语句<br>
 1. for语句的语法如下：<br>
    for(初始值;布尔值;计数器){<br>
     //语句块<br>
    } <br>
##### while语句<br>
1. while语句语法如下所示：<br>
   while(bool){
    //bool为true,循环执行
}
在每次循环的过程中都会让n的值加1，这样当n的值等于10，循环便停止，下面我来使用while语句输出100以内所有正整数的加和<br>
#### 函数基础<br>
1. 概念：函数是一个可执行的语句块，定义的时候不执行，调用的时候执行，使用"函数名()"的形式可以调用函数<br>
2. function fun(){   <br>
      //定义函数,函数名为fun<br>
      //函数体<br>
   }<br>
   fun();            //调用函数<br>
3. 通过return关键字指定一个返回值，函数有了return，当函数被调用的时候就可以把调用的结果赋值给另一个变量了<br>
#### 对象<br>
1. 对象的基本概念:在现实生活中，所有东西都可以看成对象，比如一台电脑，一个房子，一只猫，一个人，对象有他自己的属性，比如电脑有颜色，房子有尺寸，猫和人多有年龄。<br>
2. 自定义对象:<br>
 我们可以通过一对花括号来创建一个对象:<br>
 var obj = {};<br>


