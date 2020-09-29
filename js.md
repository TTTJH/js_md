### 迭代
* forEach
	* 单纯的迭代
	* 不修改原内容
* map
	* 返回新内容
	* 不修改原内容

Array会修改原数组的方法sort,push,pop,unshift,shift,reverse,splice
### Array

-------------array修改器方法--------------------

* arr.pop()
	* 删除数组最后一个元素
	* 修改原数组
	* 返回值为 被删除元素的值
* arr.push()
	* 添加一个或多个元素到数组的末尾
	* 修改原数组
	* 返回值为 当前数组长度
* arr.shift()
	* 删除数组的第一个元素
	* 修改原数组
	* 返回值为 被删除元素的值
* arr.unshift()
	* 添加一个或多个元素到数组的开头
	* 修改原数组
	* 返回值为 当前数组长度
* arr.splice()
	* 删除或替换现有元素或添加新元素
	* 修改原数组
	* 返回值为 数组形式的被修改的内容

* arr.reverse()
	* 颠倒元素
	* 返回值为颠倒后的元素
	* 修改原数组

-------------array访问方法----------------------

* arr.concat()
	* 合并两个或者多个数组
	* 不修改原数组
	* 返回值为 合并后的新数组
* arr.join()
	* 将一个数组(类数组对象)所有元素连接为字符串
	* 不修改原数组
	* 返回值为 连接后的字符串
* arr.slice()
	* 生成由begin和end决定的原数组的浅拷贝
	* 不修改原数组
	* 返回值为 原数组的浅拷贝
* arr.toString()
	* 生成由数组元素组成的字符串
	* 不修改原数组
	* 返回值为 由数组元素组成的字符串
* arr.indexOf()
	* 返回值为 第一个匹配元素的索引
	* 不修改原数组
* arr.lastIndexOf()
	* 返回值为 数组右边开始第一个匹配元素的索引
	* 不修改原数组

### String ----- 字符串的方法都不修改原数组😳
* str.charAt()
	* 返回值为 根据索引指定的字符
	* 当然不修改原字符串

* str.concat()
	* 返回值为 一个 或 多个字符串的拼接

* str.repeat()
	* 返回值为参数个原字符串

* str.includes()
	* 用于判断字符串是否包含该参数
	* 返回值为 true 或者 false

* str.endsWith()
	* 用于判断该字符串是否已该参数结尾
	* 返回值为 true 或者 false

* str.indexOf()
	* 返回值为 参数 在字符串中位置的索引

* str.replace(arg1,arg2)
	* 返回值为 被替换后的字符串
	* 不修改原字符串

* str.slice()
	* 摘取一个字符串领域
	* 返回值为 新字符串
	* 不修改原数组

* str.split()
	* 根据参数将字符串分割成数组
	* 返回值为 字符串数组
	* 不修改原数组

* str.substring()
	* 返回值为 由开始参数和结束参数决定的字符串子集
	* 不修改原数组

### Object方法
* Object.assign()
	* 将可枚举属性值复制到目标对象
	* 返回值为 修改后的目标对象
	* 会修改原对象

* Object.entries()
	* 返回值为 一个由自身可枚举属性的键值对数组
	* 不修改原对象

* Object.keys()
	* 返回值为 自身对象可枚举属性的属性名组成的数组

* Object.values()
	* 返回值为 自身对象可枚举属性的属性值组成的数组

### 题目记录
* 当前域的cookie不全都是可以通过js直接获取的
* localStorage不支持设置过期时间，而是永久有效，sessionStorage随着网页关闭消失
* Object.assign(obj1,obj2)实现的是对象的浅拷贝
* Object.keys()不可遍历初对象原型链上的属性
* 使用 event.cancelBubble 取消冒泡
* 严格模式下：
	* 变量必须声明再使用
	* 变量不允许重复声明
	* 全局执行上下文中和全局执行上下文中的函数的this指向不再是window对象
	* 不在支持arguments
* null == undefined // true
* null === undefined // false
* null === null //true
* undefined === undefined // ture
* Infinity + 1 === Infinity
* 0.1 + 0.2 // 0.30000000000000004
* typeof NaN // number
* typeof Function // function
* typeof Object // function
* typeof {} // object
* "a" - 1 //NaN
* Function instanceof Object // true
* Object instanceod Function // true
* 定义的promise函数内部代码立刻执行
* for...in... 可以遍历对象每一个可枚举属性，包括原型链上的可枚举属性
* 使用new操作符时，构造函数内的this就指向相应的实例化对象
* ^是正则表达式匹配字符串开始位置
* $是正则表达式匹配字符串结束位置
* 400（错误请求）服务器不理解请求的语法
* 401 (身份验证错误)  此页要求授权
* 403（禁止）服务器拒绝请求
* 404（未找到）服务器找不到请求的网页
* HTML页面加载完毕触发 window.onload 事件
* JSONP是json的一种“使用模式”，可以让网页从别的域名获取资料,即跨域读取数据
* XMLHttpRequest的readyState和status
	* readyState
		* 0:请求尚未初始化
		* 1:服务器建立连接
		* 2:收到了请求	
		* 3:处理请求
		* 4:请求完成响应准备就绪
	* status
		* 200："OK"
		* 404: 找不到页面
* 执行一个XMLHttpRequest
	* xmlhttp = new XMLHttpRequest()
	* xmlhttp.onreadystatechange = function(){
	* if(xmlhttp.readyState == 4 && xmlhttp.status == 200){
	* return xmlhttp.responseText
	* }
	* }
	* xmlhttp.open("GET", url, true)
	* xmlhttp.send()
* 使用正则表达式检查字符串是否含有a
	* var reg = new RegExp("a")
	* var str = "heeloa"
	* reg.test(str) // true // 正则表达式的test方法
* 使用正则表达式检查字符串是否含有a //字面量创建
	* var reg = /a/
	* var str = "helloa"
	* reg.test(str) // true //正则表达式的test方法
* 使用正则表达式检查字符串是否含有a或者b
	* var reg = /a | b/   //var reg = new RegExp("a|b")
	* var str = "helloa"
	* reg.test(str) //true
* []在正则中也是或的意思
* [^*] 在正则中表示 除了... 的意思
* 使用正则匹配除了有a的字符串
	* var str1 = "helloa"
	* var str2 = "hello"
	* var reg = /[^a]/   // 表示被检查字符串中只要存在a之外的其他字符就返回true,即除非该字符串就为a
	* reg.test(str1) //true
	* reg.test(str2) //true
	* reg.test("a") //false	
* 使用正则表达hi匹配除了有a或者b的
	* var reg = /[^ab]/
* 重绘：
	* 重绘是指一个元素外观的改变所触发的浏览器行为，浏览器会根据元素的新属性重新绘制，使元素呈现新的外观。
* 重排：
	* 当渲染树中的一部分或全部因为元素的规模尺寸，布局，隐藏等改变而需要重新构建，这就称为回流。
* 重排发生情况：
	* 页面渲染初始化
	* 添加或删除可见的dom元素
	* 元素位置的改变
	* 浏览器窗口尺寸变化
	* 读取某些属性（offsetLedt/Top/Height/Width,clientTop/Left/Width/Height）
* 重绘发生的情况
	* 重绘发生在元素的可见外观被改变但没有影响布局的时候。
* js异步任务和同步任务流程图
	*         ______________
	*        |任务进入执行栈|
	*		||
	*               v
	*              / \
	*          判断同步还是异步
	*          /              \
	*        同步            异步
	*         |               |
	*       主线程        Event Table
        *	  |               |    
        *	  |          (注册回调函数)    
	*         |               |
	*    任务执行完毕     Event Queue
	*         |               |
	*   读取任务队列中的      |   
        * 结果，进入主线程执行____|
	
	* 同步 和 异步任务 分别进入不同的执行场所，同步任务进入主线程，异步任务进入Evenet Table 
	* 当异步任务的指定事情完成时，Event Table会讲该函数移入Event Queue
	* 主线程内的任务执行完毕为空，才会去Evenet Queue读取对应的回调函数
	* 此过程不断重复，也就是Event Loop（事件循环）
* 常见语义化标签：
	* <header></header>
	* <title></title>
	* <footer></footer>
	* <strong></strong>
	* <nav></nav>
	* <em></em>
	* <main></main>
	* 代码结构清晰，便于阅读
	* 有利于搜索引擎优化
* new操作符做了什么
	* new首先会生成一个空的对象
	* 然后构造函数中的this会指向这个空对象
	* 构造函数内的this.x = 1就相当于将1赋值给了这个空对象
	* 并且默认 return this
	* 即返回值为 this
* cookie/session实习登入保存
	* session是服务端状态保存机制
	* cookie是客户端状态保存机制
	* 每一个登入之后的用户信息都会保存在服务器session中
	* 同时服务器会把sessionid返回给客户端，
	* 客户端将sessionid存放在本地cookie中
	* 下次访问接口携带该cookie
	* 服务器比对session验证该cookie，判断用户登入
* 事件传播三个阶段：
	* 捕获阶段：	
		* 在捕获阶段时从最外层的祖先元素，向目标元素进行事件的捕获(一般不会开启)
	* 目标阶段：
		* 事件捕获到目标元素，捕获结束开始在目标元素上触发事件
	* 冒泡阶段：
		* 事件从目标元素向其祖先元素传递，依次触发祖先元素上的事件
	* 捕获阶段默认不开启，可通过设置addEventListener第三个参数为true来进行捕获和冒泡的切换
* web服务器三要素：
	* 协议(http,https)
	* 端口
	* 域名	
	* 三要素全部一致才算同源
* a标签可以包括除了自身任何元素
* h5常用标签：
	* <header></header>
	* <nav></nav>
	* <section></section>
	* <aside></aside>
	* <footer></footer>
	* <article></article>
* canvas
	* 将 渲染阶段 的开销转嫁到 计算阶段 之上
	* 使用 多个分层 的canvas绘制复杂场景
	* 不要频繁设置绘图上下文的font属性
	* 将固定的内容预先绘制在离屏canvas上以提高性能
* css权重：
	* id选择器：100
	* 类选择器：10
	* 元素选择器：1
* white-space:nowrap  元素内文字永远在一行内显示
* BEM:css命名规范
* 阻止事件默认行为：
	* preventDefault()
* 阻止冒泡：
	* stopPropagation() w3c标准的阻止冒泡
	* cancelBubble()  ie的阻止冒泡
* js模块化：
	* ES6 Module规范：
		* 模块功能主要由 export 和 import 两个命令构成。
		* export 用于定义模块的对外接口
		* import 用于输入其他模块提供的功能
		* 浏览器 和 服务端 通用
	* CommonJS规范：
		* module.exports 或者 exports 对外暴露接口
		* require命令加载其他模块
		* 主要用于服务端(nodejs)
	* AMD 规范：
		* Asynchronous Moudles Definition   异步模块定义规范
		* 该方案的实现者是RequireJS
		* 通过define定义模块
		* 通过require加载模块
* Canvas 和 SVG 都可以使用 javascript 绘制
* 如何提高网页加载速度
	* 部分操作设置 防抖 和 节流
	* 进行图片懒加载
	* 使用雪碧图
	* 增加服务器带宽
* box-sizing:
	* content-box:
		* 默认值，其中设置的width和height只包含内容的宽高，不包含内边距，边框，外边距。
		* 如果设置padding是在盒子的外部
	* border-box:
		* 其设置的width和height是包含content,padding,border，但是不包含margin的。
		* 如果设置了width和height的值，就相当于设置了content和padding
* Dom Tree 就是由各种dom节点组成的dom结构
* Render Tree 就是Dom Tree + 样式体
* 装箱：把基本数据类型 转换成对应的 引用数据类型的操作
* 拆箱：把 引用数据类型 转换成 基本数据类型 的操作
* forEach只能遍历数组
* Http本质是无状态的，使用cookies可以创建有状态的会话
* XMLHttpRequest是HTTP的API
* HTTP缓存是一种保存资源副本并在下次请求时直接使用该副本的技术,有利于缓解服务压力
* HTTP缓存但重新验证，每次有请求发出，缓存会将此请求发到服务器，服务器会验证请求所述缓存是否过期，若未过期（返回304），则缓存才使用本地缓存副本。
* CORS(跨域资源共享机制)
* 跨源域资源共享（ CORS ）机制允许 Web 应用服务器进行跨源访问控制，从而使跨源数据传输得以安全进行。
* 什么情况下需要CORS?
	* XMLHttpRequest或Fetch发起的跨源HTTP请求
	* Web字体（css中通过@font-face使用跨源字体资源）
	* WebGL贴图
* 
