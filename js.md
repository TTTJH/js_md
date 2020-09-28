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

