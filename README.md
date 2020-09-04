# 19-Interview

---

## JavaScript知识点

---

### 闭包-从编译原理角度解释词法作用域

谈到闭包少不了关于作用域的讲解。要想理解作用域的实现机制，我们需要结合 JS 的编译原理一起来看。

``` 
var name = '19-Qingfeng'
```

这段代码在JS中其实做了两件事。

* var name （编译时处理）

* name = 19-Qingfeng （运行时处理）

> 事实上，JS 也是有编译阶段的，它和传统语言的区别在于，JS 不会早早地把编译工作做完，而是一边编译一边执行。简单来说，所有的 JS 代码片段在执行之前都会被编译，只是这个编译的过程非常短暂（可能就只有几微妙、或者更短的时间），紧接着这段代码就会被执行。

* 编译阶段： 这时登场的是一个叫 编译器 的家伙。编译器会找遍当前作用域，看看是不是已经有一个叫 name 的家伙了。如果有，那么就忽略 var name 这个声明，继续编译下去；如果没有，则在当前作用域里新增一个 name。然后，编译器会为引擎生成运行时所需要的代码，程序就进入了执行阶段

* 执行阶段： 这时登场的就是大家常常听到的 JS 引擎 了。JS 引擎在执行代码的时候，仍然会找遍当前作用域，看看是不是有一个叫 name 的家伙。如果能找到，那么万事大吉，我来给你赋值。如果找不到，它也不会灰心，它会从当前作用域里 “探出头去”，看看 “外面” 有没有，或者 “外面的外面” 有没有。如果最终仍然找不到 name 变量，引擎就会抛出一个异常。

#### 作用域套作用域，就有了作用域链

> 作用域本质上就是程序存储和访问变量的规则。

目前JS语言中已经有了三种作用域链：

1. 全局作用域。 

2. 函数作用域。

3. 块级作用域:ES6开始的let和const声明。

> 看看下面这个例子

``` 
function addABC(){
  var a = 1,b = 2;
  
  function add(){
    return a+b+c;
  }
  return add;
}

var c = 3

var globalAdd = addABC()

console.log(globalAdd()) // 6

```

上面例子的嵌套规则和作用域用图来说:

![bibao.jpg](https://i.loli.net/2020/09/03/tO84CzAa1y2GKwR.png)

他的作用域链是这样的

![bibao2.jpg](https://i.loli.net/2020/09/03/WSZOKTuBeJIYUda.png)

其中 add 这个函数，它嵌套在函数 addABC 的内部，想要查找 a、b、c 三个变量，它得去上层的 addABC 作用域里找，对吧？

#### 引出闭包的概念:

**像 a、b、c 这样在函数中被使用，但它既不是函数参数、也不是函数的局部变量，而是一个不属于当前作用域的变量，此时它相对于当前作用域来说，就是一个自由变量。而像 add 这样引用了自由变量的函数，就叫闭包。**

#### 顺道说说 LHS、 RHS

LHS、RHS，是引擎在执行代码的时候，查询变量的两种方式。其中的 L、R，分别意味着 Left、Right。这个“左”和“右”，是相对于赋值操作来说的。当变量出现在赋值操作的左侧时，执行的就是 LHS 操作，右侧则执行 RHS 操作：

``` 
name = '19-Qingfeng';
```

在这个例子里，name 变量出现在赋值操作的左侧，它就属于 LHS。**LHS 意味着 变量赋值或写入内存，**

它强调的是一个写入的动作，所以 LHS 查询查的是这个变量的“家”（对应的内存空间）在哪。

``` 
var myName = name
console.log(name)
```

在这个例子里，第一行有赋值操作，但是 name 在操作的右侧，所以是 RHS；第二行没有赋值操作，name 就可以理解为没有出现在赋值操作的左侧，这种情况下我们也认为 name 的查询是 RHS。**RHS意味着变量查找或从内存中读取，它强调的是读这个动作，查询的是变量的内容。**

---

### 闭包-探索词法作用域模型

当我们在 JavaScript 语言的范畴里讨论“作用域”这个概念的时候，确实不需要区分它是“词法”还是“动态”，**因为我们 JS 的作用域遵循的就是词法作用域模型**。

但是站在语言的层面来看，作用域其实有两种主要的工作模型：

* 词法作用域：也称为静态作用域。这是最普遍的一种作用域模型。(重点)
* 动态作用域：相对“冷门”，但确实有一些语言采纳的是动态作用域，如：Bash 脚本、Perl 等

#### 词法作用域机制

> 根据函数书写(定义)时决定作用域，也被称作静态作用域。

``` 
var name = '19-Qingfeng';

function showName() {
    console.log(name);
}

function changeName() {
    var name = 'BigBear';
    showName();
}

changeName(); // 19-Qingfeng
```

因为 JS 采取的就是词法（静态）作用域，这段代码运行过程中，经历了这样的变量定位流程：

在 showName 函数的函数作用域内查找是否有局部变量 name
发现没找到，**于是根据书写的位置**，查找上层作用域（全局作用域），找到了 name 的值是 19-Qingfeng，所以结果会打印 19-Qingfeng。

> 此时他的作用域链查找规则如下

![bibao3.jpg](https://i.loli.net/2020/09/03/AsKGWavcyQF914O.png)

这里我们作用域的划分，
**是在书写的过程中（例子中也就是在函数定义的时候，块作用域同理是在代码块定义的时候），根据你把它写在哪个位置来决定的。**
像这样划分出来的作用域，遵循的就是词法作用域模型。

> 书写时showName的作用域链父亲就是global，所以自身找不到的情况下回去global去查找。

#### 动态作用域机制

> 根据函数运行时去查找作用域机制。

同样一段代码在在动态作用域运行下会有不同的结果。

* 在 showName 函数的函数作用域内查找是否有局部变量 name
* 发现没找到，**于是沿着函数调用栈、在调用了 showName 的地方继续找 name。**这时大家看看它找到哪去了？是不是就找到 changeName 里去了？ 刚好，changeName 里有一个 name，于是这个 name 就会被引用到 showName 里去。

> 动态作用域链查找规则如下:(沿着调用栈查找而非定义时去查找)

![bibao4.jpg](https://i.loli.net/2020/09/03/AgMNDWX4ZIshK6l.png)

所以动态作用域规则运行下来就会是BigBear了。

我们总结一下，词法作用域和动态作用域的区别其实在于**划分作用域的时机**：

* 词法作用域： 在代码书写的时候完成划分，作用域链沿着它**定义的位置往外延伸**
* 动态作用域： 在代码运行时完成划分，作用域链沿着它的**调用栈往外延伸**

#### 修改词法作用域(欺骗JS中的词法作用域)

##### eval

``` 
function showName(str) {
  eval(str)
  console.log(name)
}

var name = '19-Qingfeng'
var str = 'var name = "BigBear"'

showName(str) // 输出 BigBear
```

大家知道，eval 函数的入参是一个字符串。当 eval 拿到一个字符串入参后，它会把这段字符串的内容当做一段 js 代码（不管它是不是一段 js 代码），插入自己被调用的那个位置。所以上面这个例子里，被 eval “改造” 过后的 showName 函数其实长这样了：

``` 
function showName(str) {
  var name = 'BigBear'
  console.log(name)
}
```

此时当我们尝试输出 name 的时候， 函数作用域内的 name 已经被 eval 传入的这行代码给修改掉了，所以作用域内 name 的值就从 '19-Qingfeng' 变成了 ‘BigBear’（eval 带来的改变如下图所示）。而这个改变确实只有在 eval (str) 这行代码被执行后才发生 ——**eval 在运行时改变了作用域的内容**，它成功地 “修改” 了词法作用域规则约束下在书写阶段就划分好的作用域。

![bibao5.jpg](https://i.loli.net/2020/09/03/BMSuQWFeRokxdZ1.png)

##### with对于作用域的修改

先来看一段神奇的代码

``` 
function changeName(person) {
  with(person) {
    name = 'BigBear'
  }
}

var me = {
  name: '19-Qingfeng',
  career: 'coder',
  hobbies: ['coding', 'footbal']
}

var you = {
  career: 'product manager'
}

changeName(me)
changeName(you)
console.log(name) // 输出 'BigBear'
```

这其实就是 with 在 “捣鬼”。其实大家通过使用 with 的过程不难感受出来，**with 做的事情其实就是凭空创建出了一个新的作用域**。

总结下 with 改变作用域的方式：

* with 会原地创建一个全新的作用域，这个作用域内的变量集合，其实就是传入 with 的目标对象的属性集合。
* 因为 “创建” 这个动作，是在 with 代码实际已经被执行后发生的，所以这个新作用域确实是在运行时被添加的， with 因此也实现了对书写阶段就划分好的作用域进行修改。

**这里面需要注意的是，“改变” 仅仅是描述 “创建” 这个动作 —— 创建出来的这个新的作用域。因此它的作用域查询机制仍然是遵循词法作用域模型的。**

> Tips：千万不要用 with 和 eval 写代码。及时面试官问我平常对于eval和with的应用，我会告诉他不好意思我不用这两个东西。

---

### 闭包面试真题集中解析

#### 基础面试题

``` 
for (var i = 0; i < 5; i++) {
    setTimeout(function() {
        console.log(i);
    }, 1000);
}

console.log(i); // 5 5 5 5 5 
```

解决这个问题的三种思路

* 使用let声明

* 匿名函数自执行

* setTimeout传递第三个参数

#### 进阶面试题

``` 
function foo(a, b) { 
    console.log(b);
    return {
        foo: function (c) { 
            return foo(c, a); 
        }
    }
}

var func1 = foo(0); // undefined
func1.foo(1); 
func1.foo(2);
func1.foo(3); 
var func2 = foo(0).foo(1).foo(2).foo(3); 
var func3 = foo(0).foo(1); 
func3.foo(2); 
func3.foo(3); 
```

> 输出结果可以自己打印结合闭包和作用域链理解。
> 其实本质就是访问不同的作用域链。

需要注意的Tips:

* foo()和foo.foo()这两种调用方式的区别。

* func3.foo(), func3.foo()对于上一次调用并不是链式调用。 
