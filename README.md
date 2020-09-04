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

> 当然闭包的应用不仅仅限于私有变量，偏函数以及函数柯里化还有很多应用，比如封装函数，节流，防抖等等。

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
