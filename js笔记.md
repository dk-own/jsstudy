# JS

## 初步简介

一个完整的JavaScript应该由下列三个不同的部分组成：
1.核心（ ECMAScript ）　　
2.文档对象模型 （ DOM ）　
3.浏览器对象模型 （ BOM）

ECMAScript是一种由ECMA国际（前身为欧洲计算机制造商协会,英文名称是European Computer Manufacturers Association）通过ECMA-262标准化的脚本程序设计语言。这种语言在万维网上应用广泛，它往往被称为JavaScript或JScript， 但实际上后两者是ECMA-262标准的实现和扩展。

文档对象模型(DOM，Document Object Model)是针对XML但经过扩展用于HTML的应用程序编程接口(API，Application Programming Interface)。DOM有三个级别，每个级别都会新增很多内容模块和标准(有兴趣可以搜索查询)。

访问和操作浏览器窗口的浏览器对象模型(BOM，Browser Object Model)。开发人员使用BOM可以控制浏览器显示页面以外的部分。而BOM真正与众不同的地方(也是经常会导致问题的地方)，还是它作为JavaScript实现的一部分，至今仍没有相关的标准。

<script>标签介绍
<script></script>这组标签，是用于在html页面中插入js的主要方法。它主要有以下几个属性：
1．type：必需。表示代码使用的脚本语言的内容类型。例如：type="text/javascript"。
2．charset：可选。表示通过src属性指定的字符集。
3．defer：可选。表示脚本可以延迟到文档完全被解析和显示之后再执行。
4．src：可选。表示包含要执行代码的外部文件。	
5. async：可选。规定异步执行脚本（仅适用于外部脚本）。

书写js的方法：

1、 行内

2、 内嵌：script标签里面

3、 外部引入

Console：控制台

Console.log()：向web控制台输出一条消息。

Alert()：向web窗口弹出消息。

Debugger：断点查询

 

 

 

## 变量：var，声明/创建一个可以储存数据的容器

​       变量的组成：

1、 字母、数字、下划线、$

2、 不能以数字开头

3、 关键字不能用来当成变量

 

驼峰式命名法 ：

​       user_name

​       username

 

ps：在html标签里面，不区分大小写，但是在js里面，区分大小写

 

关键字：ecma规定了一些单词，这些单词拥有特殊的含义，

保留字：将会成为关键字的单词

运算符：+ - /

赋值运算符：吧右边的值赋予给左边的变量  =

 

## 获取元素/标签

 

1、 通过id获取元素

Document.getElementById();

2、 class是关键字，不能用来找标签的类，通过className来获取。

 

给标签添加事件：

​       标签.onclick = function(){

​              触发行为时执行的代码

​       }

 

## 数据类型：6种数据类型

Ecma规定：

1、 数字类型：0-9  Number

2、 字符串类型：只要被引号包裹的内容就是字符串

3、 布尔类型：Boolean

True：真

False：假

4、 未定义：Undefiend

5、 空：Null

6、 对象类型：复杂数据类型/引用数据类型，可以储存多个数据的类型

1、 数组

写法：2种

​         1、[2,3,4] 每一个数据之间以逗号隔开

​         2、new Array(2,2,2,);

2、 对象

## 流程控制语句：

​       If判断

​              If(判断条件){

​                     代码是否执行,通过判断条件决定

}

判断条件：

​       True：执行

​       False：不执行

判断运算符：比较两个数，得到一个布尔值的结果

\><  >=  <=  !=  ==    ===

​       第二种用法：

​                     If(判断条件){

​                            代码1

}else{

​       代码2

}

​              判断条件：布尔值

​                     True：执行代码1

​                     False：执行代码2

 

 

innerHTML：获取从开始标签到结束标签的所有内容；

​       获取：获取内容

​       设置：把原来的内容覆盖；

​                如果内容里面的值，又像标签的，浏览器就会解析成为标签



Switch判断：

Switch（值）{

​       Break：中断

}

遍历：循环

For（初始变量；判断条件；变量自增）{}：

++：在自身的基础上加1

--：在自身的基础减1

+=：在自身的基础上n

-=：在自身的基础上减n

循环执行的步骤：

​       第一步：先执行声明的变量

第二步：判断条件结果是

​       True：执行花括号里面的所有代码

​       False：循环结束

第三步：让变量加一

第四部：判断条件结果是

##  获取元素

获取元素：通过标签获取元素

​       document.getElementsByTagName(‘标签名’)；

​       结果：是一个类数组，，每个数据就是找到的元素，通过下标可以找到具体的元素

 

获取元素：通过class名获取元素

​       Document,getElementsByClassName(‘class名’)

​       结果：是一个类数组，，每个数据就是找到的元素，通过下标可以找到具体的元素

获取元素的方法：

​       Document.querySelector(css选择器)

 

​       结果：是一个元素，找到的第一个元素

document.querySelectorAll(’.、#、div’)

​       结果是一个类数组，每个数据就是找到的元素，通过下标可以找到具体的元素

 

## 检测数据的类型：

​       Typeof：运算符，计算出该数据的类型

​                     例：var nub=120;

​                            Console.log(typeof nub);

 

 

## 运算符：      

​       \1. 算数运算符 ：

​              +加  -  *  /

​       \2. 比较运算符/判断运算符

​              \> < >= <= == != ===

​              == : 只判断数值是否相等

​              === ：判断数据类型和数值是否相等

​       \3. 赋值运算符 ：

​                                   

​              =  ：

​              += ：

​              -= ：     

​       \4. 逻辑运算符 ： 结果是布尔值

​              与 ： && 

​                     结果：

​                            true:  运算符的前后两个值必须同时为true,整体的结果才为true

​                                                 

​                            false: 运算符的前后两个值如果有一个false，整体的结果才为false

​                                           

​                                          

​              或 ： || 结果是布尔值

​                                          

​                     true:  运算符的前后两个任意一个为true,整体的结果才为true

​                     false : 运算符的前后两个值同时为false，整体的结果才为false

​                                          

​                                   

​              非 ： !  计算一个值，得出结果，结果是布尔值

​                     typeof 12

​                     先把要计算的数据转换成布尔值，然后在把该布尔值去反。

​       if() : 可以把非布尔值类型转换成布尔值类型：

​              \1. 数字 ：

​                     非0数字统统转换成true

​                     0 : 转换成false

​              \2. 字符串 ：

​                     空字符串： 转换为false

​                     非空字符串 ： 转换为true

​              \3. 空 ：null转换为false

​                                   

​              \4. 未定义 ：undefined : 转换为false

​                                   \5. 对象 ： 转换为true

​                                          \1. 数组：

​                                          \2. 对象：

if(){}

​       隐式转换：

​              \1. 数字 ：0   !0

​              \2. 字符串： ''  !''

​              \3. 未定义  ： false

​              \4. null : false

​              \5. 对象 ： true

​                     

​       算数运算符： 

​              \+  -  *  / 

​              \+  :

​              \-  : '3' - 1

​                                   

​       判断运算符 ：> < != >= <= ==  ===

​              == :

​              === : 

​                            

​       赋值运算符： = += -= 

​              ++:  +=1

​              --:  -=

​                            

​       逻辑运算符 ：

​              &&  ||  !

​                                   

​              && :      1&&2

​              || :    1||2 

​              !  :   !2

​                            

​       逗号运算符 ：,

 

取模 ： a%b

​              \1. a>b 结果是余数

​              \2. a<b 结果就是a

​              \3. a=b 结果是0

跳出当前循环 ：

​              continue : 跳过当次循环

​              break :   终止整个循环

​       ps:只能放在循环里面，否则会报错

for: 

​       break : 终止循环

​       continue : 跳过当前循环

 

 

 

一元运算符：

​              ！ typeof  new delete

二元运算符：

​              \+ - * || && += = 1+2

三元运算符：三目运算符

​       判断条件?真的值:假的值

 

 

 

++ :

​                            

​       前置++ ： ++num

​       后置++ ： num++

​                            

​       都是让变量在自身的基础上加一

​                            

​       加加赋值给其他变量

​              前置++ : 先加加，后赋值

​              后置++ ：先赋值，后加加

this : 

\1.      在事件里面，this指的是事件前面的元素

 

while循环

var num = 1;

​                 

​                 while(num<10){                       

​                        console.log(1);

​                        num++;             

​                 }

 

鼠标点击事件：onclick

鼠标移入/移出事件 ：

​                                   

​       鼠标移入 ：onmouseenter 

​                            

​       鼠标移出 ： onmouseleave

oninput : 当value值发生改变，触发事件

 

 

隐式转换 ：if(){}

​                            

强制转换 ：

​                                   

​       把其他类型的数据转换为数字类型： Number       

​                            

​       Number()方法： 把其他类型的数据转换为数字类型

​                                          

​              用法：Number('3333')

​              结果： 就是数字

​                                          

​              转换 ：

​                     \1. 字符串：

​                            \1. 纯数字的字符串 ：数字

​                            \2. 非纯数字 ： NaN

​                                                        

​                     \2. 未定义 ： NaN

​                                                 

​                     \3. 空： 0

​                                                 

​                     \4. 布尔值 ：

​                            true : 1

​                            false: 0

​                     \5. 对象

​                                          

​              parseInt() : 把其他类型的数据转换为数字类型

​                     非数字开头： 结果NaN

​                     数字开头 ： 整数

​                                                                                    

​              parseFloat(): 把其他类型的数据转换为数字类型

​                                                                                           

​       NaN : not a number ,不是一个数的数

​              什么时候出现：非法运算的结果

​                                   

​              自己都不等于自己的值      

 

## 函数 ：盛放代码的容器                           

写函数的方式 ：

​       \1. 函数声明

​              function关键字

​              function fn(){}

​       \2. 函数表达式

​              var box = function(){

​                                                                  

​              }

​                 

​       凡是在函数里面的代码，不会自己执行                  

​                                   

​       让函数里面的代码运行：

​              \1. 函数调用：

​                     函数名()

​                                   

​       最大的作用 ： 可以反复的使用

 

 

### 函数传参 ：

​       在声明一个函数时，在小括号里面写一个变量，把这个变量叫做 ： 形参

​       在函数调用时，小括号里面实际写的值，把这个实际的值叫做 ：  实参

 

function $(id,age,like){ // var id =11

​                        // var aaaaa

​                        // 获取元素

​                        var box = document.querySelector(id);

​                        

​                        console.log(id,age,like);

​                        return box;

​                 } 

​                     var a = $('.box',2,3,4);

​                     var b = $('.warp'); 

​                     

​                     console.log(a,b);

 

### 函数 ：         

​       函数声明：

​              function fn(){}        

​       函数表达式：

​              var box = function(){}

​       \1. 函数调用：

​              函数名()        

​       \2. 事件调用

return : 只能用于函数内部，

​       作用：

​              \1. 在return后面写一个值，值就是函数调用后的结果

​              \2. 终止代码执行

 

全局变量 ：没有被函数包裹的变量

使用范围 ：在任何地方都可以使用（使用值和改变值）

局部变量 ： 被函数包裹的变量

​       使用范围 : 只能在该函数里面使用

作用域 ：js的作用范围

​       以函数来划分作用域 

作用域链 ：

​       单向流通，有里往外

 

 

 

## 定时器 ：          

\1. 延迟定时器

​                                  

setTimeout(function(){},延迟的时间)

​                                                                      

\2. 间隔定时器

​       setInterval（function(){},间隔的时间）

特点 ： 

​              \1. 只要开启了定时器，不人为的关闭，那么久会永远执行

​              \2. 每个定时器调用后的返回值，是该定时器的编号，编号是惟一的

关闭定时器 ：

​       clearInterval(参数)

​       参数 ：定时器的编号

 

 

通过style属性只能获取行间样式

获取元素表现出来的样式：

​                                   

​       getComputedStyle() :

​              作用 ：

​              参数 ： 元素

​       返回值 ： 该元素的样式集合

ie专属的一个获取元素的属性：

​              currentStyle   

​              用法：元素.currentStyle

​              结果 ： 元素样式的集合   

​       Number('ww') :

 

## 函数称呼：

​       \1. 有名函数

​                                   

​       \2. 匿名函数(没有名字的函数)

​              (function(){})

​                            

匿名函数的调用，称之为自执行函数      

​       \1. 

​              解决变量名冲突

​              (function(){})()

递归函数 ：函数自己调用自己

ps :  不要代码死循环



##  预解析机制

预解析机制 ： 浏览器先把要执行的代码，预先排列一个顺序，顺序排列完成在执行代码           

​       第一步 ：

​              先找到代码里面的所有var 变量，把var 变量 提前（排在最前面）

​                            

​       第二部 ：

​              找到要声明的函数，把整个函数提前

​       第三部 ： 

​              把剩下的代码在按从上往下的顺序排列          

 

## 闭包函数 ：在函数里面嵌套一个函数            

​       特点 ： 在调用闭包函数时，如果闭包函数里面没有某个变量或者参数，在使用这个变量或者参数时，会沿着作用域链找变量或者参数，找到后放到自己的作用域里面，不会被浏览器的垃圾回收机制清空。

​       内存泄漏 ：本质上，内存泄露可以定义为：应用程序不再需要占用内存的时候，由于某些原因，内存没有被操作系统或可用内存池回收。

​		浏览器的垃圾回收机制 ：由于字符串、对象和数组没有固定大小，所有当他们的大小已知时，才能对他们进行动态的存储分配。JavaScript程序每次创建字符串、数组或对象时，解释器都必须分配内存来存储那个实体。只要像这样动态地分配了内存，最终都要释放这些内存以便他们能够被再用，否则，JavaScript的解释器将会消耗完系统中所有可用的内存，造成系统崩溃。



## this指向 ：                         

​       \1.  如果是通过事件来指向的函数，在这一次指向过程中的this指的是事件前面的元素

​                                   

​       \2.  如果是一般的函数调用，这一次指向过程中的this指的是window对象

​                                   

​       \3.  在定时器里面，this指的就是window

​       ps : this指的是调用时函数前面的对象

 

window : 是一个对象，指的是浏览器对象

​                                   

​       window.onload :等代码执行完后再执行

### 改变this指向

call() : 改变this的指向
	用法：
		函数.call(参数一，参数二,........)
		参数一 : this指代的对象
		参数二....: 实参
		
apply(参数一，参数二) : 改变this的指向
	使用 ：fn.apply(obj);
	参数 ：
		参数一 : this指代的对象
		参数二 ：是一个数组，放的是实参的集合						
						
es6新增的改变this指向的方法：
		bind()  : 改变this的指向

​		fn.bind(this指向) : 只是改变this指向
​					

​		fn.bind(this指向)(实参)
​				参数二 ：是一个数组，放的是实参的集合						

## 数学内置方法

内置对象方法：                      

​       Math ： 跟数学有关的方法

​       Math.floor() : 向下取整数

​       Math.ceil(num) : 向上取整

Math.round(num) : 小数四舍五入                  

​       数字.toFixed(n小数点后几位) ：保留小数点后几位，结果是一个字符串

​       Math.random() : 随机数，产生一个0 - 1 之间的任意小数

​                                   

Math :

​       方法：

向下取整 ：Math.floor() :      

​              ：Math.ceil() :

​              : Math.round() :

​              3333.toFixed(n) :

​              : Math.random()  

​              Math.abs() : 获取数的绝对值

​              Math.pow(参数一，参数二)  :  获取某个数的n次方

​                     参数一 : 底数

​                     参数二 ：次方数

​                     返回值 ： 计算结果

​              Math.sqrt(参数一)  : 获取某个数的开方数

​                     参数一 : 开平方的数 

​              Math.PI : π            

​              弧度和角度的换算 ：

​                     Math.PI/180 * 90

​              Math.min(参数.............) : 求最小值

​                     返回结果 ： 最小值

​              Math.max(参数.............) : 求最大值

​                     返回结果 ： 最大值

## 日期对象 ：      

​       new Date() : 时间对象,当前的本机时间

​              返回结果 ： 是一个对象

​       获取具体时间的方法：

​              获取年 ：

​                     date.getFullYear() 

​              获取月 ：     

​                     date.getMonth() : 获取的月份比中国少一；

​              获取日期(号数)

​                     date.getDate() : 

​              获取星期日期 ：

​                     date.getDay() :

​              获取小时 ：

​                     date.getHours()  :

​              获取分钟数 ：

​                     date.getMinutes()

​              获取秒钟数 ：

​                     date.getSeconds()

​              获取毫秒数 ：

​                     date.getMilliseconds();

​              时间戳 ：有当前时间到1970,01,01,00:00:00 的秒时间差

​                     getTime() :

 

### 设置时间 ：

​       new Date(2019,10,11,0,0,0) : 年，月，日，时，分，秒

​       new Date(1573401600000) : 时间戳

把获取到的本地时间在重新设置：

​       重新设置年 ：

​              newDate.setFullYear(参数)

​              参数 ：重新设置的年份

​       重新设置月份 ：  

​       newDate.setMonth(参数);

​                     参数 ： 月份，从0开始   

​       重新设置日期 ：

​              newDate.setDate(9);

​       星期只能获取不能设置 

​       重新设置时分秒：

​              newDate.setHours(16);

​              newDate.setMinutes(0);



## 数组的方法 ：    

​       push(参数) : 

​              作用：往数组的最后添加数据

​              参数 ： 要添加的数据

​              返回结果 ：添加数据以后新数组的长度

​       unshift(参数) :

​              作用：往数组的最前面添加数据

​              参数 ： 要添加的数据

​              返回结果 ：添加数据以后新数组的长度

​       pop() :

​              作用：把数组的最后一个数据删除

​              返回结果 ：被删除的数

​       shift() :

​              作用：把数组的第一个数据删除

​              返回结果 ：被删除的数据

​       indexOf(参数) :

​              作用 ： 查看某个数据在数组里面是否存在

​              参数 ： 某个数据

​              返回结果 ：查找结果

​                     -1  ： 没有找到

​                     下标 ：该数据在数组里面的下标

​       join(参数) :

​              作用 ： 把数组里面的每一个数据拼接在一起

​              参数 ： 数据与数据之间的链接内容

​              返回结果 ： 拼接后的字符串

​       concat(参数) :

​              作用 : 把几个数组拼成一个新的数组

​              参数 ： 另一个数组

​              返回结果 ： 组合后的新数组

 

### 数组方法 ：

​       reverse() :

​              作用 ：让数组倒叙

​              返回结果 ：倒叙后的新数组

​       sort(参数) :

​              作用 ： 让数组里面的数据排序

​              参数 ： function(a,b){}

​              ps : 改变原数组

​       splice(参数一，参数二，参数三，参数四。。。。。。) :

​              作用 ：对数组里面的数据进行增删改

​              参数 ：

​                     参数一 ：数组的某一个进行数据操作的下标

​                     参数二 ：删除数据的个数

​                     参数三 ......： 替换的内容

​              删 ：

​                     arr.splice(0,1);

​              改 ：

​                     arr.splice(0,1,'这是替换的内容',000,222);

​              增 ：

​                      arr.splice(4,0,'这是替换的内容',000,222);  

​              返回值 ： 是一个数组，包含的是删除的数据

 

## 项目管理工具

git : 项目版本管理工具 

svn : 项目版本管理工具 

​       这是一个软件 ：

Git Gui Here :  可视化工具(不推荐)

Git Bash Here:  用命令行的方式操作

​       .git :  git init   初始化一个git文件

git status : 监控当前文件夹里面的所有文件，是否有发送改变

把工作区里面的文件放到暂存区里面：

git add 文件名

把暂存区里面的所有文件储存到版本库：

​       git commit -m '注释说明（推荐使用英语）'

​       git add .   :  把工作区里面的所有文件放到暂存区

​       git log  :  查看版本库里面的版本

​       git reset --hard  id  : 把项目返回到某个版本

github  : 网站  基友网

远程仓库 ：

​       \1. 在github网站上面创建远程仓库

​       \2. 现在远程仓库 ：在git里面输入指令

​              git clone https://github.com/PL620/doem1.git

​       \3.  把项目储存到版本库

\4. 把版本库里面的版本推送到远程仓库

​              git push origin master

 

## es6新增的对数组的操作方法 ：

forEach() :  遍历数组

​       arr.forEach(function(data,i){

​                                          

​       })

map()  : 遍历数组

​       返回结果 ：一个和原数组一个个数的新数组，新数组的数据就是retruen结果

filter()  :  过滤器,遍历数组

some()  : 

​       返回结果： 是一个布尔值

​       数据满足某个条件，整体结果为true

every() :

把类数组变成真数组：

Array.from(参数) :

​              参数 ：类数组

返回结果 ： 真数组

 

## 字符串的方法：             

属性： length

charAt(n):  或取字符串里面下标为n的字符

n:下标

​                            

charCodeAt(n) :

​       n:下标

ASCII :

indexOf(参数一，参数二): 查找某个字符在字符串里面的位置

​       参数一 ： 查询的字符

​       参数二 ： 开始查找的位置

​       返回值 ： 

​				-1 ：没有找到

​                下标：首次找到



toLocaleLowerCase()/toLowerCase() :把大写字母变成小写这字母           

​       返回值 ： 变成小写后的字符串

​                            

toLocaleUpperCase()/toUpperCase() :把小写字母变成大写                     

​       返回值 ： 变成大写后的字符串



split(参数) : 把字符串拆分成数组

​       参数：把那个字符变成逗号

​       返回值 ：数组

 

substring(start,end): 从字符串里面截取某段字符

​       start : 开始截取的位置,包含到截取里面

​       end : 截取的结束位置，截取不到

​       返回值 ： 截取的某段字符

​                            

slice(start,end) : 从字符串里面截取某段字符

​       start : 开始截取的位置,包含到截取里面

​       end : 截取的结束位置，截取不到

​       返回值 ： 截取的某段字符

substr(start,length) : 从字符串里面截取某段字符

​       start : 开始截取的位置,包含到截取里面

​       length : 截取的个数

toString() : 把其他类型转换为字符串类型

trim() : 去掉字符串的首尾空格

 

# DOM对象

js主要分为三个部分 ：

​       1. ecmascript 

​              var if for funtion 

​       2. DOM                

​       3 .BOM 

​       DOM : 通过document对页面的元素进行增删改查

​              获取元素

​              获取样式

​              设置样式

​              删除样式

​              获取属性

​              设置属性

​              改变属性                 

​                  

## 把标签进行分类学习              

​              按标签来分 ：

​                     把标签分为各个节点 ：                                        

​              1. 如何获取元素节点 ：

​                     5                                              

​                     w3c : 

​                            1   - >  元素节点

​                            2   ->  属性节点

​                            3   ->  文本节点

​                            8   ->  注释节点

​                            9   ->  文档节点docment                                        

​                                          

​                     获取节点的类型: 

​                            nodeType                                                

​                     获取元素节点的具体名称：

​                            nodeName : 结果是元素的名称，而且是大写

​                     获取元素节点下面的属性节点：

​                            attributes

​                     元素节点包含的子节点：

​                            childNodes

 

## 通过标签与标签找元素

​                            

获取上一个兄弟元素 ：

​       previousElementSibling

获取下一个兄弟标签 ：

​       nextElementSibling

获取某元素的父级元素 ：

​       parentNode

获取某个元素的所有子元素

​       children

某元素下面的第一个子元素

​       firstElementChild  

某元素下面的最后一个子元素

​       lastElementChild

 

 

## 对属性的操作            

​       获取属性值设为方法：

​       \1. box.className(只能获取w3c定义好的属性和通过js.的方式设置的属性)

​       \2. getAttribute('属性名'): 可以获取行间属性，通过setAttribute设置的属性

​       \3. box.dataset.cc

​       设置属性 ：

​              \1. box.className = 11；

​              \2. box.setAttribute('属性名'，‘属性值’)

​              \3. box.dataset.cc = '11';       

​       删除属性 ：

​              box.removeAttribute('属性名');

 

### 创建一个元素 ：

​       document.createElement('标签名')

### 删除标签：

​        box.remove(); 

​        父级.removeChild(要删除的子元素);

### 把创建的元素插入到页面

​       \1. appendChild(要插入的标签) : 往父级的最后位置插入标签

​       父级.appendChild(要插入的标签)

insertBefore(参数一，参数二)  :  往某个元素之前插入标签

​       参数一 : 创建的元素

​       参数二 ： 参考物

父.insertBefore()

 

### 克隆元素 ：

​       cloneNode(参数)

​              参数：布尔值

​              true：全部复制

​              fasle: 默认值，只克隆当前元素

​       目标.cloneNode()

### 替换 ：

​       replace(参数一，参数二): 把一个标签替换另一个标签

​              参数一：  替换

​              参数二 ： 被替换

### 位置：

​       一个元素到另外一个元素的位置（拥有包含关系）

​       offsetLeft:

​              元素到定位父级的左边的距离

​       offsetTop :

​              元素到定位父级的top边的距离



getBoundingClientRect(): 获取元素向对于可视区的位置和自身的大小

​       返回结果 ： 集合

window.onresize : 浏览器的窗口大小发生改变，触发事件

window.onscroll : 滚动条的位置发生改变，触发事件

 

### 获取元素的实际大小：

​                                   

​       offsetWidth : width + padding + border

​       offsetHeight : 

​       clientWidth : width + padding

​       clientHeight :

 

## DOM事件                             

onclick 

onmouseenter 

onmouseleave 

oninput

​       鼠标移入：

​              onmouseenter ：

​              onmouseover:  从父级进入子元素会触发事件，从子元素进入父级也会触发事件

​       鼠标移出 ：

​              onmouseleave  :

​              onmouseout  : 从父级进入子元素会触发事件，从子元素进入父级也会触发事件

​       onclick : 鼠标左键按下抬起 

​       onmousedown :  鼠标左键按下事件

oninput:input的值发生改变后执行

onchange：value值发生改变并且失去光标后执行

onfocus:获取光标，触发事件

onblur：失去光标，触发事件    

### 获取光标的方法：

inp.focus:获取光标，但是不选中值

inp.select:获取光标，选中值

### 键盘事件：

onkeydown:按下键盘触发事件

onkeyup:抬起键盘触发事件

onkeypress:拿下键盘触发事件

onmouseup : 鼠标左键抬起事件

onmousemove :  鼠标移动

ondblclick : 鼠标左键双击事件

 

 

## 事件          

### 传统事件 ：

​       带on的事件，特点一个元素只能用有一个相同事件，

​       如果有多个，下面的事件会把上面的事件覆盖

### 事件监听 :

事件绑定函数/事件监听 ：通过一个函数的方式给元素添加事件

​       addEventListener(参数一，参数二，参数三)

​              参数一 ： 不带on的事件名称，是一个字符串 

​              参数二 :  触发事件时，要执行的函数

​              参数三 :  是否冒泡

​              特点 ：元素能拥有n个相同事件。

ie低版本专属事件监听

​       attachEvent(参数一，参数二)

​              参数一:带on的事件名称，是一个字符串

​              参数二:触发事件时，要执行的函数



### 解绑事件

​       removeEventListener(参数一，参数二)

​       参数一:

​              解除的事件的名称，字符串

​              参数二:

​              解除事件里面的函数名

低版本ie解绑事件

​       detachEvent(参数一，参数二)

​              参数一:

​              解除的事件的名称，字符串

​              参数二:

​              解除事件里面的函数名

 

### 冒泡机制

冒泡机制：当元元素触发事件时，事件先从window开始一层层往下面找目标元素，找到目标元素以后又回到window，整过程就叫做冒泡机制 

捕获阶段：事件先从window开始一层层往下面找，一直到找到目标元素的节点，叫做捕获阶段

冒泡阶段：找到目标元素以后又回到window，冒泡阶段。

冒泡机制的特点 ： 从window找到目标元素 的过程中，如果祖先元素拥有和目标元素相同的事件，祖先元素的事件就会被触发。

​       addEventListener('不带on的事件名'，函数，布尔值)   

​              false:默认值 ，表示冒泡

​              true : 表示捕获

 

## 事件对象

事件对象：触发函数时，事件调用函数时传的实参

​       是一个对象，叫做事件对象

event: e/ev

​       取消冒泡机制：

​       ev.cancelBubble = true 不是w3c提供的阻止冒泡的方法，但是兼容低版本ie

​              true: 取消冒泡机制

​              false: 不取消冒泡机制

​              stopPropagation() : W3C官方提供的阻止冒泡的方法，但是不兼容低版本ie

在地版本ie浏览器里面，事件调用函数不会忘里面传实参，只是在window对象里面

添加了一个event属性，和event事件对象一样。

 

pageX  :  当触发事件时，鼠标箭头在可视区的x轴位置

pageY  :  当触发事件时，鼠标箭头在可视区的y轴位置

 

### 取消浏览器的默认行为:

​       preventDefault();

 

### 事件源

事件源： 事件发生的源头,是一个元素，具体到元素上面

在事件对象里面有一个属性：   target

ev.target :

 

### 滚轮事件 ：

​              onwheel                   

​              DOMMouseScroll :只能用于事件监听

 

## 懒加载

懒加载也就是延迟加载。当访问一个页面的时候，先把img元素或是其他元素的背景图片路径替换成一张大小为1*1px图片的路径（这样就只需请求一次，俗称占位图），只有当图片出现在浏览器的可视区域内时，才设置图片正真的路径，让图片显示出来。这就是图片懒加载。



为什么要有懒加载？

很多页面，内容很丰富，页面很长，图片较多。比如说各种商城页面。这些页面图片数量多，而且比较大，少说百来K，多则上兆。要是页面载入就一次性加载完毕，估计用户已经失去耐心关闭网页了。



原理是什么？

​		页面中的img元素，如果没有src属性，浏览器就不会发出请求去下载图片，只有通过javascript设置了图片路径，浏览器才会发送请求。懒加载的原理就是先在页面中把所有的图片统一使用一张占位图进行占位，把正真的路径存在元素的“data-url”（一般这个属性我们自己定义）属性里，要用的时候就取出来，再设置。
懒加载的实现步骤？
​		1)首先，不要将图片地址放到src属性中，而是放到其它属性(data-original)中。 
​		2)页面加载完成后，根据scrollTop判断图片是否在用户的视野内，如果在，则将data-original属性中的值取出存放到src属性中。
​		3)在滚动事件中重复判断图片是否进入视野，如果进入，则将data-original属性中的值取出存放到src属性中。



懒加载的优点？

​		页面加载速度快、可以减轻服务器的压力、节约了流量,用户体验好。



懒加载的意义及实现方式

意义：

​		懒加载的主要目的是作为服务器前端的优化，减少请求数或延迟请求数。 

实现方式： 

​		\1.  第一种是纯粹的延迟加载，使用setTimeOut或setInterval进行加载延迟. 

​		\2.  第二种是条件加载，符合某些条件，或触发了某些事件才开始异步下载。 

​		\3.  第三种是可视区加载，即仅加载用户可以看到的区域，这个主要由监控滚动条来实现，一般会在距用户看到某图片前一定距离遍开始加载，这样能保证用户拉下时正好能看到图片。



## 预加载

什么是预加载？

​		提前加载图片，当用户需要查看时可直接从本地缓存中渲染。



为什么要使用预加载？

​		图片预先加载到浏览器中，访问者便可顺利地在你的网站上冲浪，并享受到极快的加载速度。这对图片画廊及图片占据很大比例的网站来说十分有利，它保证了图片快速、无缝地发布，也可帮助用户在浏览你网站内容时获得更好的用户体验。



实现预加载的方法有哪些？

​		方法一： 用CSS和JavaScript实现预加载

​		单纯使用CSS，可容易、高效地预加载图片



使用Ajax实现预加载

​		我们使用Ajax实现图片预加载的方法。该方法利用DOM，不仅仅预加载图片，还可以预加载CSS、JavaScript等相关的东西。使用Ajax，比直接使用JavaScript，优越之处在于JavaScript和CSS的加载不会影响到当前页面。该方法简洁、高效。



预加载的意义及实现方式

意义:

​		预加载可以说是牺牲服务器前端性能，换取更好的用户体验，这样可以使用户的操作得到最快的反映。 

实现方式：

​		实现预载的方法非常多，比如：用CSS和JavaScript实现预加载；仅使用JavaScript实现预加载；使用Ajax实现预加载。 

​		常用的是new Image();设置其src来实现预载，再使用onload方法回调预载完成事件。只要浏览器把图片下载到本地，同样的src就会使用缓存，这是最基本也是最实用的预载方法。当Image下载完图片头后，会得到宽和高，因此可以在预载前得到图片的大小(方法是用记时器轮循宽高变化)。



## 懒加载与预加载的概念和区别

概念

​		懒加载也叫延迟加载：JS图片延迟加载,延迟加载图片或符合某些条件时才加载某些图片。 

预加载：提前加载图片，当用户需要查看时可直接从本地缓存中渲染。



区别

​		两种技术的本质：两者的行为是相反的，一个是提前加载，一个是迟缓甚至不加载。懒加载对服务器前端有一定的缓解压力作用，预加载则会增加服务器前端压力。



# BOM

BOM是浏览器对象模型BOM是browser object model的缩写，简称浏览器对象模型。BOM提供了独立于内容而与浏览器窗口进行交互的对象
由于BOM主要用于管理窗口与窗口之间的通讯，因此其核心对象是window。BOM由一系列相关的对象构成，并且每个对象都提供了很多方法与属性。BOM缺乏标准，JavaScript语法的标准化组织是ECMA，DOM的标准化组织是W3C。BOM最初是Netscape浏览器标准的一部分。



window.screenTop   //窗口顶部距屏幕顶部的距离
window.screenLeft  //窗口左侧距屏幕左侧的距离
window.innerWidth  //窗口中可视区域(viewpoint)的宽
window.innerHeight  //窗口中可视区域(viewpoint)的高度 该值与浏览器是否显示菜单栏等因素有关
window.outerWidth  //浏览器窗口本身的宽度(可视区域宽度+浏览器边框宽度)
window.outerHeight  //浏览器窗口本身的高度
注意：
chrome在最大化时浏览器窗口没有边框宽度,非最大化时有8px边框
ff和ie上下左右有8px的边框宽度



## BOM结构示意图

BOM学习中我们将学到与浏览器窗口交互的一些对象，例如可以移动，调整浏览器大小的window对象，可以用于导航的location 对象与history对象，可以获取浏览器，操作系统与用户屏幕信息的navigator与screen对象，可以使用document作为访问HTML文档的入口，管理框架的frames对象等。

![image-20191120204511065](C:\Users\15953\AppData\Roaming\Typora\typora-user-images\image-20191120204511065.png)





## DOM和BOM的区别

DOM通过脚本动态地访问和更新文档的内容、结构以及样式的接口。BOM通过脚本操作浏览器的各个功能组件的接口。

 区别：DOM描述了处理网页内容的接口，BOM描述了与浏览器进行交互的接口。document是DOM的核心对象，window则是BOM的核心对象。



## window对象是什么

浏览器打开一个文档，就创建了一个 window 对象，即 window 对象表示浏览器中打开的窗口。

window 对象是全局对象，可以把窗口的属性作为全局变量来使用。例如，可以只写 document，而不必写 window.document。同样，可以把当前窗口对象的方法当作函数来使用，如只写 alert()，而不必写 Window.alert()。

如果文档包含框架（frame），浏览器会为文档创建一个 window 对象，并为每个框架创建一个额外的 window 对象。

在window对象属性和方法中，某些属性和方法存在浏览器兼容性的问题，而有些属性则已经被浏览器弃用。所以我们这里主要着重讲解：location、navigator、screen和history。



### window.open(); 

打开一个新窗口http://www.cnblogs.com/li0803/archive/2008/11/03/1324746.html（HTTP协议详解）有两种方式打开：

 1：直接调用IE支持ff/chrome有拦截

 2:*人为主动触发*的事件调用：所有浏览器都支持

 		参数（4个参数，最后一个参数没用，相当于3个参数）：

 1.url:如果路径为线上地址，要遵循HTTP协议 

 2.打开的方式:默认值为，_blank当前页面打开：_self

​		如果在iframe中打开，那么在window.open的第二个参数中填写name值

 3.设置窗口大小width,height,IE下设置是否可以缩放，yes可以缩放，no不可以缩放

 		注意：如果要设置第三个参数，那么第二个必须为_blank

 		返回值为，新打开窗口的window



### window.close();

 关闭当前窗口

 如果直接调用：chrome中直接关闭当前窗口

​							ff没反应

​							IE，有个温馨提示

​							人为主动触发事件也和直接调用一样；所有浏览器都能兼容的方法是：通过window.open去打开，然后就可以关闭打开的窗口。  



### window.navigator.userAgent;

用户代理信息,操作系统 、 浏览器内核 、浏览器版本等

window.location:  获取地址栏信息是个对象

​								字符串版的地址信息：window.location.href;

​								地址栏查询信息：window.location.search (问号到井号之间的信息)

​								既可以读也可以写,如果为写操作，那么是会刷新页面的(除非有设置锚信息)。没有用人为事件触发，那么设置的时候会一直刷新。

​								锚信息：window.location.hash (井号之后的内容) 既可以读也可以写



### 获取可视区的高宽

window.innerWidth:获取可视区的宽度（包含滚动条宽度） 

window.innerHeight



pageYOffset:只能读取不能设置滚动条的高度

pageXOffset只能读取不能设置滚动条的宽度

window.scrollTo(x,y) 设置滚条的距离

clientHeight:如果没有设置样式高度，那么结果就为内容撑出来的高度

document.body.scrollHeight ：被内容称出来的高度（但是不是太精确，会有点点误差，可以通过统一文字的样式，这样就能精确获取）。

document.body.offsetHeight:如果没有设置高度，跟内容撑开的值来走，如果设置了就走设置的高度。



可视区的宽高：document.documentElement.clientWidth

可视区的高度：document.documentElement.clientHeight

左右两边居中：left:(可视区的宽度 - 当前元素的宽度)/2

 top:(可视区的高度 - 当前元素的高度)/2

 

onscroll:当滚动滚动条的时候，触发的事件

onresize:当页面缩放的时候，触发的事件



## 什么是History 对象？

JavaScript History 对象用于记录操作浏览器的访问历史。History 对象是 window 对象的一部分，可通过 window.history 属性对其进行访问。

提示：History 对象的有效作用范围都是指当前窗口。



History 对象有唯一的一个 length 属性，用于得到浏览器访问历史记录中的 URL 数量。



### History 对象有如下 3 个方法：

\1. history.back()：返回前一个浏览页面（如果存在）

\2. history.forward()：前往下一个浏览页面（如果存在）

\3. history.go(2/-1)：前往 history 列表中的某个指定页面（如果存在）





## Location是什么？

JavaScript Location 对象用于获取或设置当前的 URL 信息。Location 对象是 window 对象的一部分，可通过 window.location 属性对其进行访问。

Location 对象常用于得到 URL 地址中的信息，或者刷新当前页面，页面重定向等，具体可见下面列出的各属性和方法。

![image-20191120195452561](C:\Users\15953\AppData\Roaming\Typora\typora-user-images\image-20191120195452561.png)

<script type="text/javascript">
		console.log(window.location.hash);//  #1
		console.log(window.location.host);//  127.0.0.1:8001
		console.log(window.location.hostname);//  127.0.0.1
		console.log(window.location.href);//  http://127.0.0.1:8001/2.08/01.location.html?__hbt=1532484540442#1
		console.log(window.location.pathname);//  /2.08/01.location.html
		console.log(window.location.port);//  8001
		console.log(window.location.protocol);//  http:
		console.log(window.location.search);//   ?__hbt=1532484395449
	</script>



### Location 对象方法

Location对象有如下 3 个方法：

location.assign()：加载新页面文档

location.reload()：重新加载（刷新）当前页面

location.replace()：用新的文档替代当前文档



说明：实际上 location.assign() 方法的效果与 location.href 是一样的。



#### location.reload()

Location 对象的 reload() 方法用于重新加载当前文档（页面），语法如下：

location.reload( false|true )

如果该方法参数为 false 或者省略参数，它就会用 HTTP 头 If-Modified-Since 来检测服务器上的文档是否已改变。如果文档已改变，location.reload() 会再次下载该文档。如果文档未改变，则该方法将从缓存中装载文档。

如果要强制刷新当前页面，请将参数设置为 true。



#### location.replace()

Location 对象的 replace() 方法用于重新加载当前文档（页面），语法如下：

location.replace( new_URL )



#### replace() 与 reload() 的区别

location.reload() 方法用于刷新当前页面，如果有 POST 数据提交，则会重新提交数据；location. replace() 则将新的页面以替换当前页面，它是从服务器端重新获取新的页面，不会读取客户端缓存且新的 URL 将覆盖 History 对象中的当前纪录（不可通过后退按钮返回原先的页面）。

如果想要刷新当前的页面，又避免 POST 数据提交，可以使用：

window.location.replace( location.href );



## Navigator 对象是什么？

JavaScript Navigator 对象包含了有关浏览器的相关信息。

提示：Navigator 对象虽然没有明确的相关标准，但所有浏览器都支持该对象。

![image-20191120200922460](C:\Users\15953\AppData\Roaming\Typora\typora-user-images\image-20191120200922460.png)

注意说明

\1. navigator.appCodeName：IE/Firefox/Chrome 系列浏览器中，它的值都是 "Mozilla"。

\2. navigator.appName：Firefox/Chrome 均为 Netscape。

\3. navigator.browserLanguage：Firefox/Chrome 返回 "undefined"。

\4. navigator.cpuClass：Firefox/Chrome 返回 "undefined"。

\5. navigator.onLine：Firefox/Chrome 返回 "undefined"。

\6. navigator.systemLanguage：Firefox/Chrome 返回 "undefined"。

\7. navigator.userLanguagee：Firefox/Chrome 返回 "undefined"。

利用 Navigator 对象提供的浏览器信息，可以方便的得到访问用户的浏览器名称及版本。



### 定位事件

HTML5 Geolocation API 用于获得用户的地理位置。 Internet Explorer 9、Firefox、Chrome、Safari 以及 Opera 支持地理定位。对于拥有 GPS 的设备，比如 iPhone，地理定位更加精确。该对象主要有三个方法：getCurrentPosition()，watchPosition()，clearWatch()。但是我们要判断浏览器的支持情况。

<script type="text/javascript">

 if (navigator.geolocation){ // 支持

   

 }else{ // 不支持

   console.log("您的浏览器不支持定位")

 }

 </script>



#### getCurrentPosition方法

getCurrentPosition()方法 可以传递三个参数。调用这个方法就会触发请求用户共享地理定位信息的对话框 。这个方法接收三个具体的参数分别是成功的回调函数，失败回调函数，以及配置选项。

![image-20191120201405428](C:\Users\15953\AppData\Roaming\Typora\typora-user-images\image-20191120201405428.png)

position对象有两个属性：coords 和 timestamp 。 coords 对象中将包含下列与位置相关的信息。

latitude：以十进制度数表示的纬度

longitude：以十进制度数表示的经度

accuracy：经纬度坐标的精度，以米为单位

有些浏览器可能会在 coords 对象中提供如下属性。

altitude：以米为单位的海拔高度，如果没有相关数据则值为 null

altitudeAccuracy：海拔高度的精度，以米为单位，数值越大越不精确

heading：指南针的方向，0°表示正北，值为 NaN 表示没有检测到数据

speed：速度，即每秒移动多少米，如果没有相关数据则值为 null

msg包含两个属性：message 和 code。其中，message 属性是提示文本消息，解释为什么会出错，而 code 属性中保存着一个数值，表示错误的类型：用户拒绝共享（1），位置无效（2）或者超时（3）



<script type="text/javascript">
		if (navigator.geolocation){  // 支持
		    navigator.geolocation.getCurrentPosition(success, error);
		    // 成功的回调函数
		    function success(position) {
		        // 获取经纬度信息
		      	console.log(position.coords.latitude, position.coords.longitude);
		    }
			// 失败的回调函数
		    function error(msg) {
		        // 输出失败的信息
		       console.log(msg.code, msg.message);
		    }
		}else{  // 不支持
		    console.log("您的浏览器不支持定位")
		}
	</script>
注意：因为我们的这个API默认访问的使用谷歌地图，所以很有可能会出现错误，因为国内访问谷歌地图服务器有限制。



#### watchPosition()

如果要跟踪用户的位置，那么可以使用 watchPosition() 方法。这个方法的使用和 getCurrentPosition() 完全相同。实际上 watchPosition() 与定时调用 getCurrentPosition() 能得到相同效果。在第一次调用 watchPosition() 方法后，会取得当前位置，执行成功回调或者错误回调。然后，watchPosition() 就地等待系统发出位置已改变的信号。

 调用 watchPosition() 会返回一个数值标识符，用于跟踪监控的操作。基于这个返回值可以取消监控操作，只要将其传递给 clearWatch() 方法即可（与使用 setTimeout() 和 clearTimeout() 类似），例如：

var watchId = navigator.geolocation.watchPosition(success, error);

clearWatch(watchId);



#### clearWatch()

清除一个跟踪控制监听。需要传入使用watchPosition函数返回的值。



#### 为什么使用百度地图

我们的百度地图和高度地图是目前国内主要的地图工具提供商。官方都提供了非常相信的信息内容。具体可以参考官方文档进行学习。

 <!--// 注意要引入百度key-->

```html
<script type="text/javascript" src="http://api.map.baidu.com/api?v=2.0&ak=???"></script>
<script>
var geolocation = new BMap.Geolocation();
geolocation.getCurrentPosition(function(r){
	if(this.getStatus() == BMAP_STATUS_SUCCESS){
		alert('您的位置：'+r.point.lng+','+r.point.lat);
	}else {
		alert('failed'+this.getStatus());
	} 
});
</script>
```



## 本地存储

### 什么是 HTML 本地存储？

通过本地存储（Local Storage），web 应用程序能够在用户浏览器中对数据进行本地的存储。

在 HTML5 之前，应用程序数据只能存储在 cookie 中，包括每个服务器请求。本地存储则更安全，并且可在不影响网站性能的前提下将大量数据存储于本地。

与 cookie 不同，存储限制要大得多（至少5MB），并且信息不会被传输到服务器。

本地存储经由起源地（origin）（经由域和协议）。所有页面，从起源地，能够存储和访问相同的数据。



### Cookies

储存的时间默认为session时间

设置cookies：document.cookie = 'name = 111';

获取存储的数据：document.cookie

修改已经存储的数据：给已经存在的name重新赋值

修改存储的时间：document.cookie = 'user1=112222;expires=时间';

如何删除时间：让储存的数据时间过期



###  本地存储（Local Storage） 

获取本地存储的数据：window.localStorage.getItem();

设置：window.localStorage.setItem();

清除某条数据：window.localStorage.removeItem();

清除所有数据：window.localStorage.clear();



## 什么是正则表达式

正则表达式(regular expression)是一个描述字符模式的对象。ECMAScript的RegExp类表示正则表达式，而String和RegExp都定义了使用正则表达式进行强大的模式匹配和文本检索与替换的函数。

正则表达式的作用

正则表达式主要用来验证客户端的输入数据。用户填写完表单单击按钮之后，表单就会被发送到服务器，在服务器端通常会用JAVA、PHP、ASP.NET等服务器脚本对其进行进一步处理。因为客户端验证，可以节约大量的服务器端的系统资源，并且提供更好的用户体验。



### 如何创建正则表达式

建正则表达式和创建字符串类似，创建正则表达式提供了两种方法，一种是采用new运算符，另一个是采用字面量方式。



new运算符创建正则表达式

它接收两个参数：一个是要匹配的字符串模式，另一个是可选的标志字符串。

实例（ 21.RegExp1.html ）：

<script type="text/javascript">

var pattern = new RegExp("[bc]at","i");

//匹配第一个bat或者cat,不区分大小写

</script>



采用字面量方式创建正则表达式

与new运算符方式类似，它也可以看作是接收两个参数：一个是要匹配的字符串模式，另一个是可选的标志字符串。

实例（ 22.RegExp2.html ）：

<script type="text/javascript">

var pattern = /[bc]at/i;

//匹配第一个bat或者cat,不区分大小写

</script>



### 常用的正则表达式方法

正则表达式有很多方法，在这里只选几个比较常用的来讲解：

exec()方法

test()方法

search()方法

match()方法

replace()方法



exec()方法：

该方法是专门为捕获组而设计的，其接受一个参数，即要应用模式的字符串，然后返回包含第一个匹配项信息的数组；或者在没有匹配项的情况下返回null。返回的数组虽然是Array的实例，但是包含两个额外的属性：index和input。其中index表示匹配项在字符串中的位置，而input表示应用字符串表达式的字符串。

实例（ 23.exec.html ）：

<script type="text/javascript">
var text = "mom and dad and baby";
var pattern = /mom( and dad( and baby)?)?/gi;
var matches = pattern.exec(text);
console.log(matches.index); //0
console.log(matches.input); //mom and dad and baby
console.log(matches[0]);    //mom and dad and baby
console.log(matches[1]);    //and dad and baby
console.log(matches[2]);    //and baby
</script>



test()方法：
正则表达式常用方法test()，它接受一个字符串参数。在模式与该参数匹配的情况下返回true，否则返回false。
实例（ 24.test.html ）：

<script type="text/javascript">
//判断是否是数字
var str = '374829348791';
var re = /\D/;      //  \D代表非数字
if( re.test(str) ){   // 返回true,代表在字符串中找到了非数字。
    alert('不全是数字');
}else{
    alert('全是数字');
}
</script>



search()方法：
在字符串搜索符合正则的内容，搜索到就返回出现的位置（从0开始，如果匹配的不只是一个字母，那只会返回第一个字母的位置）， 如果搜索失败就返回 -1
实例（ 25.search.html ）：

<script type="text/javascript">
var str = 'abcdef';
var re = /B/i;
//var re = new RegExp('B','i'); 也可以这样写
alert( str.search(re) ); // 1
</script>



match ()方法：
获取正则匹配到的结果，以数组的形式返回
实例（ 26.match.html ）：

<script type="text/javascript">
"186a619b28".match(/\d+/g); // ["186","619","28"] 
</script>



replace()方法：
replace 本身是JavaScript字符串对象的一个方法，它允许接收两个参数：replace([RegExp|String],[String|Function])
第1个参数可以是一个普通的字符串或是一个正则表达式.第2个参数可以是一个普通的字符串或是一个回调函数.
实例（ 27.replace.html ）：

<script type="text/javascript">
var phone = "13112345678";
var sliceNumber = 1234;
var newPhone = phone.replace(new RegExp(sliceNumber,'g'),'****');
console.log(newPhone); //131****5678
</script>



### 正则表达式的特殊字母和符号

特殊字母 ：
	\  : 转义符，把用于特殊作用的字母的功能显示出来				
	\d : 任意数字
	\D : 非数字
	\w : 数字，字母，下划线
	\W : !(数字，字母，下划线)
	\s : 空格
	\S : 非空格
	\n:换行
					
特殊符号：
	\  :  转义符
	F:\web2017\work\2019-11-22

​	2 ~/Desktop

​	+: 量词，代表数量,至少一个
​	?  : 量词, 最多一个

​	*： 量词，代表数量,至少一个
​	.  : 任意字符
​	^  : 从开头开始查找
​	$  : 以什么结束
​	[] : 选择任意一个
​	[^] : 非[]里面的任意字符
​	{}  : 
​		{3} : 几位数
​		{3,6}: 几位到几位
​		{3,} :  至少几位



# jQuery

jQuery的基本功能

访问和操作 DOM 元素

控制页面样式

对页面事件的处理

大量插件在页面中的运用

与 Ajax 技术的完美结合

搭建jQuery开发环境

 由于 jQuery 是一个完整的 JavaScript 文件库， 因此， 搭建 jQuery 开发环境十分简单， 无须安装任何文件，只需要先在 jQuery 官方网站下载最新的文件库，然后将该文件库引入页面中的 <head> 元素间即可。



jQuery 程序的代码风格

1.“$”美元符的使用

\2. 事件操作链接式书写

事件操作链接式书写

 功能描述

在示例 1-1 基础之上，增加两个 <div> 元素，一个为框架，另一个为标题。示例 1-1 显示的文字为内容，框架元素包含标题和内容元素。当页面首次加载时，被包含的内容 <div> 标记是不可见的，当用户单击主题 <div> 标记时，改变自身的背景色，并将内容 <div> 标记显示出来。



选择器的优势

与传统的 JavaScript 获取页面元素和编写事务相比，jQuery 选择器具有明显的优势，具体表现在以下两个方面：

n代码更简单。

n完善的检测机制。

jQuery 选择器的类型

根据所获取页面中元素的不同，可以将 jQuery 选择器分为四大类：基本选择器、层次选择器、过滤选择器、表单选择器。其中，在过滤选择器中又可分为 ：简单过滤选择器、内容过滤选择器、可见性过滤选择器、属性过滤选择器、子元素过滤选择器、表单对象属性过滤选择器。



通过jq获取元素 ：
			$('选择器')



给获取到的元素设置样式：
					css(样式，样式值) : 给元素添加样式
					css({
						background:'red',
						height:'200px',
						'color':'green'
					})



属性的操作：
					获取 ：attr('属性名')     属性名:要获取属性值的属性

​					设置 ：attr('属性名','属性值')

​					删除 ：removeAttr(属性)



对class：
					添加class:addClass():


​					删除class:removeClass()


​					toggleClass: 有class就删除，没有class就添加

​					eq(n)  : 从获取的jq对象里面选出一个来操作 n: 获取到的元素下标



size() : 获取元素的长度
				
				get(参数) :把jq对象转换为原生元素
					参数 ： 下标
				
				each(参数) : 遍历获取到的元素
					参数 ：函数，每次循环时执行的代码
					$.each(arr,function(i,data){
								   console.log(data,i)
					})	
				
				标签与标签的关系：
					
					s上一个兄弟：
						prev(): 上一个兄弟标签的jq对象
					
					上面的所有兄弟：
						prevAll(参数) ：
							参数 : 选择器，筛选出上面所有兄弟里面的某些元素


​					
​					下一个兄弟 ：
​						next(): 下一个兄弟标签的jq对象
​						
​						nextAll('.lis2') :


​					
​					父级：
​						parent(): 父级
​						
​						parents(参数): 祖先级
​							参数 ：选择器


​					后代：
​						children(参数): 所有的子元素
​							参数： 选择器，所有子元素里面的某些元素
​						

						find(参数): 找到某个元素下面的后代元素
							参数：选择器， 后代的范围
详细见手册



# 面向对象

## 什么是面向对象

面向对象编程（ObjectOrientedProgramming，OOP，面向对象程序设计）是一种计算机编程架构。OOP的一条基本原则是计算机程序是由单个能够起到子程序作用的单元或对象组合而成。OOP达到了软件工程的三个主要目标：重用性、灵活性和扩展性。为了实现整体运算，每个对象都能够接收信息、处理数据和向其它对象发送信息。



创建一个对象:创建一个对象，然后给这个对象新建属性和方法。

![image-20191128180238840](C:\Users\15953\AppData\Roaming\Typora\typora-user-images\image-20191128180238840.png)

## 工厂模式

工厂模式:上面创建了一个对象，并且创建属性和方法，在run()方法里的this，就是代表box对象本身。这种是JavaScript创建对象最基本的方法，但有个缺点，想创建一个类似的对象，就会产生大量的代码。

![image-20191128180331376](C:\Users\15953\AppData\Roaming\Typora\typora-user-images\image-20191128180331376.png)

为了解决多个类似对象声明的问题，我们可以使用一种叫做工厂模式的方法，这种方法就是为了解决实例化对象产生大量重复的问题。

![image-20191128180517103](C:\Users\15953\AppData\Roaming\Typora\typora-user-images\image-20191128180517103.png)



## 构造方法

构造方法:工厂模式解决了重复实例化的问题，但还有一个问题，那就是识别问题，因为根本无法搞清楚他们到底是哪个对象的实例。

![image-20191128180547217](C:\Users\15953\AppData\Roaming\Typora\typora-user-images\image-20191128180547217.png)

ECMAScript中可以采用构造函数（构造方法）可用来创建特定的对象。类似于Object对象。

![image-20191128180559882](C:\Users\15953\AppData\Roaming\Typora\typora-user-images\image-20191128180559882.png)



使用构造函数的方法，即解决了重复实例化的问题，又解决了对象识别的问题，但问题是，这里并没有new Object()，为什么可以实例化Box()，这个是哪里来的呢？new Object()在什么地方执行了？

执行的过程如下：

当使用了构造函数，并且new 构造函数()，那么就后台执行了new Object()；

将构造函数的作用域给新对象，(即new Object()创建出的对象)，而函数体内的this就代表new Object()出来的对象。

执行构造函数内的代码；

返回新对象()



使用了构造函数的方法，和使用工厂模式的方法他们不同之处如下：

构造函数方法没有显式的创建对象(new Object())；

直接将属性和方法赋值给this对象；

没有renturn语句。

构造函数的方法有一些规范：

函数名和实例化构造名相同且大写，(非强制，但这么写有助于区分构造函数和普通函数)；

通过构造函数创建对象，必须使用new运算符。



关于this的使用，this其实就是代表当前作用域对象的引用。

如果在全局范围this就代表window对象，如果在构造函数体内，就代表当前的构造函数所声明的对象。

![image-20191128180701355](C:\Users\15953\AppData\Roaming\Typora\typora-user-images\image-20191128180701355.png)



