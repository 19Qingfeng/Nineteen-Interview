# 19-Interview

&nbsp; &nbsp; <a  href="#1">1. JavaScript知识点</a>

&nbsp; &nbsp; &nbsp; &nbsp; <a  href="#1-1">1-1. 闭包-从编译原理角度解释词法作用域</a>

&nbsp; &nbsp; &nbsp; &nbsp; <a  href="#1-2">1-2. 闭包-探索词法作用域模型</a>

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <a  href="#1-2-1">1-2-1. 词法作用域机制</a>

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <a  href="#1-2-2">1-2-2. 动态作用域机制</a>

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <a  href="#1-2-2-1">1-2-2-1. 欺骗词法作用域</a>

&nbsp; &nbsp; &nbsp; &nbsp; <a href="#1-3">1-3. 闭包真题解析</a>

&nbsp; &nbsp; &nbsp; &nbsp; <a  href="#1-4">1-4. 闭包的应用</a>

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <a  href="#1-4-1">1-4-1. 模拟私有变量的实现</a>

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <a  href="#1-4-2">1-4-2. 偏函数和函数柯里化</a>

&nbsp; &nbsp; &nbsp; &nbsp; <a  href="#1-5">1-5. JS内存管理机制解析</a>

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <a  href="#1-5-1">1-5-1. 引用计数法</a>

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <a  href="#1-5-2">1-5-2. 标记计数法</a>

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <a  href="#1-5-3">1-5-3. 闭包和内存泄漏</a>

&nbsp; &nbsp; &nbsp; &nbsp; <a  href="#1-6">1-6. this指向原理解析</a>

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <a  href="#1-6-1">1-6-1. 普通函数this指向</a>

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <a  href="#1-6-2">1-6-2. 箭头函数this指向</a>

&nbsp; &nbsp; &nbsp; &nbsp; <a  href="#1-7">1-7. 改变this指向，深入理解call、apply、bind原理</a>

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <a  href="#1-7-1">1-7-1. 改变书写代码的方式，进而改变 this 的指向</a>

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <a  href="#1-7-1-1">1-7-1-1. 箭头函数中的this</a>

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <a  href="#1-7-1-2">1-7-1-2. 构造函数中的this</a>

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <a  href="#1-7-2">1-7-2. 显式调用一些方法来帮忙</a>

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <a  href="#1-7-2-1">1-7-2-1. call、apply、bind改变this区别</a>

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <a  href="#1-7-2-2">1-7-2-2. call、apply、bind改变this实现原理</a>

&nbsp; &nbsp; &nbsp; &nbsp; <a  href="#1-8">1-8. 执行上下文与调用栈</a>

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <a  href="#1-8-1">1-8-1. 全局上下文的创建和组成</a>

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <a  href="#1-8-1-1">1-8-1-1. 变量提升的本质</a>

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <a  href="#1-8-2">1-8-2. 函数上下文的创建和组成</a>

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <a  href="#1-8-2-1">1-8-2-1. 调用栈</a>

&nbsp; &nbsp; &nbsp; &nbsp; <a  href="#1-9">1-9. 原型编程范式与面向对象</a>

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <a  href="#1-9-1">1-9-1. 原型与原型链</a>

&nbsp; &nbsp; &nbsp; &nbsp; <a  href="#1-10">1-10. 原型与面向对象真题解析</a>

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <a  href="#1-10-1">1-10. new关键字究竟发生了什么</a>

&nbsp; &nbsp; <a  href="#2">2. JavaScript中的异步</a>

&nbsp; &nbsp; &nbsp; &nbsp; <a  href="#2-1">2-1. 异步编程模型与异步解决方案</a>

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <a  href="#2-1-1">2-1-1. 异步进化史</a>

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <a  href="#2-1-2">2-1-2. 回调函数时期以及早期解决异步途径</a>

&nbsp; &nbsp; &nbsp; &nbsp; <a  href="#2-2">2-2. 现代异步解决方案</a>

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <a  href="#2-2-1">2-2-1. Promise</a>

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <a  href="#2-2-2">2-2-2. Generator</a>

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <a  href="#2-2-3">2-2-3. Async/Await</a>

&nbsp; &nbsp; &nbsp; &nbsp; <a  href="#3">3. ES6.7.8.9.10.11</a>

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <a  href="#3-1">3-1. Promise专题问题</a>

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <a  href="#3-1-1">3-1-1. 理解Promise</a>

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <a  href="#3-1-2">3-1-2. Promise解决的问题</a>

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <a  href="#3-1-3">3-1-3. Promise常见静态方法</a>

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <a  href="#3-2">3-2. 启底PromiseA+，从零实现Promise</a>

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <a  href="#3-3">3-3. 启底PromiseA+，决议程序（Resolution Procedure）</a>

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <a  href="#3-3-1">3-3-1. Promise决议程序</a>

---

## <a name="1">JavaScript知识点</a>

---

### <a name="1-1">闭包-从编译原理角度解释词法作用域</a>

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

### <a name="1-2">闭包-探索词法作用域模型</a>

当我们在 JavaScript 语言的范畴里讨论“作用域”这个概念的时候，确实不需要区分它是“词法”还是“动态”，**因为我们 JS 的作用域遵循的就是词法作用域模型**。

但是站在语言的层面来看，作用域其实有两种主要的工作模型：

* 词法作用域：也称为静态作用域。这是最普遍的一种作用域模型。(重点)
* 动态作用域：相对“冷门”，但确实有一些语言采纳的是动态作用域，如：Bash 脚本、Perl 等

#### <a name="1-2-1">词法作用域机制</a>

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

#### <a name="1-2-2“>动态作用域机制</a>

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

#### <a name="1-2-2-1">修改词法作用域(欺骗JS中的词法作用域)</a>

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

### <a name="2">闭包面试真题集中解析</a>

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

---

### <a name="1-4">闭包的应用</a>

#### <a name="1-4-1">模拟私有变量的实现</a>

首先解释一下私有变量在JS中意味着什么：

``` 
class User {
    constructor(username, password) {
    // 用户名
    this.username = username
    // 密码
    this.password = password
  }
  
  login() {
    // 使用 fetch 进行登录请求
    fetch(登录请求的目标url地址, {
      method: 'POST', // 指定请求方法为post
      body: JSON.stringify({
        username,
        password
      }), // 请求参数带上用户名和密码
            ...  // 这里省略其它 fetch 参数
    }).then(res => res.json())
  }
}

```

在这个 User 类里，我们的本意是实现 login 这个能力，并且确保 User 的每一个实例都具备这个能力：

``` 
let user = new User('19-Qingfeng', '19-Qingfeng123')

// 输出 login 函数的内容，说明 User 的实例中有 login 这个方法
user.login
```

我们看到，login 方法已经成功的被实现了。但这里面藏着一个隐患，现在我尝试输出一下 password：

``` 
user.password // 直接打印出密码
```

> 这在业务开发中，是一个非常危险的操作：你不能保证你的队友拿到这个 user 之后不会误操作它的 password—— 你甚至不能保证三个月后的自己还会不会记得要保护这个 password！大家谨记，在软件世界中，只要是依赖人的意志才可以确保其安全稳定的东西，都是不可靠的。所以我们需要想办法从代码层面去保护 password。

像 password 这样的变量，**我们希望它仅在对象内部生效，无法从外部触及，这样的变量，就是私有变量。** 其实就是java中的private的概念。

这时候就可以使用js闭包的特性去模拟实现private的功能了。

``` 
// 利用闭包生成IIFE，返回 User 类
const User = (function () {
    // 定义私有变量_password
    let _password

    class User {
        constructor(username, password) {
            // 初始化私有变量_password
            _password = password
            this.username = username
        }

        login() {
            // 这里我们增加一行 console，为了验证 login 里仍可以顺利拿到密码
            console.log(this.username, _password)
            // 使用 fetch 进行登录请求
        }
    }

    return User
})()

let user = new User('19-Qingfeng', '19-Qingfeng123')

console.log(user.username)
console.log(user.password)
console.log(user._password)
user.login()
```

> 此时，User类被一个私有作用域包裹。该作用域内的_password和User类中的password是无法被外部访问到的。

> password和_password只能在User这个函数内使用和被访问到。

这个时候在控制台中打印出User这个类会发现他的constructor和prototype中无论如何也无法访问到password。(除非我们想让他暴露出来)

利用闭包的自由变量特性就可以完美的实现private的功能。

#### <a name="1-4-2">偏函数和函数柯里化</a>

其实柯里化和偏函数并不复杂（只是名字有点拗口），**他们都是可以帮我们把需要多个入参的函数，转化为需要更少入参的函数的方法。**

> 在计算机科学中，柯里化（英语：Currying），又译为卡瑞化或加里化，是把接受多个参数的函数变换成接受一个单一参数（最初函数的第一个参数）的函数，并且返回接受余下的参数而且返回结果的新函数的技术。

用人话稍微翻译一下:
柯里化是把**接受 n 个参数的 1 个函数**改造为**只接受 1个参数的 n 个互相嵌套的函数**的过程。也就是fn(a, b, c) 会变成fn(a)(b)(c)。

来看一个比方你就什么都明白了:

我们现在是一家电商公司，旗下有多个电商站点。为了确保商品名的唯一性，我们考虑使用 prefix（一个标识不同站点的前缀字符串）、 type（商品类型）、name（商品原本名称）三个字符串拼接的方式来为商品生成一个完整版名称。对应的方法如下：

``` 
function generateName(prefix, type, itemName) {
    return prefix + type + itemName
}
```

我们看到这个方法里需要视情况传入 prefix、type、name 参数。如果是作为一个细分工种的 leader，我可能只会负责一个站点的业务。比如我负责了 “大卖网” 的业务，那我每次生成商品名时，都会这样传参：

``` 
// itemName 是原有商品名
generateName('大卖网', type, itemName)
```

发现问题没有？这里面 prefix 其实是一个固定的入参，而我们每次都还要手动把它告诉给 generateName 函数，这很不爽。

如果是作为一个细分工种的程序员，我负责的东西可能更具体了，比如仅仅负责 “大卖网” 站点下的 “母婴” 类商品，那么我每次生成完整名称的时候，调用这个函数就是这样传参的：

``` 
// itemName 是原有商品名
generateName('大卖网', '母婴', itemName)
```

隔壁组的小哥，他只负责 “洗菜网” 站点下的 “生鲜” 类商品，那么他每次是这样传参的：

``` 
// itemName 是原有商品名
generateName('洗菜网', '生鲜', itemName)
```

一样的道理，无论是站在我的角度、还是隔壁组小哥的角度，对我们各自来说，调用 generateName 时其实真正的变量只有 itemName 一个，而我们却每次都不得不把前两个参数也手动传一遍。

此时我们多么希望，有一种魔法，可以让**函数在必要的情况下帮我们 “记住” 一部分入参**。在这个场景下，柯里化可以帮我们很大的忙。现在我们对 generateName 进行柯里化（解析在注释里）：

``` 
function generateName(prefix) {  
    return function(type) {
        return function (itemName) {
            return prefix + type + itemName
        }    
    }
}

// 生成大卖网商品名专属函数
var salesName = generateName('大卖网')

// “记住”prefix，生成大卖网母婴商品名专属函数
var salesBabyName = salesName('母婴')

// "记住“prefix和type，生成洗菜网生鲜商品名专属函数
var vegFreshName = generateName('洗菜网')('生鲜')

// 输出 '大卖网母婴奶瓶'
salesBabyName('奶瓶')
// 输出 '洗菜网生鲜菠菜'
vegFreshName('菠菜')

// 啥也不记，直接生成一个商品名
var itemFullName = generateName('洗菜网')('生鲜')('菠菜')
```

我们看到，在新的 generateName 函数中，我们可以以自由变量的形式将 prefix、type 的值保留在 generateName 内部的两层嵌套的外部作用域里。

这样一来，原有的 generateName (prefix, type, name) 现在经过柯里化已经变成了 generateName (prefix)(type)(itemName)。通过后者这种形式，我们可以选择性地决定是否要 “记住” prefix、type，从而即时地生成更加符合我们预期的、复用程度更高的目标函数。此外，柯里化还可以帮助我们以嵌套的形式把多个函数的能力组合到一起，这就是柯里化的魅力。

#### 偏函数应用与柯里化的辨析

**柯里化是将一个 n 个参数的函数转换成 n 个单参数函数。**你有 10 个入参，就得嵌套 10 层函数，且每层函数都只能有 1 个入参。它的目标就是把函数的入参拆解为精准的 n 部分。

偏函数应用相比之下就 “随意” 一些了。**偏函数是说，固定你函数的某一个或几个参数，然后返回一个新的函数（这个函数用于接收剩下的参数）**。你有 10 个入参，你可以只固定 2 个入参，然后返回一个需要 8 个入参的函数 —— **偏函数应用是不强调 “单参数” 这个概念的。它的目标仅仅是把函数的入参拆解为两部分。**

##### 偏函数应用

除了约束条件与柯里化略有不同，偏函数在动机和实现思路上都与柯里化一致 —— 动机就是为了 “记住” 函数的一部分参数，实现思路就是走闭包。

仍然是上面的例子。我们单纯地把一口气传入 3 个入参，拆分为先传 1 个、再传 2 个，这样就算实现了偏函数应用：

原有的函数形式与调用方法

``` 
function generateName(prefix, type, itemName) {
    return prefix + type + itemName
}

// 调用时一口气传入3个入参
var itemFullName = generateName('大卖网', '母婴', '奶瓶')
```

偏函数应用改造：

``` 
function generateName(prefix) {
    return function(type, itemName) {
        return prefix + type + itemName
    }
}

// 把3个参数分两部分传入
var itemFullName = generateName('大卖网')('母婴', '奶瓶')
```

当然闭包的应用不仅仅限于私有变量，偏函数以及函数柯里化还有很多应用，**[比如自行实现[Symbol. Iterator]](https://github.com/19Qingfeng/EcmaScript6-11/blob/master/src/demo/iterator.js)，封装函数，节流，防抖等等**。

---

### <a name="1-5">JS内存管理机制解析</a>

内存管理是每一种编程语言都会具备的一种基本能力。

区别在于，一些语言会将这种能力开放 —— 比如 C 语言中的 malloc() 和 free() 方法 ，这些方法的暴露，使得开发者能够切身感受到内存管理这件事情的存在。

而在另一些语言 —— 比如 JS 中，这种能力是被 “隐藏” 了的：JS 并没有暴露任何内存操作给开发者，而是自己默默地自动完成了所有的管理动作。这是 JS 内存管理不被大多数同学所重视的原因。

#### 堆内存和盏内存

##### 基本类型和引用类型

JS 中的数据类型，整体上来说只有两类：基本类型和引用类型。

其中基本类型包括：Sting、Number、Boolean、null、undefined、Symbol。这类型的数据最明显的特征是大小固定、体积轻量、相对简单，它们被放在 JS 的栈内存里存储。

而排除掉基本类型，剩下的数据类型就是引用类型，比如 Object、Array、Function 等等等等。这类数据比较复杂、占用空间较大、且大小不定，它们被放在 JS 的堆内存里存储。

``` 
let a = 0; 
let b = "Hello World" 
let c = null; 
let d = { name: '19' }; 
let e = ['19', '小明', 'bear']; 

a —— Number类型 —— 基本类型 —— 栈内存
b —— String类型 —— 基本类型 —— 栈内存
c —— null —— 基本类型 —— 栈内存
d —— Object —— 引用类型 —— 堆内存
e —— Array —— 引用类型 —— 堆内存
```

![闭包7.png](https://i.loli.net/2020/09/04/m5ApuhJafVR3ycE.png)

在访问 a、b、c 三个变量时，过程非常简单：**从栈中直接获取该变量的值**。

而在访问 d 和 e 时，则需要分两步走：

* 从栈中获取变量对应对象的引用（即它在堆内存中的地址）
* 拿着 1 中获取到的地址，再去堆内存空间查询，才能拿到我们想要的数据

#### 垃圾回收机制

> 每隔一段时间，JS 的垃圾收集器就会对变量做 “巡检”。当它判断一个变量不再被需要之后，它就会把这个变量所占用的内存空间给释放掉，这个过程叫做垃圾回收。

> 在 JS 中，我们讨论的垃圾回收算法有两种 —— 引用计数法和标记清除法。

##### <a name="1-5-1">引用计数法</a>

这是最初级的垃圾回收算法，它在现代浏览器里几乎已经被淘汰得干干净净。

**在引用计数法的机制下，内存中的每一个值都会对应一个引用计数。当垃圾收集器感知到某个值的引用计数为 0 时，就判断它 “没用” 了，随即这块内存就会被释放。**

###### 为什么淘汰引用计数

``` 
function badCycle() {
  var cycleObj1 = {}
  var cycleObj2 = {}
  cycleObj1.target = cycleObj2
  cycleObj2.target = cycleObj1
}

badCycle()
```

我们执行了 badCycle 这个函数。大家知道，函数作用域的生命非常短暂，当函数执行完之后，作用域内的变量也会全部被视作 “垃圾” 进而移除。

但如果咱们用了引用计数法，那么即使 badCycle 执行完毕，cycleObj1 和 cycleObj2 还是会活得好好的 —— 因为 cycleObj2 的引用计数为 1（cycleObj1.target），而 cycleObj1 的引用计数也为 1 （cycleObj2.target）

引用计数法对于这些循环引用的变量是无法清除的，还是会保留在内存当中。就会造成内存泄漏。

##### <a name="1-5-2">标记计数法</a>

考虑到引用计数法存在严重的局限性，自 2012 年起，所有浏览器都使用了标记清除算法。可以说，标记清除法是现代浏览器的标准垃圾回收算法。

在标记清除算法中，一个变量是否被需要的判断标准，**是它是否可抵达** 。

* 标记阶段：垃圾收集器会先找到根对象，在浏览器里，根对象是 Window；在 Node 里，根对象是 Global。从根对象出发，垃圾收集器会扫描所有可以通过根对象触及的变量，这些对象会被标记为 “可抵达”。

* 清除阶段： 没有被标记为 “可抵达” 的变量，就会被认为是不需要的变量，这波变量会被清除

``` 
function badCycle() {
  var cycleObj1 = {}
  var cycleObj2 = {}
  cycleObj1.target = cycleObj2
  cycleObj2.target = cycleObj1
}

badCycle()
```

badCycle 执行完毕后，从根对象 Window 出发，cycleObj1 和 cycleObj2 都会被识别为不可达的对象，它们会按照预期被清除掉。这样一来，循环引用的问题，就被标记清除干脆地解决掉了。

##### <a name="1-5-3">闭包和内存泄漏</a>

> 事实上，单纯由闭包导致的内存泄漏，极少极少（除非你的操作极其不规范，但那就不是闭包的问题了，是代码写得有问题）。真正导致内存泄漏的原因，我们还需要从其他方面来看。不过为了保证大家没有知识盲区，我们先从闭包对内存的 “威胁” 说起。

来看一个常见的theThing问题：

``` 
var theThing = null;
var replaceThing = function () {
  var originalThing = theThing; // 被共享
  var unused = function () {
    if (originalThing) // 'originalThing'的引用
      console.log("嘿嘿嘿");
  };
  theThing = {
    longStr: new Array(1000000).join('*'),
    someMethod: function () {
      console.log("哈哈哈");
    }
  };
};
setInterval(replaceThing, 1000);
```

**在 V8 中，一旦不同的作用域位于同一个父级作用域下，那么它们会共享这个父级作用域。**

在这段代码里， unused 是一个不会被使用的闭包，但和它共享同一个父级作用域的 someMethod，则是一个 “可抵达”（也就意味着可以被使用）的闭包。unused 引用了 originalThing，这导致和它共享作用域的 someMethod 也间接地引用了 originalThing。结果就是 someMethod “被迫” 产生了对 originalThing 的持续引用，originalThing 虽然没有任何意义和作用，却永远不会被回收。不仅如此，originalThing 每次 setInterval 都会改变一次指向（指向最近一次的 theThing 赋值结果），这导致无法被回收的无用 originalThing 越堆积越多，最终导致严重的内存泄漏。

> 在新版Chrome中已经修复了这个bug。

###### 常见一些操作失误引入的内存泄漏场景

1. 手滑导致的全局变量。

``` 
function test() {
  me = '19-Qingfeng'
}
```

当你在非严格模式下写代码时，me 而非 var me 这种写法，会导致这个 me 被默默地挂载到全局对象上。

根据我们前面所讲的垃圾回收策略，本来 me 这个变量，如果被 var 声明过，它作为函数作用域内的变量，在函数调用结束后就会消失 —— 这也是我们所期望的。但现在它是一个全局变量了，永远无法被清除。这样的变量一多，问题就来了。

2. 忘记清除的 setInterval 和 setTimeout

我们在实现轮询效果时，会用到 setInterval：

``` 
setInterval(function() {
    // 函数体
}, 1000);
或者链式调用 setTimeout：

setTimeout(function() {
  // 函数体
  setTimeout(arguments.callee, 1000);
}, 1000);
```

在 setInterval 和链式调用的 setTimeout 这两种场景下，定时器的工作可以说都是无穷无尽的。当定时器囊括的函数逻辑不再被需要、而我们又忘记手动清除定时器时，它们就会永远保持对内存的占用。因此当我们**使用定时器时，一定要先问问自己：我打算什么时候干掉这玩意儿？**

3. 清除DOM的不正当方法

``` 
const myDiv = document.getElementById('myDiv')

function handleMyDiv() {
    // 一些与myDiv相关的逻辑
}

// 使用myDiv
handleMyDiv()

// 尝试”删除“ myDiv
document.body.removeChild(document.getElementById('myDiv'));
```

针对于这段代码

``` 
document.body.removeChild(document.getElementById('myDiv'));
```

其实它仅仅是删除了myDiv这个DOM元素，在JS代码中仍然是可以抵达的，通过myDiv这个变量一直可以抵达对于该DOM的引用。这种代码如果堆积多了起来就会造成很严重的内存泄漏。

解决它的方式很简单，在删除不需要DOM的时候清空他在内存中的引用就可以了，显示赋值为null。JS就会自动帮你进行标记回收。

> 其实闭包对于内存泄漏没有很大的关系，只是说日常代码中的内存泄漏大多都是我们书写代码的不规范和对于js理解不彻底而造成。

---

### <a name="1-6">this指向原理解析</a>

#### <a name="1-6-1">普通函数this指向</a>

多数情况下，**this 指向调用它所在方法的那个对象。**

**说得更通俗点， 谁调的函数，this 就归谁。**当调用方法没有明确对象时，this 就指向全局对象。在浏览器中，指向 window；在 Node 中，指向 Global。（严格模式下，指向 undefined）

**this 的指向是在调用时决定的，而不是在书写时决定的。这点和闭包恰恰相反。**

``` 
// 声明位置
var me = {
  name: '19-Qingfeng',
  hello: function() {
    console.log( `你好，我是${this.name}` )
  }
}

var name = 'BigBear'
var hello = me.hello 

// 调用位置
me.hello() // 你好，我是19-Qingfeng
hello() // 你好， 我是BigBear 等价于window.hello() 也就等价于window.name
```

注意下面这段代码:

``` 
// 声明位置
var me = {
  name: '19-Qingfeng',
  hello: function() {
    console.log( `你好，我是${this.name}` )
  }
}

var you = {
  name: 'xiaoming',
  hello: function() {
    var targetFunc = me.hello
    targetFunc()
  }
}

var name = 'BigBear'

// 调用位置
you.hello()
```

我们再复习一下我们开头那句话 ——“this 指向调用它所在方法的那个对象”。

我们看到虽然 targetFunc 是在 you 对象的 hello 方法里声明的，但是在调用它的时候，我们是不是没有给 targetFunc 指明任何一个对象作为它前缀？ 所以 you 对象的 this 并不会神奇地自动传入 targetFunc 里，js 引擎仍然会认为 targetFunc 是一个挂载在 window 上的方法，进而把 this 指向 window 对象。

谨记，**“不管方法被书写在哪个位置，它的 this 只会跟着它的调用方走” 这个核心原则，就一定不会出错。“**

在三种特殊情境下，this 会 100% 指向 window(普通函数声明)：

* 立即执行函数（IIFE）
* setTimeout 中传入的函数
* setInterval 中传入的函数

##### 立即执行函数

所谓立即执行函数，就是定义后立刻调用的匿名函数（参见下面这道例题里 hello 方法的函数体里这种写法）。

``` 
var name = 'BigBear'

var me = {
  name: '19-Qingfeng',
  // 声明位置
  sayHello: function() {
    console.log( `你好，我是${this.name}` )
  },
  hello: function() {
    (function(cb) {
      // 调用位置
      cb()
    })(this.sayHello)
  }
}
```

me.hello() // 大家再猜下输出啥了？
经过我们楼上的提点，相信这里大家可以想都不想就说出 me.hello 的执行结果，没错，就是 BigBear ， 是 window.name 的值。

但其实，即便不考虑立即执行的匿名函数这种所谓的“特殊情况”，大家按照我们上面的指向原则来分析，结果也是一样一样的。 立即执行函数作为一个匿名函数，在被调用的时候，我们往往就是直接调用，而不会（也无法）通过属性访问器（ 即 xx.xxx） 这样的形式来给它指定一个所在对象，所以它的 this 是非常确定的，就是默认的全局对象 window。

setTimeout 和 setInterval 中传入的函数
考虑到 setTimeout 和 setInterval 中函数的 this 指向机制其实是一样的，咱们这里拿 setTimeout 来开刀就够了：

``` 
var name = 'BigBear'

var me = {
  name: '19-Qingfeng', 
  hello: function() {
    // 这里其实是 window.setTimeout(...)
    setTimeout(function() {
      console.log( `你好，我是${this.name}` )
    })

  }
}
```

me.hello() // 你好，我是BigBear
是不是觉得好神奇？我们的 this.name 明明看起来是在 me.hello () 里被调用的，结果却输出了 window.name。 setTimeout 到底对函数做了什么？

其实，我们所看到的延时效果（setTimeout）和定时效果（setInterval），都是在全局作用域下实现的。无论是 setTimeout 还是 setInterval 里传入的函数，都会首先被交付到全局对象手上。因此，函数中 this 的值，会被自动指向 window。

##### “危险” 的严格模式

在有的书籍中，也会强调 setTimeout 传入函数中 this 的值在非严格模式下指向 window 对象，在严格模式下是 undefined。好像只要加了严格模式，那么 undefined 就是一种必然 —— 确实如此吗？

事实上，严格模式确实在一些情况下会导致 this 指向 undefined， 但并非总是如此 —— 没错，事情并不简单，我们需要分情况来看：

普通函数中的 this 在严格模式下的表现
所谓 “普通函数” ，这里我们是相对于箭头函数来说的。在非严格模式下，直接调用普通函数时，正如我们开篇所说，函数中的 this 默认指向全局变量（window 或 global）：

###### 全局代码中的 this 在严格模式下的表现

所谓全局代码中的 this， 就是在全局作用域下执行的函数 / 代码段里的 this，它可以是这样的：

``` 
'use strict'

console.log(this) // 直接在全局代码里尝试去拿 this
也可以是这样的：

'use strict'

var name = 'BigBear'

var me = {
  name: '19-Qingfeng',
  hello: function() {
    // 全局作用域下实现的延时函数
    setTimeout(function() {
      console.log( `你好，我是${this.name}` )
    })
  }
}
```

me.hello() // 你好，我是BigBear
像这样处于全局代码中的 this， 不管它是否处于严格模式下，它的 this 都指向 Window（这点要特别注意，区分度非常高，很多同学面试的时候会误以为这里也是 undefined ）。

所以说，严格模式 “危险”，它危险在哪？undefined 固然可怕，它往往使我们代码报错的元凶。但站在辅助大家面试的角度，见到 ‘use strict’ 就立刻认为 this 会是 undefined ， 无疑是件更危险的事情。因此，严格模式下 this 的不同表现，还望大家牢记～

#### <a name="1-6-2">箭头函数this指向</a>

箭头函数中的 this 比较特别，它和严格模式、非严格模式啥的都没关系。它和闭包很相似，都是认“死理”—— 认“词法作用域”的家伙。**所以说箭头函数中的 this，和你如何调用它无关，由你书写它的位置决定**（和咱们普通函数的 this 规则恰恰相反～）。

* 普通函数，this指向根据调用时指向。(谁调用它它就指向谁)

* 箭头函数，this指向根据书写时指向。(定义时的位置决定)

例如：

``` 
var name = 'BigBear'
var me = {
  name: '19-Qingfeng',
  // 声明位置
  hello: () => {
      console.log(this.name)
  }
}

// 调用位置
me.hello() // BigBear

```

在这个例子里，因为 this 在书写的时候，它所在的作用域是全局作用域，于是这个 this 就和全局对象绑在了一起。

来看看这个题，搞懂了其实就差不多了：

``` 
var a = 1
var obj = {
  a: 2,
  func2: () => {
    console.log(this.a)
  },
  
  func3: function() {
    console.log(this.a)
  }
}

// func1
var func1  = () => {
  console.log(this.a)
}

// func2
var func2 = obj.func2
// func3
var func3 = obj.func3

func1()
func2()
func3()
obj.func2()
obj.func3()
```

牢记普通函数根据调用时候的规则，箭头函数是根据书写(词法作用域相似)定义时候的规则。
答案是 1、1、1、1、2。

> 关于如何改变this的指向，一些this指向的特殊用法。咱们在下一节中去探讨。

### <a name="1-7">改变this指向，深入理解call、apply、bind原理</a>

#### <a name="1-7-1">改变书写代码的方式，进而改变 this 的指向</a>

* <a name="1-7-1-1">箭头函数中的this</a>

关于箭头函数就再次强调一下：

``` 
var a = 1

var obj = {
  a: 2,
  // 声明位置
  showA: () => {
      console.log(this.a)
  }
}

// 调用位置
obj.showA() // 1
```

当我们将普通函数改写为箭头函数时，**箭头函数的 this 会在书写阶段（即声明位置）就绑定到它父作用域的 this 上。**无论后续我们如何调用它，都无法再为它指定目标对象 —— 因为箭头函数的 this 指向是静态的，“一次便是一生”。

* <a name="1-7-1-2">构造函数构造函数中的this</a>

当我们使用构造函数去 new 一个实例的时候：

``` 
function Person(name) {
  this.name = name
  console.log(this)
}

var person = new Person('19-Qingfeng')
```

构造函数里面的 this 会绑定到我们 new 出来的这个对象上：

![constructor.png](https://i.loli.net/2020/09/07/348cTfvtuWm9dA2.png)

#### <a name="1-7-2">显式地调用一些方法来帮忙</a>

<a name="1-7-2-1">改变 this 指向，我们常用的是 call、 apply 和 bind 方法。</a>

![changeThis.jpg](https://i.loli.net/2020/09/07/qNQ5gGbKvhJrxRl.png)

结合这张图来说明，会清楚得多：

call、apply 和 bind，都是用来改变函数的 this 指向的。

call、apply 和 bind 之间的区别比较大，前者在改变 this 指向的同时，也会把目标函数给执行掉；后者则只负责改造 this，不作任何执行操作。

call 和 apply 之间的区别，则体现在对入参的要求上。前者只需要将目标函数的入参逐个传入即可，后者则希望入参以数组形式被传入。

<a name="1-7-2-2">call 方法的模拟</a>
在实现 call 方法之前，我们先来看一个 call 的调用示范：

``` 
var me = {
  name: '19-Qingfeng'
}

function showName() {
  console.log(this.name)
}

showName.call(me) // 19-Qingfeng
```

结合 call 表现出的特性，我们首先至少能想到以下两点：

* call 是可以被所有的函数继承的，所以 call 方法应该被定义在 Function.prototype 上

* call 方法做了两件事：

  1. 改变 this 的指向，将 this 绑到第一个入参指定的的对象上去；

  2. 根据输入的参数，执行函数。

结合这两点，我们一步一步来实现 call 方法。首先，改变 this 的指向：

showName 在 call 方法调用后，表现得就像是 me 这个对象的一个方法一样。

所以我们最直接的一个联想是，如果能把 showName 直接塞进 me 对象里就好了，像这样：

（想得到的结果就是调用showName方法同时希望它的this指向me，那么就在me下挂载一个一模一样的showName然后自身去调用，这样就可以解决改变this指向的问题。）

``` 
var me = {
  name: '19-Qingfeng', 
  showName: function() {

    console.log(this.name)

  }
}

me.showName()
```

但是这样做有一个问题，因为在 call 方法里，me 是一个入参：

``` 
showName.call(me) // 19-Qingfeng
```

用户在传入 me 这个对象的时候， 想做的仅仅是让 call 把 showName 里的 this 给改掉，而不想给 me 对象新增一个 showName 方法。所以说我们在执行完 me.showName 之后，还要记得把它给删掉。遵循这个思路，我们来模拟一下 call 方法（注意看注释）：

``` 
Function.prototype.myCall = function(context) {

    // step1: 把函数挂到目标对象上（这里的 this 就是我们要改造的的那个函数）
    context.func = this
    // step2: 执行函数
    context.func()
    // step3: 删除 step1 中挂到目标对象上的函数，把目标对象”完璧归赵”
    delete context.func

}
```

有兴趣的同学，可以测试一下我们的 myCall:

showName.myCall(me) // 19-Qingfeng

到这里，我们已经实现了 **“改变 this 的指向”** 这个功能点。现在我们的 myCall 还需要具备**读取函数入参的能力**，类比于 call 的这种调用形式：

``` 
var me = {
  name: 'Chris'
}

function showFullName(surName) {
  console.log( `${this.name} ${surName}` )
}
```

showFullName.call(me, 'Lee') // Chris Lee

直接上代码：

``` 
Function.prototype.myCall = function(context, ...args) {
    // step1: 把函数挂到目标对象上（这里的 this 就是我们要改造的的那个函数）
    context.func = this
    // step2: 执行函数，利用扩展运算符将数组展开
    context.func(...args)
    // step3: 删除 step1 中挂到目标对象上的函数，把目标对象”完璧归赵”
    delete context.func
}
```

> 当然照着这个思路对于apply和bind的实现就特别简单了，以及对于传入null时候的逻辑判断和是否存在原本方法的方法缓存。

---

### <a name="1-8">执行上下文与调用栈</a>

为什么要有执行上下文

大家平时写项目的时候，肯定是一个文件一个文件去写；具体到每一个文件里，又会细分出不同的方法、模块 —— 我想应该不会有同学会把成千上万行的庞大的代码逻辑塞进一个文件里。当大家这样做的时候，其实已经在践行一种软件世界里非常重要的思想 —— 分治。

分治是编写软件的一种策略，它意味着你会把一个庞大的问题拆分成若干个具体的小问题，然后逐个去解决它们，以此来化解问题的复杂度。表现在代码上，就是把庞大的逻辑拆分成独立的代码块。这些 “代码块” 根据粒度的不同，有着不同的名字，它可以是函数、模块、包等等等等。

如果说把代码逻辑划分成 “块”，是我们程序员在编写阶段的智慧。那么把庞大的执行任务划分成不同的执行上下文，就是 JS 引擎在执行阶段的智慧了。

**我们可以把执行上下文理解为引擎在执行过程中对代码进行了又一次的 “划分”，这样做的目的，仍然是为了分解复杂度。**

执行上下文的分类
执行上下文主要分为三类：

* 全局上下文 —— 全局代码所处的环境，不在函数中的代码都在全局执行上下文中

* 函数上下文 —— 在函数调用时创建的上下文

* Eval 执行上下文 —— 运行 Eval 函数中的代码时所创建的环境，Eval 被前端诟病多年，时下对 Eval 感兴趣的人非常少了，面试官也普遍对它嗤之以鼻。大家答题时只需要说明 “我不用 Eval”，直接跳过这个东西就好了（还可以拉一波好感度，说明你是一个明辨是非的好孩子）。综上所述，Eval 执行上下文，不在我们本文的讨论范围内。

接下来我们就着重讲讲全局上下文和函数上下文。

#### <a name="1-8-1">全局上下文的创建和组成</a>

当我们的 JS 脚本跑起来之后，第一个被创建的执行上下文就是全局上下文。

当我们的脚本里一行代码也没有的时候里，全局上下文里会比较干净，只有两个东西：

* 全局对象（浏览器里是 Window, Node 环境下是 Global）
* this 变量。这里的 this ，指向的还是全局变量

但只要你往里面写了点东西，这个世界就会热闹起来了，比如你要敢随手写这么几句：

``` 
var name = '19-Qingfeng'
var tel = '123456'

function getMe() {

    return {
        name: name,
        tel: tel
    }

}
```

它就会变成这个样子：

![zhan1.jpg](https://i.loli.net/2020/09/07/OpobSsde9WqF61c.png)

虽然我们已经给name和tel进行了赋值，但是为什么并没有初始化值呢。

这时候其实已经结束了执行上下文第一次的生命周期(预加载阶段)，开始进入第二个生命周期。

**这里就要引出上下文的一个生命周期了，每一个执行上下文都会经历这样一个生命周期**：

* 创建阶段 —— **执行上下文的初始化状态，此时一行代码都还没有执行，只是做了一些准备工作**

* 执行阶段 —— **逐行执行脚本里的代码**

各位看到的就是创建阶段的全局上下文概览。为啥这时候变量没有值呢？这是因为创建阶段里，JS 引擎不多不少只做这么几件事：

* 创建全局对象（Window 有了）
* 创建 this ，并让它指向全局对象
* 给变量和函数安排内存空间
* 默认给变量赋值为 undefined；将函数声明放入内存
* 创建作用域链

到这里为止， 真正的赋值动作都还没有执行。所以大家先别急，我们接下来赶紧瞅一眼执行阶段的全局上下文是什么光景：

![zhan2.jpg](https://i.loli.net/2020/09/07/8HMqiTDX1ckRJpY.jpg)

这时候我们看到该有值的都有值了，这是因为 JS 引擎已经在一行一行执行代码、执行赋值操作了。

需要大家注意的是，**执行上下文在执行阶段里其实始终是处在一个动态**，比如说你执行完第一行没执行第二行的时候，这时候就只有 name 有值了， 而 tel 还是 undefined；再往下执行一行， tel 也有值了，就会看到执行上下文的内容又变了（从创建到执行完全的过程如下图）。

![test.jpg](https://i.loli.net/2020/09/07/TUqyonRsimk1uxB.jpg)

##### <a name="1-8-1-1">站在上下文角度，理解 “变量提升” 的本质</a>

之前大家理解 “变量提升”，或许更多的是靠记忆。

书本里会告诉你，在非严格模式下，当我们在没有声明一个变量就去调用它时，会出现这样的现象：

``` 
// 没有报错，而是输出 undefined
console.log(name)
```

var name = '19-Qingfeng'
JS 引擎不会抛出变量未声明的错误，而是会输出一个 undefined 值，表现得好像这个 name 变量早已被声明过一样。像这样的现象，我们叫它 “变量提升”。

现在结合我们的上下文创建过程，你会知道，**其实根本不存在任何的 “提升”，变量一直在原地。所谓的 “提升”，只是变量的创建过程（在上下文创建阶段完成）和真实赋值过程（在上下文执行阶段完成）的不同步带来的一种错觉。执行上下文在不同阶段完成的不同工作，才是 “变量提升 “的本质**。

#### <a name="1-8-2">函数上下文的创建和组成</a>

函数上下文在机制层面和全局上下文高度一致，各位只需要关注它与全局上下文之间的不同即可。**两者之间的不同主要体现在以下方面上：**

* 创建的时机 —— 全局上下文在进入脚本之初就被创建，**而函数上下文则是在函数调用时被创建**

* 创建的频率 —— 全局上下文仅在代码刚开始被解释的时候创建一次；而函数上下文由脚本里函数调用的多少决定，理论上可以创建无数次

* 创建阶段的工作内容不完全相同 —— 函数上下文不会创建全局对象（Window），而是创建参数对象（arguments）；创建出的 this 不再死死指向全局对象，而是取决于该函数是如何被调用的 —— 如果它被一个引用对象调用，那么 this 就指向这个对象；否则，this 的值会被设置为全局对象或者 undefined（在严格模式下）

除此之外，我们完全可以像理解全局上下文一样来理解函数上下文。我们仍然用一个简单的例子来看看函数上下文在不同阶段的表现:

``` 
var name = '19-Qingfeng'
var tel = '123456'

function getMe() {
    return {
        name: name,
        tel: tel
    }
}

// 增加了函数调用
getMe()
```

当引擎执行到 getMe () **调用**这一行时，首先会进入函数上下文的创建阶段，在这个阶段里，函数上下文的内容如下：

![diaoyong.jpg](https://i.loli.net/2020/09/07/3ZJl4aqowcIyuEt.png)

调用getMe时，初始化arguments以及初始化this(全局调用指向window)。

接着进入执行阶段，逐行执行函数内部的代码。此处我们只有一行代码，在代码执行过程中，没有涉及到变量的修改，因此函数上下文的内容保持不变。**执行完毕后，函数上下文的生命周期就结束了。**

#### <a name="1-8-2-1">调用栈</a>

我们看到函数执行完毕后，其对应的执行上下文也随之消失了。这个消失的过程，我们叫它” 出栈 “—— 没错，在 JS 代码的执行过程中，引擎会为我们创建” 执行上下文栈 “（也叫调用栈）。

因为函数上下文可以有许多个，我们不可能保留所有的上下文。当一个函数执行完毕，其对应的上下文必须让出之前所占用的资源。因此上下文的建立和销毁，就对应了一个” 入栈 “和” 出栈 “的操作。当我们调用一个函数的时候，就会把它的上下文推入调用栈里，执行完毕后出栈，随后再为新的函数进行入栈操作。

我们通过一个例子来理解一下这个过程：

``` 
function testA() {
  console.log('执行第一个测试函数的逻辑');
  testB();
  console.log('再次执行第一个测试函数的逻辑');
}

function testB() {
  console.log('执行第二个测试函数的逻辑');
}

testA();
```

以上这个脚本的执行上下文栈，随着代码的执行，会经历一个这样的过程：

1. 执行之初，全局上下文创建：

![func1.jpg](https://i.loli.net/2020/09/07/WRYwy1tvCTKOu9Q.png)

2. 执行到 testA 调用处，testA 对应的函数上下文创建：

![fun2.jpg](https://i.loli.net/2020/09/07/M5Szn1oNtpTVLcs.png)

3. 执行到 testB 处，testB 对应的函数上下文创建：

![fun3.jpg](https://i.loli.net/2020/09/07/WspTKdStCR6NhUQ.png)

4. testB 执行完毕，对应上下文出栈，剩下 testA 和 全局上下文：

![fun4.jpg](https://i.loli.net/2020/09/07/ifoe8Z6StHaUJIx.png)

5. testA 执行完毕，对应执行上下文出栈，剩下全局上下文：

![fun5.jpg](https://i.loli.net/2020/09/07/JUhZSgGXAano9yQ.png)

整个过程执行上下文，调用入栈出栈的过程如下：

![all.jpg](https://i.loli.net/2020/09/07/jp3OZU49K5zM61E.png)

#### 站在调用栈的角度，理解作用域的本质

作用域是什么？之前，我们认为作用域是” 访问变量的一套规则 “。**作用域其实就是当前所处的执行上下文。**我们基于执行上下文，来理解一下作用域的特征：

##### 作用域对外隔离

我们仍然用这段代码来举例：

``` 
function testA() {
  console.log('执行第一个测试函数的逻辑');
  testB();
  console.log('再次执行第一个测试函数的逻辑');
}

function testB() {
  console.log('执行第二个测试函数的逻辑');
}

testA();
```

这里，全局作用域 相对于 testA 的函数作用域，它是外部作用域；全局作用域、testA 相对于 testB 的函数作用域，它们都是外部作用域。我们知道，作用域在嵌套的情况下，**外部作用域是不能访问内部作用域的变量的。**现在，结合调用栈的情况，相信你会更清楚这其中的原因：

![all.jpg](https://i.loli.net/2020/09/07/jp3OZU49K5zM61E.png)

以 testB 为例，我们看到，最初处于外部作用域（testA、全局上下文）时，testB 对应的上下文还没有被推入调用栈；而当 testB 执行结束、代码执行退回到外部作用域时，testB 早已从栈顶弹出。这意味着，每次位于外部作用域时，testB 的执行上下文都压根不存在于调用栈内。此时就算 testA 函数上下文和全局上下文无论如何也找不到任何关于 testB 的线索，自然访问不到它内部的变量啦！

##### 闭包 —— 特殊的 “弹出”

一般来说，函数出栈后，我们都没有办法再访问到函数内部的变量了。但闭包可不是这样：

``` 
function outer(a) {
  return function inner (b) {
    return a + b;
  };
}

var addA = outer(10);

addA(20)
```

在这个例子里，inner 函数引用了 outer 函数的自由变量 a 变量，形成了一个闭包。在 outer 函数执行完毕出栈后，实际上 inner 函数仍然可以访问到这个 a 变量 ——a 变量好像没用随着 outer 函数执行上下文的消失而消失，这是为什么呢？

大家别忘了，在执行上下文的创建阶段，跟着被创建的还有作用域链！**这个作用域链在函数中以内部属性的形式存在，在函数定义时，其对应的父变量对象就会被记录到这个内部属性里。闭包正是通过这一层作用域链的关系，实现了对父作用域执行上下文信息的保留。**

自由变量的查找 —— 作用域链与上下文变量的结合
前面咱们讲了外部作用域难以 “触及” 内部作用域的原因。但反过来看，站在函数作用域内部，却可以访问到外部作用域的变量，这又是为啥呢？我们稍微改一下第一小节的代码：

``` 
var name = '19-Qingfeng'

function testA() {
  console.log('执行第一个测试函数的逻辑');
  testB();
  console.log('再次执行第一个测试函数的逻辑');
}

function testB() {
  console.log(name);
}

testA();
```

仍然说回 testB。我们看到，当代码执行到 testB 这个位置时，它位于调用栈的栈顶，此时 testA 和全局上下文都稳稳地坐在调用栈底部 —— 这首先为 testB 查找到自由变量创造了可能性。

在执行阶段，如果像例子中的 testB 一样，在函数作用域内部找不到 name 这个变量，那么引擎会沿着作用域链向上找、定位到它对应的父级作用域的上下文、看有没有目标变量，如果还没有，那么就沿着作用域链继续往上定位、直到找到为止。

**注意！这里是沿着作用域链找，可不是沿着调用栈一层一层往上找哦！**调用栈是在执行的过程中形成的，而作用域链可是在书写阶段就决定了。因此，testB 里找不到的变量，绝不会去 testA 里找，而是去全局上下文变量里找！

### <a name="1-9">原型编程范式与面向对象</a>

原型（Prototype）模式其实还是一种设计模式，同时更是一种是一种编程范式（programming paradigm）。

在原型编程范式中，我们正是通过 “复制” 来创建新对象。但这个 “复制” 未必一定要开辟新的内存、把原型对象照着再实现一遍 —— 我们复制的是能力，而不必是实体。比如在 JS 中，我们就是通过使新对象保持对原型对象的引用来做到了 “复制”。

#### JavaScript 中的 “类”

这时有一部分小伙伴估计要炸毛了：啥？？？JavaScript 只能用 Prototype？我看你还活在上世纪，ES6 早就支持类了！现在我们 JavaScript 也是以类为中心的语言了。

这波同学的思想非常危险，因为 ES6 的类其实是原型继承的语法糖:

ECMAScript 2015 中引入的 JavaScript 类实质上是 JavaScript 现有的基于原型的继承的语法糖。类语法不会为 JavaScript 引入新的面向对象的继承模型。 ——MDN

当我们尝试用 class 去定义一个 Dog 类时：

``` 
class Dog {
  constructor(name ,age) {
   this.name = name
   this.age = age
  }
  
  eat() {
    console.log('肉骨头真好吃')
  }
}
其实完全等价于写了这么一个构造函数:

function Dog(name, age) {
  this.name = name
  this.age = age
}
Dog.prototype.eat = function() {
  console.log('肉骨头真好吃')
}
```

所以说，JS 以原型作为其面向对象系统基石的本质并没有被改变。

#### <a name="1-9-1">理解原型与原型链</a>

原型编程范式的核心思想**就是利用实例来描述对象，用实例作为定义对象和继承的基础**。在 JavaScript 中，原型编程范式的体现就是基于原型链的继承。这其中，对原型、原型链的理解是关键。

原型
在 JavaScript 中，每个构造函数都拥有一个 prototype 属性，它指向构造函数的原型对象，这个原型对象中有一个 construtor 属性指回构造函数；每个实例都有一个__proto__属性，当我们使用构造函数去创建实例时，实例的__proto__属性就会指向构造函数的原型对象。

> children._proto_ === Parent.prototype

> Tips:children的_proto_是一个隐藏属性，我们无法通过普通方式直接访问到。(可以通过Reflect.has(children, "_prtot_")访问)

具体来说，当我们这样使用构造函数创建一个对象时：

``` 
// 创建一个Dog构造函数
function Dog(name, age) {
  this.name = name
  this.age = age
}
Dog.prototype.eat = function() {
  console.log('肉骨头真好吃')
}
// 使用Dog构造函数创建dog实例
const dog = new Dog('旺财', 3)
```

这段代码里的几个实体之间就存在着这样的关系：

![prototype.jpg](https://i.loli.net/2020/09/08/gItCvAVBPwSfEZX.jpg)

##### 原型链

现在我在上面那段代码的基础上，进行两个方法调用:

``` 
// 输出"肉骨头真好吃"
dog.eat()
// 输出"[object Object]"
dog.toString()
```

明明没有在 dog 实例里手动定义 eat 方法和 toString 方法，它们还是被成功地调用了。**这是因为当我试图访问一个 JavaScript 实例的属性 / 方法时，它首先搜索这个实例本身；当发现实例没有定义对应的属性 / 方法时，它会转而去搜索实例的原型对象；如果原型对象中也搜索不到，它就去搜索原型对象的原型对象，这个搜索的轨迹，就叫做原型链。**

以我们的 eat 方法和 toString 方法的调用过程为例，它的搜索过程就是这样子的：

![prtotype2.jpg](https://i.loli.net/2020/09/08/KU163dBm4tcLlWC.jpg)

楼上这些彼此相连的 prototype，就构成了所谓的 “原型链”。

注： **几乎所有 JavaScript 中的对象都是位于原型链顶端的 Object 的实例，除了 Object.prototype**（当然，如果我们手动用 Object.create(null) 创建一个没有任何原型的对象，那它也不是 Object 的实例）。

###### Object.create(a[, b])

Object.create(a)
注意：参数是直接作为实例的原型对象, a._proto_ === a。

``` 
 function People() {

    }
    People.prototype.eat = () => {
      console.log("eat")
    }
    const a = Object.create(People.prototype)

    a.eat()
```

### <a name="1-10">原型与面向对象真题解析</a>

##### 命题点一：原型基础 + 构造函数基础

``` 
var A = function() {};
A.prototype.n = 1;
var b = new A();
A.prototype = {
  n: 2,
  m: 3
}
var c = new A();

console.log(b.n);
console.log(b.m);

console.log(c.n);
console.log(c.m);

// 1 undefined 2 3
```

###### Step1：明确原型关系：

b 实例与 A 之间的关系：

![setp1.jpg](https://i.loli.net/2020/09/08/sSKYbNU5mlZzcI6.png)

c 实例与 A 之间的关系：

![setp2.jpg](https://i.loli.net/2020/09/08/GA4xWhOgoHPvM8p.png)

###### Step2：关键思路解析 - 构造函数的工作机理

相信很多同学对 c 实例没有疑问，更多是疑惑 b 实例为什么明明和 c 实例继承自一个原型，却有着不同的表现。

#### <a name="1-10-1">new关键字究竟发生了什么</a>

这里需要大家注意一个知识点：**当我们用 new 去创建一个实例时，new 做了什么？**它做了这四件事：

* 为这个新的对象开辟一块属于它的内存空间

* 把函数体内的 this 指到 1 中开辟的内存空间去并且使用this调用父类构造函数(相当于Parent.call(children))

* 将新对象的 _ proto_ 这个属性指向对应构造函数的 prototype 属性，把实例和原型对象关联起来( children._ptoto_ = Parent.prototype )

* 执行函数体内的逻辑，最后即便你没有手动 return，构造函数也会帮你把创建的这个新对象 return 出来(return this)

注意第二步哦，第二步执行完之后，**实例对象的原型就把构造函数的 prototype 的引用给存下来了**。那么在 b 实例创建的时候，构造函数的 prototype 是啥呢？就是这么个对象：

![stp3.jpg](https://i.loli.net/2020/09/08/DWGQoTHnKIwiP78.png)

所以 b 实例输出的 n 就是 1；同时由于它没有 m 属性，直接输出 undefined。

有同学会说了，可是后面我们还对 A 的 prototype 做了修改啊！b 如果存的是引用，它应该感知到我这个修改啊！注意你修改 A 的 prototype 的形式：

``` 
A.prototype = {
  n: 2,
  m: 3
}
```

**这严格意义上来说不算修改，而是一个重新赋值操作。这个动作的本质是把 A 的 prototype 指向了一个全新的 js 对象：**

由于b实例缓存的引用是之前的原型对象，现在进行了重新赋值相当于重新开辟了一片内存空间所以b仍然指向旧的引用而新创建的c实例指向的就是已经改变过后A的prototype了。

![result.jpg](https://i.loli.net/2020/09/08/WEniyZGmkDfIoAa.png)

从图中我们可以看出，A 单方面切断了和旧 prototype 的关系，而 b 却仍然保留着旧 prototype 的引用。这就是造成 b 实例和 c 实例之间表现差异的原因。

其实对比这个例子就能明白差距在哪里了：

``` 
var A = function () {};
A.prototype.n = 1;
var b = new A();
A.prototype["n"] = 2
A.prototype["m"] = 3

var c = new A();

// 原型 共享一个对象

console.log(b.n); // 2
console.log(b.m); // 3

console.log(c.n); // 2
console.log(c.m); // 3
```

他和上边的差距在于**一个是对原型对象直接的赋值(重新开辟一片地址)，一个是对原型对象属性的修改(未改变引用)**。所以造成的结果也就不同了。

##### 自有属性与原型继承属性

``` 
function A() {
    this.name = 'a'
    this.color = ['green', 'yellow']
 }
 function B() {
   
 }
 B.prototype = new A()
 var b1 = new B()
 var b2 = new B()
 
 b1.name = 'change'
 b1.color.push('black')

console.log(b2.name) // 'a'
console.log(b2.color) // ["green", "yellow", "black"]
```

好好回忆new一个对象发生了什么：
当执行到

``` 
B.prototype = new A()
```

有两步操作：

1. A.call(B.prototype):B.prototype上将会增加两个实例属性。

2. B.prototype._proto_ = A.prototype

再重新结合代码就会明白发生了什么了。

实际上b1和b2共享了一个原型链上的原型对象。

Step1：画出原型链图

这道题有一个迷惑你的地方，就是没有直接用 A 去 new 对象，而是找了一个 “中间人” B，这样就达到了把原型链复杂化的目的。不过问题不大，咱们图照画：

![setp2-1.jpg](https://i.loli.net/2020/09/08/kg347q96RbhPeOp.png)

Step2：读操作与写操作的区别
这里呢，大家看到 b1 和 b2 之间的一个区别就是 b1 有自有的 name 属性。有的同学可能会迷惑，这一行代码：

``` 
b1.name = 'change'
```

在查找 b1 的 name 属性时，难道不应该沿着原型链去找，然后定位并修改原型链上的 name 吗？

实际上，这个 “逆流而上” 的变量定位过程，当且仅当我们在进行 “读” 操作时会发生。

楼上这行代码，是一个赋值动作，是一个 “写” 操作。在写属性的过程中，如果发现 name 这个属性在 b1 上还没有，那么就会原地为 b1 创建这个新属性，而不会去打扰原型链了。

那么 color 这个属性，看上去也像是一个 “写” 操作，为什么它没有给 b2 新增属性、而是去修改了原型链上的 color 呢？首先，这样的写法：

``` 
b1.color.push('black')
```

包括这样的写法（修改对象的属性值）：

``` 
b1.color.attribute = 'xxx'
```

它实际上并没有改变对象的引用，而仅仅是在原有对象的基础上修改了它的内容而已。像这种不触发引用指向改变的操作，它走的就是 原型链 查询 + 修改 的流程，而非原地创建新属性的流程。

如何把它变成写操作呢？直接赋值：

``` 
b1.color = ['newColor']
```

这样一来，color 就会变成 b1 的一个自有属性了。 因为 [‘newColor’] 是一个全新的数组，它对应着一个全新的引用。对 js 来说，这才是真正地在向 b1 “写入” 一个新的属性。

##### 构造函数综合考察

``` 
function A() {}
function B(a) {
    this.a = a;
}
function C(a) {
    if (a) {
        this.a = a;
    }
}
A.prototype.a = 1;
B.prototype.a = 1;
C.prototype.a = 1;

console.log(new A().a); // 1
console.log(new B().a); // undefined
console.log(new C(2).a); // 2
```

此题我们仍然回想一下new发生了，new一个对象的时候，牢记返回的是new出来的实例, 以及new关键字对于实例上属性的挂载和对于原型的访问规则。

* 查找属性，实例存在返回实例属性。

* 实例不存在去实例原型上去找，找不到返回undefined。

结合我们前面对构造函数的分析，当我们像这样通过 new + 构造函数创建新对象的时候：

``` 
function C(a) {
    if (a) {
        this.a = a;
    }
}

var c = new C(2)
```

实际上发生了四件事情：

为 c 实例开辟一块属于它的内存空间
把函数体内的 this 指到 1 中开辟的内存空间去
将实例 c 的 _ proto_ 这个属性指向构造函数 C 的 prototype 属性
执行函数体内的逻辑，最后构造函数会帮你把创建的这个 c 实例 return 出来
我们基于这个结论来看 console 中的三次调用：

* new A ().a：构造函数逻辑为空，返回的实例对象 _ proto_ 中包含了 a = 1 这个属性。new A ().a 时，发现实例对象本身没有 a，于是沿着原型链找到了原型中的 a，输出其值为 1。
* new B ().a：构造函数中会无条件为实例对象创建一个自有属性 a，这个 a 的值以入参为准。这里我们的入参是 undefined，所以 a 值也是 undefined。
* new C (2).a：构造函数中会有条件地为实例对象创建一个自有属性 a—— 若确实存在一个布尔判定不为 false 的入参 a，那么为实例对象创建对应的 a 值；否则，不做任何事情。这里我们传入了 2，因此实例输出的 a 值就是 2。

其实原型上的问题，牢记new关键字发生了什么以及原型链查找规则就可以了。

以及构造继承和原型继承的区别，他们的组合继承都是必须要掌握的。

---

## <a name="2">JavaScript中的异步</a>

---

### <a name="2-1">异步编程模型与异步解决方案</a>

#### <a name="2-1-1">异步进化史</a>

异步在实现上，依赖一些特殊的语法规则。从整体上来说，异步方案经历了如下的四个进化阶段：

**回调函数 —> Promise —> Generator —> async/await**。

#### <a name="2-1-2">“回调函数” 时期</a>

所谓 “回调函数” 时期，这里严格来说指代的其实是 Promise 出现前的这么一个相对早期的阶段。在这个阶段里，回调是异步最常见、最基本的实现手段，却不是唯一的招数 —— 像事件监听、发布订阅这样的方式，也经常为我们所用。

##### 事件监听

这种形式相信每位前端同学都不陌生，给目标 DOM 绑定一个监听函数，我们用的最多的是 addEventListener：

``` 
document.getElementById('#myDiv').addEventListener('click', function (e) {
  console.log('我被点击了')
}, false);
```

通过给 id 为 myDiv 的一个元素绑定了点击事件的监听函数，**我们把任务的执行时机推迟到了点击这个动作发生时。此时，任务的执行顺序与代码的编写顺序无关，只与点击事件有没有被触发有关。**

通过给 id 为 myDiv 的一个元素绑定了点击事件的监听函数，我们把任务的执行时机推迟到了点击这个动作发生时。此时，任务的执行顺序与代码的编写顺序无关，只与点击事件有没有被触发有关。

##### 发布订阅

发布订阅，是一种相当经典的设计模式。
这里我们直接用 jQuery 中封装过的发布订阅做讲解，会更容易理解一些。
比如说我们想在名为 trigger 的信号被触发后，做点事情，我们可以订阅 trigger 信号：

``` 
function consoleTrigger() {
    console.log('trigger事件被触发')
}
jQuery.subscribe('trigger',consoleTrigger);
```

这样当 trigger 被触发时，上面对应的回调任务就会执行了：

``` 
function publishTrigger() {

    jQuery.publish('trigger');

}

// 2s后，publishTrigger方法执行，trigger信号发布，consoleTrigger就会执行了
setTimeout(publishTrigger, 2000)
```

##### 回调函数

回调函数用的最多的地方其实是在 Node 环境下，我们难免需要和引擎外部的环境有一些交流：比如说我要利用网络模块发起请求、或者要对外部文件进行读写等等。这些任务都是异步的，我们通过回调的形式来实现它们。

``` 
// -- 异步读取文件
fs.readFile(filePath,'utf8',function(err,data){
    if(err) {
      throw err;
    }
    console.log(data);// 输出文件内容
});
```

``` 
const https = require('https');
 
// 发起网络请求
https.get('目标接口', (res) => {
  console.log(data)
 
}).on("error", (err) => {
  console.log("Error: " + err.message);
});
```

##### “回调地狱”

当回调只有一层的时候，看起来感觉没什么问题。但是一旦回调函数嵌套的层级变多了之后，代码的可读性和可维护性将面临严峻的挑战。比如当我们想发起连环网络请求时：

``` 
const https = require('https');

https.get('目标接口1', (res) => {
  console.log(data)
  https.get('目标接口2', (res) => {
    https.get('目标接口3'),  (res) => {
        console.log(data)
        https.get('目标接口4', (res) => {
          https.get('目标接口5', (res) => {
            console.log(data)
            .....
            // 无尽的回调
          }
        }
    }
  }
})
```

这种情形一点也不夸张。而且其实不只是在 http、在 ajax 这样的网络请求场景里有这种谜之代码，在 “Promise 前” 的那个上古时期，我们经常被这种深不见底的回调困扰：

``` 
func1(function (resultA) {
  func2(resultA, function (resultB) {
    func3(resultB, function (resultC) {
      func4(resultC, function (resultD) {
        func5(resultD, function (resultE) {
          func6(resultE, function (resultF) {
            console.log(resultF);
            ...
            // 无尽的回调
          });
        });
      });
    });
  });
});
```

这样写代码非常糟糕，它会带来很多问题，最直接的就是：**可读性和可维护性被破坏**。

这时候如果你往里面再添油加醋，比如说加上 this、加上箭头函数、加上自由变量啥的，这段代码再过一个星期回来，你自己都很难看懂，更不要说后来的维护者了。

### <a name="2-2">现代异步解决方案</a>

#### <a name="2-2-1"> Promise

长久以来，我们一直期望着一种既能实现异步、又可以确保我们的代码好写又好看的解决方案出现。带着这样的目标，经过反复的探索，我们终于迎来了 Promise。
用 Promise 实现异步，我们这样做（这里我改造了一个网络请求的过程）：

``` 
const https = require('https');

function httpPromise(url){
  return new Promise(function(resolve,reject){
    https.get(url, (res) => {
      resolve(data);
    }).on("error", (err) => {
      reject(error);
    });
  })
}

httpPromise().then(function(data){
}).catch(function(error){})
```

可以看出，Promise 会接收一个执行器，在这个执行器里，我们需要把目标的异步任务给”填进去“。
在 Promise 实例创建后，执行器里的逻辑会立刻执行，在执行的过程中，根据异步返回的结果，**决定如何使用 resolve 或 reject 来改变 Promise实例的状态。 Promise 实例有三种状态**：

* pending 状态，表示进行中。这是 Promise 实例创建后的一个初始态；

* fulfilled 状态，表示成功完成。这是我们在执行器中调用 resolve 后，达成的状态；

* rejected 状态，表示操作失败、被拒绝。这是我们在执行器中调用 reject后，达成的状态。

在上面这个例子里，当我们用 resolve 切换到了成功态后，Promise 的逻辑就会走到 then 中的传入的方法里去；用 reject 切换到失败态后，Promise 的逻辑就会走到 catch 传入的方法中去。

这样的逻辑，本质上与回调函数中的成功回调和失败回调无异。但这种写法毫无疑问大大地提高了代码的质量。最直接的例子就是当我们进行大量的异步链式调用时，回调地狱不复存在了。取而代之的，是层级简单、赏心悦目的 Promise 调用链：

``` 
httpPromise(url1)

    .then(res => {
        console.log(res);
        return httpPromise(url2);
    })
    .then(res => {
        console.log(res);
        return httpPromise(url3);
    })
    .then(res => {
      console.log(res);
      return httpPromise(url4);
    })
    .then(res => console.log(res));。
```

#### <a name="2-2-2">Generator</a>

除了 Promise， ES2015 还为我们提供了 Generator 这个好帮手~ 。
如果你对 Generator 是什么、以及其语法特性暂时还没有太多的了解，可以点击 [这里](https://github.com/19Qingfeng/EcmaScript6-11) 先进行预备知识的学习。

Generator 一个有利于异步的特性是，它可以在执行中被中断、然后等待一段时间再被我们唤醒。通过这个“中断后唤醒”的机制，我们可以把 Generator看作是异步任务的容器，利用 yield 关键字，实现对异步任务的等待。

比如咱们用 Promise 链式调用这么写的例子：

``` 
httpPromise(url1)
    .then(res => {
        console.log(res);
        return httpPromise(url2);
    })
    .then(res => {
        console.log(res);
        return httpPromise(url3);
    })
    .then(res => {
      console.log(res);
      return httpPromise(url4);
    })
    .then(res => console.log(res));
```

其实完全可以用 yield 来这么写：

``` 
function* httpGenerator() {
  let res1 = yield httpPromise(url1)
  console.log(res);
  let res2 = yield httpPromise(url2)
  console.log(res);
  let res3 = yield httpPromise(url3)
  console.log(res);
  let res4 = yield httpPromise(url4)
  console.log(res);
}
```

现在我们想办法让 httpGenerator 按照我们的预期跑起来：我们知道，Generator 要想跑起来，需要为它创建迭代器，然后去执行这个迭代器的 next 方法。在 httpGenerator 这个例子里，**我们要想把整个函数体的逻辑走完，就必须让迭代器的 next 反复调用、直到返回值中的 done 为 true 为止。**(也就是执行完Generator函数中的所有yield)这个过程，我们当然不能手动调用，而要让程序来帮我们做：

``` 
function runGenerator(gen) {
    // 获得迭代器
    var it = gen(), ret;

    // 创造一个立即执行的递归函数
    (function iterate(val){
        // 调用Iterator对象 执行异步操作 等待httpPromise返回ret存在值
        ret = it.next(val);

        if (!ret.done) {
            // 如果能拿到一个 promise 实例
            if ("then" in ret.value) {
                // 就在它的 then 方法里递归调用 iterate
                // 等待Promise为fulfilled 
                ret.value.then( iterate );
            }
        }
    })();
}

runGenerator(httpGenerator)

```

步骤：

1. 为传入的 Generator 创建它对应的迭代器 it。然后，我们第一次调用 iterate 函数，入参为空。

2. iterate 函数内部，调用 it 的 next 方法，生成器函数开始执行，执行到第一个 yield 关键字处的逻辑执行完后暂停。它会返回一个包含了 httpPromise(url1) 这个调用返回的 promise对象（我们下文称 promise1）、以及一个 done: false 的标识，用来表示当前生成器函数内部的逻辑还没执行完（大致如下）：

``` 
{ 
  value:
   Promise {
     <pending>,
     ...// 省略一系列 promise 对象关联信息
   },
  done: false
}
```

因为 done 为 false，所以我们会进一步判断当前拿到的是否是一个 promise 对象（根据它有没有 then 属性）。判断为真后，我们在 promise1 的 then 方法里传入 iterate 函数本身。

3. promise1 的 then 方法里的 iterate 函数调用，拿到了 promise1 的返回结果（即针对 url1 的请求结果）作为入参。it.next 被第二次调用，生成器函数被“唤醒”了。注意，被“唤醒”后的生成器函数，按照流程走，它执行的第一个语句就是:

let res1 = yield httpPromise(url1)
这一步会把 next(val) 中的 val 传给 res1，而 val，恰恰就是 promise1 的返回结果。一切正如我们所预期~~

而后，生成器函数会继续执行到第二个 yield 关键字处，执行完后暂停。

此时 next 方法返回一个包含了 httpPromise(url2) 这个调用返回的 promise 对象（我们下文称 promise2）、以及一个 done: false 的标识（用来表示当前生成器函数内部的逻辑还没执行完）。因为 done 为 false，所以我们会进一步判断当前拿到的是否是一个 promise 对象（根据它有没有 then 属 性）。判断为真后，我们在 promise2 的 then 方法里传入 iterate 函数本身。

4. 循环上述过程过程，直到生成器内部逻辑执行完为止。

通过“自动执行”生成器函数对应迭代器的 next 方法，我们把异步的写法进一步优化了。它不再需要地狱般的回调，甚至不再需要 Promise 长长的链式调用，而是可以像写同步代码一样简单、清晰地实现异步特性！

不过仔细想想，咱们这个 runGenerator 其实非常简陋，它虽然体现了自动执行的思想，却不具备通用性，无法兼容更多场景——确实，要写出一个完整周到的 runGenerator 函数，不是一件轻松的事情。但是有一个好用的 runGenerator，又确实是广大开发者的强诉求。于是我们有了一个叫 co 的库，专门来封装自执行这一层的逻辑：

``` 
const co = require('co'); 
co(httpGenerator()); 
```

这里的 co，大家就可以把它看作是一个加强版的 runGenerator。我们只需要在代码里引入 co 库，然后把写好的 generator 传进去，就可以轻松地实现 generator 异步了。

#### <a name="2-2-3">Async/Await</a>

就当大家正在纷纷感慨 co 真好使，generator + promise + co 的异步方案真优雅时，更强的家伙出现了。这玩意儿甚至甩开了 co、甩开了 generator，有了它，你什么都不用操心，只需要写几个关键字，就能把异步代码处理得像同步代码一样优雅！这玩意儿就是 async/await。

它的用法非常简单。首先，我们用 **async 关键字声明一个函数为“异步函数”**：

``` 
async function httpRequest() {

}
```

然后，我们就可以在这个函数内部使用 await 关键字了：

``` 
async function httpRequest() {
  let res1 = await httpPromise(url1)
  console.log(res1)
}  
```

这个 await 关键字很绝，它的意思就是“我要异步了，可能会花点时间，后面的语句都给我等着”。当我们给 httpPromise(url1) 这个异步任务应用了 await 关键字后，整个函数会像被“yield”了一样，暂停下来，直到异步任务的结果返回后，它才会被“唤醒”，继续执行后面的语句。

是不是觉得这个“暂停”、”唤醒“的操作，和 generator 异步非常相似？事实上，async/await 本身就是 generator 异步方案的语法糖。它的诞生主要就是为了这个单纯而美好的目的——让你写得更爽，让你写出来的代码更美。

注：async/await 和 generator 方案，相较于 Promise 而言，有一个重要的优势：**Promise 的错误需要通过回调函数捕获，try catch 是行不通的。而 async/await 和 generator 允许 try/catch。**

---

## <a name="3">ES6.7.8.9.10.11</a>

[ES6-11可以参照一下我另一篇关于ES6-11的详细语法介绍。](https://github.com/19Qingfeng/EcmaScript6-11)

### <a name="3-1">Promise专题问题</a>

#### <a name="3-1-1">问：说说你理解的 Promise</a>

把握**代理对象、三个状态、状态切换机制**这三点。

Promise 对象是一个代理对象。它接受你传入的 executor（执行器）作为入参，允许你把异步任务的成功和失败分别绑定到对应的处理方法上去。一个 Promise 实例有三种状态：

* pending 状态，表示进行中。这是 Promise 实例创建后的一个初始态；

* fulfilled 状态，表示成功完成。这是我们在执行器中调用 resolve 后，达成的状态；

* rejected 状态，表示操作失败、被拒绝。这是我们在执行器中调用 reject后，达成的状态；

Promise实例的状态是可以改变的，但它只允许被改变一次。当我们的实例状态从 pending 切换为 rejected 后，就无法再扭转为 fulfilled，反之同理。当 Promise 的状态为 resolved 时，会触发其对应的 then 方法入参里的 onfulfilled 函数；当 Promise 的状态为 rejected 时，会触发其对应的 then 方法入参里的 onrejected 函数。

#### <a name="3-1-2">Promise 的出现是为了解决什么问题？</a>

不用多累赘了，callback Hell。

#### <a name="3-1-3">Promise 常见静态方法有哪些？各自是干嘛的？</a>

**all、race、reject 和 resolve, **以及ES11最新的**allSettled**。

Promise的方法有以下几种：

* Promise.all(iterable)：这个方法返回一个新的 promise 对象，该 promise 对象在 iterable 参数对象里所有的 promise 对象都成功的时候才会触发成功，一旦有任何一个 iterable 里面的 promise 对象失败则立即触发该 promise 对象的失败。

``` 
var p1 = Promise.resolve('1号选手');
var p2 = '2号选手';
var p3 = new Promise((resolve, reject) => {
  setTimeout(resolve, 100, "3号选手");
}); 
Promise.all([p1, p2, p3]).then(values => { 
  console.log(values); //  ["1号选手", "2号选手", "3号选手"]
});
```

* Promise.race(iterable)：当 iterable 参数里的任意一个子 promise 被成功或失败后，父 promise 马上也会用子 promise 的成功返回值或失败详情作为参数调用父 promise 绑定的相应处理函数，并返回该 promise 对象。

``` 
var p1 = new Promise(function(resolve, reject) { 

    setTimeout(resolve, 100, "1号选手"); 

}); 
var p2 = new Promise(function(resolve, reject) { 

    setTimeout(resolve, 50, "2号选手"); 

}); 

// 这里因为 2 号选手返回得更早，所以返回值以 2号选手为准
Promise.race([p1, p2]).then(function(value) {
  console.log(value); //  "2号选手"
}); 
```

* Promise.reject(reason)： 返回一个状态为失败的Promise对象，并将给定的失败信息传递给对应的处理方法

* Promise.resolve(value)：它返回一个 Promise 对象，但是这个对象的状态由你传入的value决定，情形分以下两种：

  + 如果传入的是一个带有 then 方法的对象（我们称为 thenable 对象），返回的Promise对象的最终状态由then方法执行决定

  

  + 否则的话，返回的 Promise 对象状态为 fulfilled，同时这里的 value 会作为 then 方法中指定的 onfulfilled 的入参

* Promise.allSettled(iterable)

ES11提出了Promise.allSettled()，它的出现就是为了解决Promise.all()的痛点。

接受一个Iterator对象，相较于all方法。无论iterable中哪一个失败或者成功它最终都会返回一个数组，数组中按照顺序包含每一个Promise返回的对象。

* 当某一个Promise成功时候，返回的 { status: 'fulfilled', value: { // resolve的value } }, 

* 当某一个失败时，数组内部对应元素返回 { status: 'rejected', reason: { //reject的值 } }, 

* 注意成功是value，失败是reason。

总之它解决的就是Promise.all() 具有并发执行异步任务的能力。但它的最大问题就是如果其中某个任务出现异常(reject)，所有任务都会挂掉，Promise直接进入 reject 状态。

如果并发任务中，allSettled无论一个任务正常或者异常，都会返回对应的的状态。

#### 真题

##### First

``` 
const promise = new Promise((resolve, reject) => {
    console.log(1);
    resolve();
    console.log(2);
});

promise.then(() => {
    console.log(3);
});

console.log(4);
```

运行结果：

``` 
1
2
4
3
```

考点点拨：Promise 中的处理函数是异步任务

then 方法中传入的任务是一个异步任务。resolve() 这个调用，作用是将 Promise 的状态从 pending 置为 fulfilled，这个新状态会让 Promise 知道“我的 then 方法中那个任务可以执行了”——注意是”可以执行了“，而不是说”立刻就会执行“。毕竟作为一个异步任务，它的基本修养就是要等同步代码执行完之后再执行。所以说数字 3 的输出排在最后。

##### Second

``` 
const promise = new Promise((resolve, reject) => {
  resolve('第 1 次 resolve')
  console.log('resolve后的普通逻辑')
  reject('error')
  resolve('第 2 次 resolve')
})
 
promise
.then((res) => {
  console.log('then: ', res)
})
.catch((err) => {
  console.log('catch: ', err)
})
```

运行结果：

``` 
resolve后的普通逻辑
then:  第 1 次 resolve
```

考点点拨：Promise 对象的状态只能被改变一次
分析：这段代码里，promise 初始状态为 pending，我们在函数体第一行就用 resolve 把它置为了 fulfilled 态。这个切换完成后，后续所有尝试进一步作状态切换的动作全部不生效，所以后续的 reject、resolve大家直接忽略掉就好；需要注意的是，**我们忽略的是第一次 resolve 后的 reject、resolve，而不是忽略它身后的所有代码。**因此 console.log(‘resolve后的普通逻辑’) 这句，仍然可以正常被执行。至于这里为啥它输出在 ”then: 第 1 次 resolve“ 的前面，原因和真题1是一样一样的~

##### Third

``` 
Promise.resolve(1)
  .then(Promise.resolve(2))
  .then(3)
  .then()
  .then(console.log)
```

运行结果：

``` 
1
```

###### Promise 值穿透问题

分析：大家知道，then 方法里允许我们传入两个参数：onFulfilled（成功态的处理函数）和 onRejected（失败态的处理函数）。

你可以两者都传，也可以只传前者或者后者。**但是无论如何，then 方法的入参只能是函数。万一你想塞给它一些乱七八糟的东西，它就会“翻脸不认人”。**

具体到我们这个题里，第一个 then 方法中传入的是一个 Promise 对象，then 说：”我不认识“；第二个 then 中传入的是一个数字， then 继续说”我不认识“；第四个干脆啥也没穿，then 说”入参undefined了，拜拜“；直到第五个入参，一个函数被传了进来，then 哭了：”终于等到一个我能处理的！“，于是只有最后一个入参生效了。

在这个过程中，**我们最初 resolve 出来那个值，穿越了一个又一个无效的 then 调用，就好像是这些 then 调用都是透明的、不存在的一样，因此这种情形我们也形象地称它是 Promise 的“值穿透”。**

需要注意console.log也是函数。

### <a  name="3-2">PromiseA+，从零实现Promise</a>

``` 
new Promise((resolve, reject) => {
    resolve("success")
}).then(resolve => {
    console.log(resolve, 'resolve')
})
```

我们现在回忆一下之前咱们用过的 Promise。从使用的感受上来说，一个 Promise 应该具备的最基本的特征，至少有以下两点：

* 可以接收一个 executor 作为入参

* 具备 pending、resolved 和 rejected 这三种状态

我们先从这最基本的轮廓入手（解析在逐行注释里，本节注释非常重要）：

``` 
function CutePromise(executor) {
    // value 记录异步任务成功的执行结果
    this.value = null;
    // reason 记录异步任务失败的原因
    this.reason = null;
    // status 记录当前状态，初始化是 pending
    this.status = 'pending';
     
    // 把 this 存下来，后面会用到
    var self = this;
  
    // 定义 resolve 函数
    function resolve(value) {
        // 异步任务成功，把结果赋值给 value
        self.value = value;
        // 当前状态切换为 resolved
        self.status = 'resolved'; 
    }
    
    // 定义 reject 函数
    function reject(reason) {
        // 异步任务失败，把结果赋值给 value
        self.reason = reason; 
        // 当前状态切换为 rejected
        self.status = 'rejected';
    }
  
    // 把 resolve 和 reject 能力赋予执行器
    executor(resolve, reject);
}
```

#### then 方法的行为

每一个 promise 实例一定有个 then 方法，由此我们不难想到，then 方法应该装在 Promise 构造函数的原型对象上（解析在逐行注释里，本节注释非常重要）：

``` 
// then 方法接收两个函数作为入参（可选）
CutePromise.prototype.then = function(onResolved, onRejected) {
  
    // 注意，onResolved 和 onRejected必须是函数；如果不是，我们此处用一个透传来兜底
    if (typeof onResolved !== 'function') {
        onResolved = function(x) {return x};
    }
    if (typeof onRejected !== 'function') {
        onRejected = function(e) {throw e};
    }

    // 依然是保存 this
    var self = this;
    // 判断是否是 resolved 状态
    if (self.status === 'resolved') {
        // 如果是 执行对应的处理方法
        onResolved(self.value);
    } else if (self.status === 'rejected') {
        // 若是 rejected 状态，则执行 rejected 对应方法
        onRejected(self.reason);
    }
};
```

来试试成果：

``` 
new CutePromise(function (resolve, reject) {
    resolve('成了！');
}).then(function (value) {
    console.log(value);
}, function (reason) {
    console.log(reason);
});

// 输出 “成了！”

new CutePromise(function (resolve, reject) {
    reject('错了！');
}).then(function (value) {
    console.log(value);
}, function (reason) {
    console.log(reason);
});

// 输出“错了！”
```

#### 链式调用

想必大家还记得，在 Promise 中，then 方法和 catch 方法都是可以通过链式调用这种形式无限调用下去的。这里先给大家透个底儿：Promise/A+ 规范里，其实压根儿没提 catch 的事儿，它只强调了 then 的存在、约束了 then 的行为。所以咱们此处，就是要实现 then 的链式调用。

要想实现链式调用，咱们考虑以下几个重大的改造点：

* then方法中应该直接把 this 给 return 出去（链式调用常规操作）；

* 链式调用允许我们多次调用 then，多个 then 中传入的 onResolved（也叫onFulFilled） 和 onRejected 任务，我们需要把它们维护在一个队列里；

* **要想办法确保 then 方法执行的时机，务必在 onResolved 队列 和 onRejected 队列批量执行前**。不然队列任务批量执行的时候，任务本身都还没收集完，就乌龙了。一个比较容易想到的办法就是把**批量执行这个动作包装成异步任务**，这样就能确保它一定可以在同步代码之后执行了。

OK，明确了改造点之后，咱们动手来完善构造函数这一侧的代码：

``` 
function CutePromise(executor) {
    // value 记录异步任务成功的执行结果
    this.value = null;
    // reason 记录异步任务失败的原因
    this.reason = null;
    // status 记录当前状态，初始化是 pending
    this.status = 'pending';
  
    // 缓存两个队列，维护 resolved 和 rejected 各自对应的处理函数
    this.onResolvedQueue = [];
    this.onRejectedQueue = [];
         
    // 把 this 存下来，后面会用到
    var self = this;
  
    // 定义 resolve 函数
    function resolve(value) {
        // 如果不是 pending 状态，直接返回
        if (self.status !== 'pending') {
            return;
        }
        // 异步任务成功，把结果赋值给 value
        self.value = value;
        // 当前状态切换为 resolved
        self.status = 'resolved'; 
        // 用 setTimeout 延迟队列任务的执行
        setTimeout(function(){
            // 批量执行 resolved 队列里的任务
            self.onResolvedQueue.forEach(resolved => resolved(self.value)); 
        });
    }
        
    // 定义 reject 函数
    function reject(reason) {
        // 如果不是 pending 状态，直接返回
        if (self.status !== 'pending') {
            return;
        }
        // 异步任务失败，把结果赋值给 value
        self.reason = reason; 
        // 当前状态切换为 rejected
        self.status = 'rejected';
        // 用 setTimeout 延迟队列任务的执行
        setTimeout(function(){
            // 批量执行 rejected 队列里的任务
            self.onRejectedQueue.forEach(rejected => rejected(self.reason));
        });
    }
  
    // 把 resolve 和 reject 能力赋予执行器
    executor(resolve, reject);
}
```

相应地，then 方法也需要进行改造。除了返回 this 以外，现在我们会把 resolved 和 rejected 任务没有完全被推入队列时的情况，全部视为 pending 状态。于是在 then 方法中，我们还需要对 pending 做额外处理：

``` 
// then 方法接收两个函数作为入参（可选）
CutePromise.prototype.then = function(onResolved, onRejected) {
  

    // 注意，onResolved 和 onRejected必须是函数；如果不是，我们此处用一个透传来兜底
    if (typeof onResolved !== 'function') {
        onResolved = function(x) {return x};
    }
    if (typeof onRejected !== 'function') {
        onRejected = function(e) {throw e};
    }

 

    // 依然是保存 this
    var self = this; 
    // 判断是否是 resolved 状态
    if (self.status === 'resolved') {
        // 如果是 执行对应的处理方法
        onResolved(self.value); 
    } else if (self.status === 'rejected') {
        // 若是 rejected 状态，则执行 rejected 对应方法
        onRejected(self.reason); 
    } else if (self.status === 'pending') {
        // 若是 pending 状态，则只对任务做入队处理
        self.onResolvedQueue.push(onResolved); 
        self.onRejectedQueue.push(onRejected); 
    }
    return this

}; 
```

使用ES6让代买看起来更加简洁：

``` 
class CutePromise {
    constructor(executor) {

        const resolve = (res) => {
            if (this.status === 'pending') {
                this.value = res;
                this.status = 'resolve'
                setTimeout(() => {
                    this.resolvedQueue.forEach(resolve => resolve(res))
                })
            }
        }

        const reject = (rej) => {
            if (this.status === 'pending') {
                this.reason = rej
                this.status = 'reject'
                setTimeout(() => {
                    this.rejectedQueue.forEach(resolve => resolve(rej))
                })
            }
        }

        this.value = null
        this.reason = null
        this.resolvedQueue = []
        this.rejectedQueue = []
        this.status = 'pending'

        executor(resolve, reject)
    }

    then(onResolved, onRejected) {
        if (typeof onResolved !== 'function') {
            onResolved = function (x) {
                return x
            };
        }
        if (typeof onRejected !== 'function') {
            onRejected = function (e) {
                throw e
            };
        }
        if (this.status === 'resolve') {
            onResolved(this.value)
        } else if (this.status === 'reject') {
            onRejected(this.reason)
        } else {
            this.resolvedQueue.push(onResolved)
            this.rejectedQueue.push(onRejected)
        }
        return this
    }
}

const cutePromise = new CutePromise(function (resolve, reject) {
    resolve('成了！');
});
cutePromise.then((value) => {
    console.log(value)
    console.log('我是第 1 个任务')
}).then(value => {
    console.log('我是第 2 个任务')
});
```

### <a  name="3-3">启底Promise/A+, 决议程序（Resolution Procedure）</a>

我们上一节写出来这个 Promise，最明显的一个缺陷就是下一个 then 拿不到上一个 then 的结果。

多次then调用拿到的resolve的值全是第一次resolve的值。

#### <a name='3-3-1'>重新审视 then 方法——理解 Promise 决议程序</a>

前面我们说过，整个 Promise 规范，在方法层面，基本就是围绕着 then 打转。 其中一个最需要引起大家注意的东西叫做 Promise Resolution Procedure(Promise决议程序)。这个名字翻译过来很绕，尤其是“决议”这个动作，看上去挺唬人的。**其实这里的“决议”，描述的就是 resolve 这个动作。决议程序，约束的就是 resolve 应该如何表现。**这个动作和 then 息息相关，所以要想把 then 方法完善起来，我们必须对决议程序的内容有细致的了解。我们一起来看看 Promise/A+ 规范中的相关内容：

决议程序处理是以一个promise和一个value为输入的抽象操作，我们把它表示为

``` 
[[Resolve]](promise, x)
```

笔者注：别懵。这种形式看起来太高级了一点也不友好，但这种写法你肯定见过：

``` 
promise2 = promise1.then(onFulfilled, onRejected);
```

[[Resolve]](promise, x)。**意思是说如果onFulfilled 或 onRejected 返回了值x， 则执行 Promise 解析流程 [[Resolve]](promise2, x)。**

> 其实关于Promise/A+规范以及决议程序我个人理解是从倒着去推。

* 平常使用的时候then方法中我们返回一个非Promise对象, 相当于直接resolve(非Promise对象)。

* 其实决议程序通俗点说就是决定Promise中then返回值的状态。

*PromiseA+决议程序稍后再进行总结，没有完全吃透。。先放一放*
