## python-interview

##### 为什么学python

[为什么xuepython](https://blog.csdn.net/Darkman_EX/article/details/81101232)

* 答题路线：a、python的优点，b、python的应用领域广
* 具体：
    * 优点
        * 1、python语法非常优雅，简单易学
        *  2、免费开源
        *  3、跨平台，可以自由移植
        *  4、可扩展，可嵌入性强
        *  5、第三方库丰富

    * 应用领域
        * 1、在系统编程中应用广泛，比如说shell工具。
        * 2、在网络爬虫方面功能非常强大，常用的库如scrapy，request等
        * 3、在web开发中使用也很广泛，如很多大型网站都用python开发的，如ins，youtube等，常用的框架如django，flask等
        * 4、python在系统运维中应用广泛，尤其在linux运维方面，基本上都是自动化运维。
        * 5、在人工智能，云计算，金融等方面也应用非常广泛。


##### 通过什么途径学习python

* 通过看官方文档
* 通过哔哩哔哩上的视频教程
* 通过百度查资料
* 通过买python相关方面的书


##### 公司线上和开发环境使用的什么系统

* 线上用的centos和Ubuntu系统
* 开发环境用的windows，mac，还有Ubuntu。


##### python和java、php、c、c#、c++ 等其他语言对比？

* Java C# PHP Python (开发效率高)，这些语言本身不需要你去管理内存了。它们都有自己的虚拟机，对于开辟内存、释放内存都由这个虚拟机处理。
* C 和 Python、Java、C#等C语言： 代码编译得到 机器码 ，机器码在处理器上直接执行，每一条指令控制CPU工作其他语言： 代码编译得到 字节码 ，虚拟机执行字节码并转换成机器码再后在处理器上执行Python 和 C Python这门语言是由C开发而来　　
* 对于使用：Python的类库齐全并且使用简洁，如果要实现同样的功能，Python 10行代码可以解决，C可能就需要100行甚至更多.
* 对于速度：Python的运行速度相较与C，绝逼是慢了Python 和 Java、C#等　　
* 对于使用：Linux原装Python，其他语言没有；以上几门语言都有非常丰富的类库支持
* 对于速度：Python在速度上可能稍显逊色所以，Python和其他语言没有什么本质区别，其他区别在于：擅长某领域、人才丰富、先入为主


##### 简述解释型和编译型编程语言

* 解释型语言编写的程序不需要编译，在执行的时候，专门有一个解释器能够将VB语言翻译成机器语言，每个语句都是执行的时候才翻译。这样解释型语言每执行一次就要翻译一次，效率比较低。
* 用编译型语言写的程序执行之前，需要一个专门的编译过程，通过编译系统，把源高级程序编译成为机器语言文件，翻译只做了一次，运行时不需要翻译，所以编译型语言的程序执行效率高，但也不能一概而论，部分解释型语言的解释器通过在运行时动态优化代码，甚至能够使解释型语言的性能超过编译型语言。

##### python解释器种类以及特点

* CPython
    * c语言开发的 使用最广的解释器
* IPython
    * 基于cpython之上的一个交互式计时器 交互方式增强 功能和cpython一样
* PyPy
    * 目标是执行效率 采用JIT技术 对python代码进行动态编译，提高执行效率
* JPython
    * 运行在Java上的解释器 直接把python代码编译成Java字节码执行
* IronPython
    * 运行在微软 .NET 平台上的解释器，把python编译成. NET 的字节码


##### 位和字节的关系
* 8位=一字节

##### b、B、kB、MB、GB的关系
1. 1B=8b
2. 1kB=1024B
3. 1MB=1024kB
4. 1GB=1024MB


##### 请列出至少5个PEP8规范

[PEP8规范](https://www.jianshu.com/p/e132bea1d2c9)
* 每个缩进级别使用4个空格
* 每行代码的最大长度限制为79个字符
* 若是导入多个库函数，应该分开依次导入
    * 道路应按照以下顺序导入
        a、标准库导入
        b、相关的第三方库导入
        c、本地应用程序的库导入
* 在表达式中避免无关的空格
    * 在括号或者大括号内
    * 在尾随逗号和后面的右括号之间
    * 在逗号，分号或者冒号前面
    * 函数名的与后面的参数的括号之间
* 代码更改时，相应的注释也要随之更改
* 命名要规范，通俗易懂
    
    
##### or 和 and
* v1=1 or 3
* v2=1 and 3
* v3=0 and 2 and 1
* v4=0 and 2 or 1
* v5=0 and 2 or 1 or 4
* v6=0 or False and 1

* 结果：
       * v1 = 1
       * v2 = 3
       * v3 = 0
       * v4 = 1
       * v5 = 1
       * v6 = False
 * 基本运算规律
    1.  在不加括号时候, and优先级大于or
    2.  x or y 的值只可能是x或y. x为真就是x, x为假就是y
    3.  x and y 的值只可能是x或y. x为真就是y, x为假就是x


##### ascii、Unicode、utf-8、gbk的区别
* ascii 是最早美国用的标准信息交换码，把所有的字母的大小写，各种符号用 二进制来表示，共有256中，加入些拉丁文等字符，1bytes代表一个字符
* Unicode是为了统一世界各国语言的不用，统一用2个bytes代表一个字符，可以表达2^16=65556个，称为万国语言，特点：速度快，但浪费空间
* utf-8 为了改变Unicode的这种缺点，规定1个英文字符用1个字节表示，1个中文字符用3个字节表示，特点；节省空间，速度慢，用在硬盘数据传输，网络数据传输，相比硬盘和网络速度，体现不出来的
* gbk  是中文的字符编码，用2个字节代表一个字符


##### 字节码和机器码的区别
* 机器码是电脑CPU直接读取运行的机器指令，运行速度最快，但是非常晦涩难懂，也比较难编写，一般从业人员接触不到。
* 字节码是一种中间状态（中间码）的二进制代码（文件）。需要直译器转译后才能成为机器码。

##### 三元运算编写格式
* 表达式1 if 布尔表达式2 else 表达式3
* 例如：a=3 if 3 > 4 else 5 


##### 列举你所了解的所有Python2和Python3的区别
[python2和python3的区别](https://blog.csdn.net/weixin_41819299/article/details/81259721)
1. python2没有nonlocal关键字，要修改临时变量只能将其改成可变数据类型，如数组。b=[a]
2. print()函数代替print语句
3.  Python3加入 Unicode 字符串，用以编码存储字符串。比如用 utf-8可以用来输入中文
4.  Python3去掉long类型，新增了bytes。
5.  Python 3整数之间做除法可以得到浮点数的结果，不需要进行数据格式转换1/2=0.5 Python 2整数int间除法结果为把运算结果去尾的整数1/2=0，3/2.0=1.5
6.   Python3 中 range()，Python2 中 xrange()。
7.   python2中的不等于号可以是!=或者<>，python3只能是!=
8.   python2中raw_input()用来输入字符串，而python3中使用input()来输入字符串

##### py2项目如何迁移成py3
1. 先备份原文件，然后使用python3自带工具2to3.py将py2文件转换位py3文件
2. 手动将不兼容的代码改写成兼容py3的代码

##### 用一行代码实现数值交换
* a=1
* b=2
* 答案：a,b=b,a

##### python3和python2中int和long的区别
* python2中有long类型，python3中没有long类型，只有int类型。python3中的int类型包括了long类型。

##### xrange和range的区别
* xrange和range用法相同，但是xrange是一个生成器，range结果是一个列表。xrange做循环的时候性能比range好。

##### 如何实现字符串的反转？如：name=felix，反转成name=xilef

```python
    name = "felix"
    # 方法一：
    name=name[::-1]
    # 方法二：
    name2=list(name)
    name2.reverse()
    name=''.join(name2)
    # 方法三：
    from functools import reduce
    name=reduce(lambda x, y: y+x, name)
```

##### 文件操作时，xreadlines和readlines的区别

* xreadlines返回的是一个生成器
* readlines返回的是一个列表

##### 请列举布尔值位False的常见值

* 0、''、[]、{}、tuple()、None、set()

##### 列举字符串、列表、元组、字典每个常用的5个方法
* 字符串---[字符串方法总结](https://www.cnblogs.com/chendai21/p/8137285.html)
    1. strip() ->去掉字符串两端的空白符
    2. split() ->对字符串进行分割，默认按照空格分割
    3. join() ->字符串连接
    4. startwith(),endwith() ->判断是否以啥开头或者结尾
    5. replace() -> 字符串替换
    6. find() -> 查找字符串，存在返回第一个索引，不存在返回-1
* 列表---[列表方法总结](https://www.cnblogs.com/smelond/p/7857701.html)
    1. count() ->统计在列表中出现的个数
    2. apped() ->在列表末尾添加值
    3. pop() ->删除一个对象，默认最后一个
    4. remove() ->删除指定的第一个匹配项
    5. insert() ->插入对象
    6. index() ->获取索引
 * 元组
     1. count() ->统计在元组中出现的个数
     2. index() ->获取索引
 * 字典
     1. keys() ->获取所有的键
     2. pop() ->删除指定的键的键值对
     3. popitem() ->随机删除一个键值对
     4. update() ->更新字典，参数为一个字典，如果键已存在，则更改，不存在则添加
     5. setdefault() ->如果键存在则，返回该键对应的值，如果不存在，设置该键为设置的默认值，然后返回该键对应的值
     6. get() ->返回键对应的值
     7. fromkeys() ->创建字典，第一个参数为可迭代对象，每个值变成字典的键，第二个参数为每个键的默认值

##### is和==的区别
* is比较的是两个对象的id是否相同
* ==比较的是两个对象的值是否相同

##### 1，2，3，4，5能组成多少个互不相同且不重复的三位数？
* 排列组合问题： 5\*4\*3=60个

##### 什么是反射，以及应用场景
[什么是反射的解释](https://www.cnblogs.com/IT-Scavenger/p/9394306.html)

* 反射就是通过字符串的形式，导入模块；通过字符串的形式，去模块寻找指定函数，并执行。利用字符串的形式去对象（模块）中操作（查找/获取/删除/添加）成员，一种基于字符串的事件驱动！
* 应用场景：当我们动态的输入一个模块名的时候就可以使用到反射。
* 通过hasattr，getattr，delattr，setattr等四个函数来操作

##### 简述python的深浅拷贝
* 浅拷贝只是对另外一个变量的内存地址的拷贝，这两个变量指向同一个内存地址的变量值。
    * 浅拷贝的特点：
        * 共用一个值
        * 这两个变量的内存地址一样
        * 对其中一个变量的值改变，另外一个变量的值也会改变
* 深拷贝是一个变量对另外一个变量的值拷贝
    * 深拷贝的特点：
        * 两个变量的内存地址不同
        * 两个变量各有自己的值，且互不影响
        * 对其任意一个变量的值的改变不会影响另外一个
* 如果是不可变类型，则深浅拷贝只拷贝引用，如果是可变类型，浅拷贝只拷贝第一层引用，深拷贝无论多少层引用都拷贝


##### python的垃圾回收机制
[python垃圾回收机制详解](https://testerhome.com/topics/16556)

* 概述：python采用的是引用计数机制为主，标记-清除和分代收集两种机制为辅的策略
* 引用计数：
    * 每当新的引用指向该对象时，引用计数加1，当对该对象的引用失效时，引用计数减1，当对象的引用计数为0时，对象被回收。缺点是，需要额外的空间来维护引用计数，并且无法解决对象的循环引用。
* 分代回收：（具体见上面链接）
    * 以时间换空间的回收方式
* 标记清除：
    * 活动对象会被打上标记，会把那些没有被打上标记的非活动对象进行回收。


##### python的可变类型和不可变类型的区别
* 可变类型有：列表，字典等
* 不可变类型有：数字，字符串，元组等
* 这里的可变不可变是指内存中的那块内容是否可以被改变。


##### 求下面代码结果
```python
v=dict.fromkeys(['k1','k2'],[])
v['k1'].append(666)
print(v)
v['k1']=777
print(v)
```
* 结果：
{'k1': [666], 'k2': [666]}
{'k1': 777, 'k2': [666]}


##### 一行代码实现删除列表中的所有的重复的值
```python
lis=[1,1,2,1,22,5]
lis=list(set(lis))
```

##### 如何实现"1.2.3"变成['1','2','3']?
```python
s="1,2,3"
s=s.split(',')
```

##### 如何实现['1','2','3']变成[1,2,3]
```python
ss=['1', '2', '3']
ss=[int(i) for i in ss]
```

##### 比较：a=[1,2,3]和b=[(1),(2),(3)]以及c=[(1,),(2,),(3,)]的区别
* a和b的结果相同，列表里面的值相同，类型也相同
* c中的列表里面的值是元组类型的


##### 如何用一行代码生成[1,4,9,16,25,36,49,64,81,100]?
```python
lis=[i**2 for i in range(1,11)]
```

##### 常用字符串格式化有哪几种？
1. 使用百分号
```python
print('hello %s and %s'%('friend','another friend'))
```
2. 使用format
```python
print('hello {first} and {second}'.format(first='friend',second='another friend'))
```

##### 什么是断言(assert)?应用场景？
[断言的参考](https://blog.csdn.net/shujuanyaning/article/details/47184541)

* assert是用来检查一个条件，如果它为真，就不做任何事。如果它为假，则会抛出AssertError并且包含错误信息。
* 应用场景：
    1. 防御型编程
    2. 运行时检查程序逻辑
    3. 检查约定
    4. 程序常量
    5. 检查文档

##### 有两个字符串列表a和b，每个字符串是由逗号隔开的一些字符
```python
a=[
    'a,1',
    'b,3,22',
    'c,3,4',
]
b=[
    'a,2',
    'b,1',
    'd,5',
]
# 按照a，b中每个字符串的第一个值，合并成c如下：
c=[
    'a,1,2',
    'b,3,22,1',
    'c,3,4',
    'd,5'
]
```
```python
# 解法：

a=[
    'a,1',
    'b,3,22',
    'c,3,4',
]
b=[
    'a,2',
    'b,1',
    'd,5',
]
a_dic={}
for s in a:
    k,v = s.split(',',1)
    a_dic[k]=v
b_dic={}
for s in b:
    k,v = s.split(',',1)
    b_dic[k]=v
c_dic=a_dic
for k,v in b_dic.items():
    if k in c_dic:
        c_dic[k]=','.join([c_dic[k],v])
    else:
        c_dic[k]=v
c=[','.join([k,c_dic[k]]) for k in c_dic]
print(c)
```


##### 有一个多层嵌套的列表A=[1,2,3,[4,1,['j1',1,[1,2,3,'aa']]]],请写一段代码将A中的元素全部打印出来
```python
A=[1,2,3,[4,1,['j1',1,[1,2,3,'aa']]]]
def my_print(lis):
    for i in lis:
        if type(i)==list:
            my_print(i)
        else:
            print(i)
my_print(A)
```

##### a=range(10),则a[::-3]的值是？
* [9,6,3,0] 或者 range(9,-1,-3)


##### 将下面列表中的元素根据位数合并成字典：
```python

lst = [1,2,4,8,16,32,64,128,256,512,1024,32769,65536,4294967296]

# 结果
{1: [1, 2, 4, 8], 2: [16, 32, 64], 3: [128, 256, 512], 4: [1024], 5: [32769, 65536], 10: [4294967296]}
```
```python

lst = [1,2,4,8,16,32,64,128,256,512,1024,32769,65536,4294967296]
dic={}
for i in lst:
    len_i=len(str(i))
    dic.setdefault(len_i,[]).append(i)
print(dic)
```

##### 用尽量简洁的方法将二维数组合并成一维数组
```python
lst = [[1,2,3],[4,5,6],[7,8,9]]
ll=[]
for l in lst:
    # ll+=l
    ll.extend(l)
print(ll)
```
      
##### 将列表按照下列规则排序：
1. 正数在前，负数在后
2. 正数从小到大
3. 负数从大到小

* 例子：
    * 排序前：[7,-8,5,4,0,-2,-5]
    * 排序后：[0, 4, 5, 7, -2, -5, -8]
```python
lis = [7,-8,5,4,0,-2,-5]
lis=sorted(lis,key=lambda x:(x<0,abs(x))) # 这里排序条件返回元组，先比较第一个，再第二个值
print(lis)
```

##### 解决哈希冲突的算法有哪几种？分别有什么特点？
[哈希冲突参考](https://blog.csdn.net/seulzz/article/details/77163878)
1. 开放定址法
2. 再哈希法
3. 链地址法
4. 建立公共溢出区

##### 简述python字符串的驻留机制
[python字符串驻留机制参考文档](https://www.cnblogs.com/asmer-stone/p/4802800.html)

* 相同对象的引用都指向内存中的同一个位置，这个也叫python的字符串驻留机制
* python的引用计数机制，并不是对所有的数字，字符串，他只对”[0-9]\[a-z]\[A-Z]
和"\_"(下划线)  ”有效“，当字符串中由其他字符比如“！ @ # ￥ % -”时字符驻留机制是不起作用的。

##### 以下代码输出什么？

```python
lis=['a','b','c','d','e']
print(lis[10:])
```
* 答案：[]

##### python哪些类型的数据才能作为字典的key？
* 可哈希的类型


##### 有如下代码：
```python
import copy
a=[1,2,3,[4,5],6]
b=a
c=copy.copy(a)
d=copy.deepcopy(a)
b.append(10)
c[3].append(11)
d[3].append(12)
```
* 求a，b，c，d
* 答案：
> a：[1, 2, 3, [4, 5, 11], 6, 10]
> b：[1, 2, 3, [4, 5, 11], 6, 10]
> c：[1, 2, 3, [4, 5, 11], 6]
> d：[1, 2, 3, [4, 5, 12], 6]

##### 对字典d={'a':30,'g':17,'b':25,'c':18,'d':50,'e':36,'f':57,'h':25}按照value字段进行排序

```python
d={'a':30,'g':17,'b':25,'c':18,'d':50,'e':36,'f':57,'h':25}
dd=sorted(d.items(),key=lambda x:x[1])
print(dd)
```

##### 找出两个列表中相同的元素和不同的元素
```python
list1=[1,2,3,5,8,7,11,10]
list2=[5,15,25,10]
sim=[i for i in list1 if i in list2]
diff=[i for i in list1+list2 if i not in sim]
print(sim)
print(diff)
```

##### 二叉树是非线性结构，栈和队列以及线性表都是线性结构，对吗？
* 对的

##### 从0-99这100个数中随机取出10个，要求不能重复
```python
import random
lis=random.sample(range(0,100),10)
print(lis)
```

##### 有一个列表lis=['This','is','a','Man','B','!']，对它进行大小写无关的排序

```python
lis=['This','is','a','Man','B','!']
lis=sorted(lis,key=str.lower)
print(lis)
```

##### 描述以下字典的items()方法和iteritems()方法有啥不同？

* 字典的items方法作用：是可以将字典中的所有项，以列表方式返回。因为字典是无序的，所以用items方法返回字典的所有项，也是没有顺序的。
* 字典的iteritems方法作用：与items方法相比作用大致相同，只是它的返回值不是列表，而是一个迭代器


##### 请列举你所知道的python代码检测工具以及他们之间的区别

* pylint --- 源代码分析器，可以分析python代码中的错误
* pyflakes --- 检查源文件错误的简单程序，不会检查代码风格。
* pep8 --- 检查代码规范的工具


##### 介绍一下try except的用法和作用？
* 主要用来处理异常
* 完整用法如下：
```python
try:
     Normal execution block
except A:
     Exception A handle
except B:
     Exception B handle
except:
     Other exception handle
else:
     if no exception,get here
finally:
     print("finally")   
```


##### 阅读以下代码，写输出结果
```python
lis = [2,4,5,6,7]
for i in lis:
    if i % 2==0:
        lis.remove(i)
print(lis)
```
* 结果：[4, 5, 7]

##### 对列表[3,1,-4,-2]按照绝对值排序
```python
lis=[3,1,-4,-2]
lis=sorted(lis,key=lambda x:abs(x))
print(lis)
```

##### 获取python解释器版本的方法
* 终端执行python -V

##### 现有mydict和变量onekey，请写出从mydict中取出onekey的值的方法

> 方法一：mydict[onekey]
> 这种方法，如果mydict中键不存在的时候程序会报错
> 方法二：mydict.get(onekey)
> 这种方法，如果存在，返回值，不存在返回None
> 方法三：mydict.setdefault(onekey,[])
> 这种方法：存在的话返回值，不存在的时候创建一个值，值得内容为第二个参数+
  
  ##### 列表中保留顺序和不保留顺序去重
  [参考文章](https://blog.csdn.net/Jerry_1126/article/details/84677212)
  
  * 不保留顺序
```python
lis=[3, 1, 4, 2, 3]
print(list(set(lis)))
```
  * 保留顺序
```python
lis=[3, 1, 4, 2, 3]
T=[]
[T.append(i) for i in lis if i not in T])
print(T)

# 或者
T=sorted(set(lis), key=lis.index)
print(T)
```

##### 在什么情况下y!=x-(x-y)会成立？
* x，y是两个不相等的非空集合

##### 实现99乘法表（使用两种方法）
```python
print('\n'.join(['\t'.join(['{}*{}={}'.format(x,y,x*y) for x in range(1,y+1)]) for y in range(1,10)]))
```
```python
for i in range(1,10):
    for j in range(1,i+1):
        print('%s*%s=%s'%(i,j,i*j),end='\t')
    else:
        print()
```

##### 判断dict中有没有某个key。
* key in dict.keys()  判断


##### a = dict(zip(('a','b','c','d','e'),(1,2,3,4,5))) 请问a是什么？
* {'a': 1, 'b': 2, 'c': 3, 'd': 4, 'e': 5}


##### 在python中如何拷贝一个对象，并说明他们之间的区别

1. 赋值（=），就是创建了对象的一个新的引用，修改其中任意一个变量都会影响到另一个。
2. 浅拷贝：创建一个新的对象，但它包含的是对原始对象中包含项的引用（copy模块的copy()函数）
3. 深拷贝：创建一个新的对象，并且递归的复制它所包含的对象（修改其中一个，另外一个不会改变）（copy模块的deep.deepcopy()函数）

##### python中进制转换
>进制转换以十进制为媒介
>十六进制前面加上0x，八进制加上0o，二进制前面加上0b

||二进制|八进制|十进制|十六进制|
| --- | --- | --- | --- | --- |
| 二进制 | |bin(int(x, 8)）  | bin(int(x, 10))  | bin(int(x, 16)) |
| 八进制 | oct(int(x, 2)) |  | oct(int(x, 10)) |oct(int(x, 16))  |
|十进制  | int(x, 2) | int(x, 8) |  | int(x, 16) |
| 十六进制 | hex(int(x, 2))|hex(int(x, 8))|hex(int(x, 10)) |

##### 将列表alist=[{'name':'a','age':25},{'name':'b','age':30},{'name':'c','age':20}]，按照age的值从大到小排列。

```python
alist=[{'name':'a','age':25},{'name':'b','age':30},{'name':'c','age':20}]
blist=sorted(alist,key=lambda x:x['age'],reverse=True)
print(blist)
```

##### 关于Python程序的运行方面，有什么手段能提升性能？

1. 使用多进程，充分利用机器的多核性能
2. 对于性能影响较大的部分代码，可以使用C或C++编写
3. 对于IO阻塞造成的性能影响，可以使用IO多路复用来解决
4. 尽量使用Python的内建函数5、尽量使用局部变量
 

##### python是如何进行内存管理的？python的程序会内存泄漏吗？说说有没有什么方面阻止或者检测内存泄漏？
[整体参考文章](https://www.jianshu.com/p/2b683cb5837c)
* python是如何进行内存管理的[参考文章](https://blog.csdn.net/u010967872/article/details/80301633)
    1. 引用计数
        * Python内部使用引用计数，来保持追踪内存中的对象，Python内部记录了对象有多少个引用，就是引用计数，当对象被创建时就创建了一个引用计数，当对象不再需要的时候，这个对象的引用计数为0时，他被垃圾回收。
    2. 垃圾回收
        * 当内存中有不再使用的部分时，垃圾收集器就会把他们清理掉。他会去检查那些引用计数为0的对象，然后清除其在内存中的空间。当然除了引用计数为0的会被清除，还有一种情况也会被垃圾收集器清掉，当两个对象相互引用时，他们本身其他引用已经为0了。
    3. 内存池机制
        * Python提供了对内存的垃圾收集机制，但是他将不用的内存放到内存池而不是反回给操作系统。
* python的程序会内存泄漏吗？
    * 会发生内存泄漏，在Python程序里，内存泄漏是由于一个长期持有的对象不断的往一个dict或者list对象里添加新的对象, 而又没有即时释放，就会导致这些对象占用的内存越来越多，从而造成内存泄漏。另外，对象的交叉引用也会造成内存无法释放的问题。
* 说说有没有什么方面阻止或者检测内存泄漏？
    1. 程序员管理好每个python对象的引用，尽量在不需要使用对象的时候，断开所有引用
    2. 尽量少通过循环引用组织数据，可以改用weakref做弱引用或者用id之类的句柄访问对象
    3. 通过gc模块的接口可以检查出每次垃圾回收有哪些对象不能自动处理，再逐个逐个处理
    
##### 一个大小为100G的文件etl_log.txt，要读取文件的内容，写出具体过程代码
```python
with open("etl_log.txt",'r',encoding='utf8') as f:
    for line in f:
        print(line,end='')
```

##### python代码如何获取命令行参数
[获取命令行参数的方法参考](https://www.cnblogs.com/ouyangpeng/p/8537616.html)
1.使用sys模块
    * 通过sys.argv来获取
2. 使用getopt模块

##### 写代码：如何由tuple1=('a','b','c','d','e')，和tuple2=(1,2,3,4,5)得到res={'a': 1, 'b': 2, 'c': 3, 'd': 4, 'e': 5}

```python
tuple1=('a','b','c','d','e')
tuple2=(1,2,3,4,5)
res=dict(zip(tuple1,tuple2))
print(res)
```

##### 1<(2==2)和1<2==2的结果分别是什么？
* 第一个为False，第二个为True，暂时按照第一个类型进行相应的转换

##### 如何打乱一个排好序的列表
* 使用random.shuffle()
```python
import random
alist=[1,2,3,4,5,6]
random.shuffle(alist)
print(alist)
```

##### 如何查找一个字符串中特定的字符？find和index的差异？
* 使用find和index方法查找

1. find()方法：查找子字符串，若找到返回从0开始的下标值，若找不到返回-1
2.  index()方法：python 的index方法是在字符串里查找子串第一次出现的位置，类似字符串的find方法，不过比find方法更好的是，如果查找不到子串，会抛出异常，而不是返回-1

##### 把a='aaabbcccdddde'这种形式的字符串，压缩成a3b2c3d4e1这种形式。
```python
a='aaabbcccdddde'
aa=''
for i in sorted(list(set(a)),key=a.index):
    aa=aa+i+str(a.count(i))
print(aa)
```

##### 一个数如果恰好等于它的因子之和，这个数就称为‘完数’，比如6=1+2+3，编程找出1000以内的所有的完数。
```python
wanshu=[]
for i in range(1,1001):
    s=0
    for j in range(1,i//2+1):
        if i % j ==0:
            s+=j
    else:
        if i==s:
            wanshu.append(i)
print(wanshu)
```

##### 输入一个字符串，输出该字符串的字符的所有组合。如输入'abc',输出a,b,c,ab,ac,bc,abc.

```python
def getC(s):
    if not s:
        return
    len_s=len(s)
    ss=[]
    for i in range(len_s):
        combination(s,0,i,ss)
aaa=[]
def combination(s,index,num,ss):
    global aaa
    if num==-1:
        return
    if index==len(s):
        return
    ss.append(s[index])
    aaa.append(''.join(ss))
    combination(s,index+1,num-1,ss)
    ss.pop()
    combination(s,index+1,num,ss)
    
getC('123')
print(aaa)
print(sorted(set(aaa),key=lambda x:len(str(x))))
```


##### 给定一个非空的字符串，判断它是否可以由它的一个子串重复多次构成。给定的字符串只含有小写英文字母，并且长度不超过10000。例如：'ababab',返回True，'ababa'，返回False
```python
def solution(s):
    ll=len(s)
    for i in range(1,ll//2+1):
        if ll % i == 0:
            j=0
            while s[:i]==s[j:j+i] and j<ll:
                j=j+i
            if j==ll:
                return True
    return False
    
print(solution('abababa'))
```

##### python递归的最大层数？
* 1000

##### filter、map、reduce的作用。
1. filter() 相当于过滤器的作用
 ```python
s=[1,2,3,5,6,8,9,10,25,12,30]
# 筛选出3的倍数
# 第一个参数为一个返回True或者False的函数，第二个参数为可迭代对象
# 该函数把可迭代对象依次传入第一个函数，如果为True，则筛选
d=filter(lambda x:True if x % 3 == 0 else False,s)
print(list(d))
```
2. map()函数，
```python
# 第一个参数为函数，依次将后面的参数传给第一个函数，并执行函数
# 如果有多个参数则，依次将后面的对应传给参数
s=map(lambda x,y:x+y,range(10),range(10))
print(list(s))
ss=map(lambda x:x*x,range(10))
print(list(ss))
```
3. reduce()函数
```python
from functools import reduce
# 开始的时候将可迭代对象的第一个数和第二个数当成x和y
# 然后将第一次函数的执行结果当成x，然后再传入一个数当成y
# 再执行函数
s=reduce(lambda x,y:x+y,range(101))
print(s) # 相当于0+1+2+……+99+100
```

##### 什么是闭包
* 在函数中可以（嵌套）定义另一个函数时，如果内部的函数引用了外部的函数的变量，则可能产生闭包。闭包可以用来在一个函数与一组“私有”变量之间创建关联关系。在给定函数被多次调用的过程中，这些私有变量能够保持其持久性。
```python
# 内部函数使用了外部函数的变量，就相当于闭包
def func1():
    a=1
    def inner():
        return a
    return inner
print(func1()())
```

##### 简述生成器，迭代器，装饰器以及应用场景
[参考链接](https://blog.csdn.net/weixin_39387409/article/details/85089652)

1. 迭代器对象实现了iter()方法
2. 迭代器实现了iter()和next()方法，迭代器对象从集合的第一个元素开始访问，直到所有的元素被访问完结束
3. 生成器是迭代器的一种，一个函数调用时返回一个迭代器，这个函数就叫生成器。通常带有yield
4. 装饰器是一个以函数作为参数，并返回一个替换函数的可执行函数，是闭包的一种应用。通常用来给一个函数添加功能


##### 使用生成器编写一个函数实现生成指定个数的斐波那契数列
```python
def fib2(imax):
    t,a,b=0,0,1
    while t<imax:
        yield b
        a,b=b,a+b
        t+=1
        
for i in fib2(10):
    print(i)
```

##### 一行代码通过filter和lambda函数输出alist=[1,22,2,33,23,32]中索引为奇数的值
```python
alist=[1,22,2,33,23,32]
ss=[x[1] for x in filter(lambda x:x[0]%2==1,enumerate(alist))]
print(ss)
```

##### 编写一个函数实现十进制转62进制，分别用0-9A-Za-z,表示62位字母
```python
import string
print(string.ascii_lowercase) # 小写字母
print(string.ascii_uppercase) # 大写字母
print(string.digits) # 0-9

s=string.digits+string.ascii_uppercase+string.ascii_lowercase
def _10_to_62(num):
    ss=''
    while True:
        ss=s[num%62]+ss
        if num//62==0:
            break
        num=num//62
    return ss
print(_10_to_62(65))
```

##### 实现一个装饰器，限制该函数被调用的频率，如10秒一次

```python
import time
from functools import wraps
def dec(func):
    key=func.__name__
    cache={key:None}
    @wraps(func)
    def inner(*args,**kwargs):
        result=None
        if cache.get(key) is None:
            cache[key]=time.time()
            result=func(*args,**kwargs)
            print('执行函数中')
        else:
            now=time.time()
            if now-cache[key]>10:
                cache[key]=now
                result=func(*args,**kwargs)
                print('执行函数中')
            else:
                print('函数执行受限')
        return result
    return inner
    
@dec
def add(x,y):
    print(x+y)
    
add(1,2)
add(1,3)
time.sleep(10)
add(3,4)
```

##### 实现一个装饰器，通过一次调用，使函数重复执行5次
```python
from functools import wraps
def dec(func):
    @wraps(func)
    def inner(*args,**kwargs):
        result=[func(*args,**kwargs) for i in range(5)]
        return result
    return inner
    
@dec
def add(x,y):
    return x+y
print(add(1,2))
```

##### 生成器与函数的区别？
* 生成器和函数的主要区别在于函数 return a value，生成器 yield a value同时标记或记忆point of the yield 以便于在下次调用时从标记点恢复执行。 yield 使函数转换成生成器，而生成器反过来又返回迭代器。
```python
# 简单实现生成器
def dec():
    n=0
    for i in range(10):
        yield n
        n+=i
        
for i in dec():
    print(i)
```

##### 列表推导式[i for i in range(10)]和生成式表达式(i for i in range(10))的区别
[参考文章](https://blog.csdn.net/qq_36523839/article/details/79807866)

1. 列表推导式的结果是一个列表。
2. 生成器表达式的结果是一个生成器，它和列表推导式类似，它一次处理一个对象，而不是一口气处理和构造整个数据结构，可以节约内存。

##### python如何定义函数时如何书写可变参数和关键字参数？
```python
def func(a,*args,b=1,**kwargs):
    pass
```

##### python中enumerate的意思是什么？
* 枚举的意思，同时得到可迭代对象，如列表和元组的索引和值，以元组形式返回

##### 描述以下dict的items和iteritems的区别
* python3中没有iteritems
* items和iteritems大致相同，只是items返回的是一个列表，iteritems返回的是一个迭代器。

##### 是否使用过functools中的函数？他的作用是什么？
1. functools.wraps()
    * 在装饰器中用过，如果不使用wraps，则原始函数的__name__和__doc__的值就会丢失
 2. functools.reduce()
     * 第一个参数是一个函数，第二个参数是一个可迭代对象，代码如下：
```python
# 下面代码相当于从1加到9
from functools import reduce
a=reduce(lambda x,y:x+y,range(10))
print(a)
```

##### 如何判断一个值是方法还是函数？
[参考链接](https://blog.csdn.net/amoscn/article/details/77074403)
1. 使用type()来判断，如果是method为方法，如果是function则是函数。
2. 与类和实例无绑定关系的function都属于函数（function）
3. 与类和实例有绑定关系的function都属于方法


##### 请编写一个函数将ip地址转换成一个整数。如10.3.9.12转换成00001010 00000011 00001001 00001100，然后转换成整数
```python
def ip2int(ip):
    nums=ip.split('.')
    # zfill()函数是补0
    to_bin=[bin(int(i))[2:].zfill(8) for i in nums]
    return int(''.join(to_bin),2)
i=ip2int('127.0.0.1')
print(i)
```

##### lambda表达式格式以及应用场景？
* 格式：lambda 参数列表 : 返回表达式
* 应用场景：常见的在filter，reduce以及map中使用。

##### pass的使用
* 通常用来标记一个还未写的代码的位置，pass不做任何事情，一般用来做占位语句，保持程序结构的完整性

##### *arg和**kwargs的作用
* 用来接收不确定个数的参数，\*args通常用来接收不确定个数的非关键字参数，而\*\*kwargs通常用来接收不确定个数的关键字参数

##### 如何在函数中设置一个全局变量？
* 在函数中使用global关键字定义变量

##### 求以下代码结果：
```python
def num():
    return [lambda x:i*x for i in range(4)]
print([m(2) for m in num()])
```
* 答案：[6,6,6,6]

##### yield from 和 yield 的区别
[简述yield和yield from](https://blog.csdn.net/lamusique/article/details/85845225)

```python
# 下面a()和b()是等价的
def a():
    yield from [1,2,3,4,5]
def b():
    for i in [1,2,3,4,5]:
        yield i
for i in a():
    print(i)
for i in b():
    print(i)
```
* yield将一个函数变成一个生成器
* yield 返回一个值
* yield from后面接可迭代对象，一个一个返回值。

##### 求以下代码的输出结果
```python
collapse=True
processFunc=collapse and (lambda s:' '.join(s.split())) or (lambda s:s)
print(processFunc('i\tam\ntest\tproject!'))

collapse=False
processFunc=collapse and (lambda s:' '.join(s.split())) or (lambda s:s)
print(processFunc('i\tam\ntest\tproject!'))
```
* 答案：
>i am test project!
>i       am
>test    project!


##### 编写一个函数，找出数组中没有重复的值的和
```python
def func(lis):
    lis1=[]
    del_lis=[]
    for i in lis:
        if i not in lis1:
            if i not in del_lis:
                lis1.append(i)
        else:
            del_lis.append(i)
            lis1.remove(i)
    return sum(lis1)
    
def func2(lis):
    return sum([i for i in set(lis) if lis.count(i)==1])
    
print(func2([3,4,1,2,5,6,6,5,4,3,3]))
```

##### 下面代码的执行结果是
```python
a=1
def bar():
    a+=3
    
bar()
print(a)
```
* 答案：运行出错

##### 写一个函数，计算出以下字母所代表的数字，每个字母值不一样
```python
for A in range(1,10):
    for B in range(10):
        if A==B:
            continue
        for C in range(1,10):
            if C in [A,B]:
                continue
            for D in range(10):
                if D in [A,B,C]:
                    continue
                for E in range(1,10):
                    if E in [A,B,C,D]:
                        continue
                    for F in range(10):
                        if F in [A,B,C,D,E]:
                            continue
                        for G in range(1,10):
                            if G in [A,B,C,D,E,F]:
                                continue
                            for H in range(10):
                                if H in [A,B,C,D,E,F,G]:
                                    continue
                                for P in range(1,10):
                                    if P in [A,B,C,D,E,F,G,H]:
                                        continue
                                    if (A*10+B)-(C*10+D)==(E*10+F) and (E*10+F)+(G*10+H)==(P*100+P*10+P):
                                    print(A,B,C,D,E,F,G,H,P)
```

#### 写出如下代码的输出结果
[参考链接](https://www.cnblogs.com/z-x-y/p/9157238.html)

```python
def decorator_a(func):
    print('Get in decorator_a')
    def inner_a(*args, **kwargs):
        print('Get in inner_a')
        return func(*args, **kwargs)
    return inner_a
    
def decorator_b(func):
    print('Get in decorator_b')
    def inner_b(*args, **kwargs):
        print('Get in inner_b')
        return func(*args, **kwargs)
    return inner_b
    
@decorator_b #f=decorator_b(f)
@decorator_a #f=decorator_a(f)
def f(x):
    print('Get in f')
    return x * 2
f(1)
```
* 答案
>Get in decorator_a
>Get in decorator_b
>Get in inner_b
>Get in inner_a
>Get in f

* 解释
 >当我们对f传入参数1进行调用时，inner_b被调用了，他会先打印Get in inner_b,然后在inner_b内部调用了inner_a,所以会再打印Get in inner_a,然后再inner_a内部调用原来的f,并且将结果作为最终的返回总结：装饰器函数在被装饰函数定义好后立即执行从下往上执行函数调用时从上到下执行


##### 写出以下代码的输出结果：
```python
def test():
    try:
        raise ValueError('something wrong')
    except ValueError as e:
        print('error occured')
        return
    finally:
        print('ok')
test()
```
* 结果(finally无论怎样都会执行)
>error occured
>ok

##### 求出以下代码的输出结果
```python
mydict={'a':1,'b':2}
def func(d):
    d['a']=0
    return d
    
func(mydict)
mydict['c']=2
print(mydict)
```
* 结果
>{'a': 0, 'b': 2, 'c': 2}

##### 写个函数接收一个文件夹名称作为参数，显示文件夹中文件的路径，以及其中包含的文件夹中文件的如今
```python
# 方法一
import os
def Test1(rootDir):
    list_dirs = os.walk(rootDir)
    for root, dirs, files in list_dirs:
        for d in dirs:
            print(os.path.join(root, d))
        for f in files:
            print(os.path.join(root, f))
Test1(r'C:\Users\felix\Desktop\aaa')
print('###################')
# 方法二
import os
def Test2(rootDir):
    paths=os.listdir(rootDir)
    for lis in paths:
        path=os.path.join(rootDir,lis)
        print(path)
        if os.path.isdir(path):
             Test2(path)
Test2(r'C:\Users\felix\Desktop\aaa')
```

##### re的match和search的区别
* match（）函数是在string的开始位置匹配，如果不匹配，则返回None
* search()会扫描整个string查找匹配；也就是说match（）只有在0位置匹配成功的话才有返回，

##### 什么是正则的贪婪匹配？贪婪模式和非贪婪模式的区别？
[参考文档](https://www.cnblogs.com/ILoke-Yang/p/8060003.html)

* 贪婪匹配:正则表达式一般趋向于最大长度匹配，也就是所谓的贪婪匹配。
* 非贪婪匹配：就是匹配到结果就好，就少的匹配字符。
* 区别：默认是贪婪模式；在量词后面直接加上一个问号？就是非贪婪模式。

##### 如何使用python删除一个文件或者文件夹？
```python
import os
import shutil
os.remove(path) # 删除文件
os.removedirs(path) # 删除空文件夹
shutil.rmtree(path) # 删除文件夹，可以为空也可以不为空
```

##### logging模块的作用以及应用场景
* logging模块定义的函数和类为应用程序和库的开发实现了一个灵活的事件日志系统。
* 记录日志

##### json序列化时可以处理的数据类型有哪些？如何定制支持datetime类型？序列化时，遇到中文转成unicode，如何保持中文形式？
1. 可以处理的数据类型是 string、int、list、tuple、dict、bool、null
2. 通过自定义时间序列化转换器
```python
import json
from json import JSONEncoder
from datetime import datetime
class ComplexEncoder(JSONEncoder):
    def default(self, obj):
        if isinstance(obj, datetime):
            return obj.strftime(‘%Y-%m-%d %H:%M:%S‘)
        else:
            return super(ComplexEncoder,self).default(obj)
d = { ‘name‘:‘alex‘,‘data‘:datetime.now()}
print(json.dumps(d,cls=ComplexEncoder))
# {"name": "alex", "data": "2018-05-18 19:52:05"}
```
3. 使用ensure_ascii=False参数

##### 写出邮箱的正则表达式

```python
import re
pp=re.compile('[a-zA-Z0-9_-]+@[0-9A-Za-z]+(\.[0-9a-zA-Z]+)+')
if pp.match('1403179190@qq.com'):
    print('ok')
```

##### 写python爬虫分别用到了哪些模块？分别有什么用？
* 模块
    * request，发起请求
    * pyquery，解析html数据
    * beautifulsoup，解析html数据
    * aiohttp，异步发送请求
* 框架
    * pyspider，web界面的爬虫框架
    * scrapy，爬虫框架
    * selenium，模拟浏览器的爬虫框架

##### sys.path.append('xxx')的作用
* 添加搜索路径

##### 输入某年某月某日，判断这是这一年的第几天？
```python
date=input('请输入某年某月某日，格式：xxxx.xx.xx')
def get_day(date):
    days1=[31,28,31,30,31,30,31,31,30,31,30,31]
    days2=[31,29,31,30,31,30,31,31,30,31,30,31]
    year,month,day = [int(i) for i in date.split('.')]
    if year % 400 ==0 or (year % 4==0 and year % 100!=0):
         days=days2
    else:
        days=days1
    return sum(days[:month-1])+day
print(get_day(date))
```

##### 简述面向对象的三大特性？
[参考链接](https://www.cnblogs.com/lfpython/p/7346385.html)
* 继承，封装和多态
    * 继承：
        * 继承就是继承的类直接拥有被继承类的属性而不需要在自己的类体中重新再写一遍，其中被继承的类叫做父类、基类，继承的类叫做派生类、子类。
    * 封装：
        * 封装就是把类中的属性和方法定义为私有的，方法就是在属性名或方法名前加双下划线，而一旦这样定义了属性或方法名后，python会自动将其转换为_类名__属性名（方法名）的格式，在类的内部调用还是用双下划线加属性名或方法名，在类的外部调用就要用_类名__属性名（方法名）。父类的私有属性和方法，子类无法对其进行修改。
    * 多态：
        * 多态就是不同的对象可以调用相同的方法然后得到不同的结果，有点类似接口类的感觉，在python中处处体现着多态，比如不管你是列表还是字符串还是数字都可以使用+和*。

##### 什么是鸭子模型？
* 鸭子类型（英语：duck typing）是动态类型的一种风格。在这种风格中，一个对象有效的语义，不是由继承自特定的类或实现特定的接口，而是由当前方法和属性的集合决定。

##### super的作用
* 当子类中的方法与父类中的方法重名时，子类中的方法会覆盖父类中的方法，那么，如果我们想实现同时调用父类和子类中的同名方法，就需要使用到super()这个函数，用法为super().函数名()

##### mro是什么？
* 对于支持继承的编程语言来说，其方法（属性）可能定义在当前类，也可能来自于基类，所以在方法调用时就需要对当前类和基类进行搜索以确定方法所在的位置。而搜索的顺序就是所谓的「方法解析顺序」（Method Resolution Order，或MRO）。

##### 什么是c3算法？
* c3算法是python新式类中用来产生mro顺序的一套算法。即多继承的查找规则。

##### 列举面向对象中带双下划线的特殊方法

>\_\_new__：可以调用其它类的构造方法或者直接返回别的对象来作为本类的实例。
>\_\_init__： 负责类的实例化
>\_\_call__：对象后边加括号，触发执行
>\_\_str__：print打印一个对象时。
>\_\_doc__：类的注释，该属性是无法继承的。
>\_\_getattr__：在使用调用属性（方式、属性）不存在的时候触发
>\_\_setattr__：添加/修改属性会触发它的执行
>\_\_dellattr__：删除属性的时候会触发
>\_\_delete__：采用del删除属性时，触发

##### 双下划线和单下划线的区别

* "单下划线" 开始的成员变量叫做保护变量，意思是只有类对象和子类对象自己能访问到这些变量；
* "双下划线" 开始的是私有成员，意思是只有类对象自己能访问，连子类对象也不能访问到这个数据。

##### 实例变量和类变量的区别

* 实例变量是对于每个实例都独有的数据
* 类变量是该类所有实例共享的属性和方法

##### 实例方法、静态方法和类方法的区别
* 实例方法：第一个参数必须是实例对象，通常为self。实例方法只能由实例对象调用。
* 类方法：使用装饰器@classmethod。第一个参数为当前类的对象，通常为cls。实例对象和类对象都可以调用类方法。
* 静态方法：使用装饰器@staticmethod。没有self和cls参数。方法体中不能使用类或者实例的任何属性和方法。实例对象和类对象都可以调用。

##### isinstance和type的作用
* 两者都用来判断对象的类型
* 对于一个类的之类对象的类型判断，type就不行了，而isinstance可以。
```pyyhon
class A(object):
    pass
class B(A):
    pass
    
ba=B()
ab=A()
print(type(ba)==A) # False
print(type(ab)==A) # True
print(isinstance(ab,A)) # True
print(isinstance(ba,A)) # True
```

##### 使用with语句的好处是什么
*  使用with后不管with中的代码出现什么错误，都会进行对当前对象进行清理工作。例如file的file.close()方法，无论with中出现任何错误，都会执行file.close（）方法
*  只有支持上下文管理器的对象才能使用with，即在对象内实现了两个方法：__enter__()和__exit__()

##### 写一个的支持with语句的类
[参考链接](https://www.cnblogs.com/yidashi110/p/10091991.html)
```python
class W(object):
    def __init__(self):
        pass
    def __enter__(self):
        print('进入with语句')
        return self
        
    def __exit__(self,*args,**kwargs):
        print('退出with语句')
        
with W() as w:
    print('之前')
    print(w)
    print('之后')
```


##### 实现一个单例模式。(尽可能多的方法)
[参考链接](https://www.cnblogs.com/huchong/p/8244279.html)
```python
# 方法一：使用__new__()
import threading
class Singleton(object):
    _instance_lock = threading.Lock()
    def __init__(self):
        pass
        
    def __new__(cls, *args, **kwargs):
        if not hasattr(Singleton, "_instance"):
            with Singleton._instance_lock:
                if not hasattr(Singleton, "_instance"):
                    Singleton._instance = object.__new__(cls)
        return Singleton._instance
        
obj1 = Singleton()
obj2 = Singleton()
print(obj1 is obj2)

# 方法二：使用元类来创建
import threading

class SingletonType(type):
    _instance_lock = threading.Lock()
    def __call__(cls, *args, **kwargs):
        if not hasattr(cls, "_instance"):
            with SingletonType._instance_lock:
                if not hasattr(cls, "_instance"):
                    cls._instance = super().__call__(*args, **kwargs)
        return cls._instance
        
class Singleton(metaclass=SingletonType):
    def __init__(self):
        pass
 
obj1 = Singleton()
obj2 = Singleton()
print(obj1 is obj2)
```

##### 如何判断一个对象是否可调用？哪些对象是可调用对象？如何定义一个类，使其对象本身就是可调用对象？
* 使用callable函数判断。
* 可调用对象有7类：
    * 用户自定义函数
    * 内置函数
    * 内置方法
    * 方法(定义在类中的函数)
    * 类
    * 类实例(如果类中定义了__call__方法，那么这个类的实例就是可调用对象)
    * 生成器函数 
* 在类中定义__call__方法，实例对象加()是即调用__call__的方法

##### 手写一个栈

```python
#给一个点，我们能够根据这个点知道一些内容
class Node(object):
    def __init__(self,val): #定位的点的值和一个指向
        self.val=val #指向元素的值,原队列第二元素
        self.next=None #指向的指针
        
class stack(object):
    def __init__(self):
        self.top=None #初始化最开始的位置
        
    def push(self,n):#添加到栈中
        n=Node(n) #实例化节点
        n.next=self.top #顶端元素传值给一个指针
        self.top=n
        return n.val
        
    def pop(self): #退出栈
        if self.top == None:
            return None
        else:
            tmp=self.top.val
            self.top=self.top.next #下移一位，进行
            return tmp
            
if __name__=="__main__":
    s=stack()
    print(s.pop())
    s.push(1)
    print(s.pop())
    s.push(2)
    s.push(3)
    print(s.pop())
    s.push(3)
    s.push(3)
    s.push(3)
    print(s.pop())
    print(s.pop())
    print(s.pop())
    print(s.pop())
```

##### 使用两个队列实现一个栈
```python
class Stack(object):
    def __init__(self):
        self.queueA=[]
        self.queueB=[]
    def push(self,node):
        self.queueA.append(node)
    def pop(self):
        if len(self.queueA)==0:
            return None
        while len(self.queueA)!=1:
            self.queueB.append(self.queueA.pop(0))
        self.queueA,self.queueB=self.queueB,self.queueA
        return self.queueB.pop()
        
st=Stack()
print(st.pop())
st.push(1)
print(st.pop())
st.push(1)
st.push(1)
st.push(1)
print(st.pop())
print(st.pop())
print(st.pop())
```
* 注意上面两个栈的实现方法，第一种的效率高，队列的这种方法效率低

##### 有如下链表类，请实现单链表逆置。
```python
class ListNode:
    def __init__(self,val):
        self.val=val
        self.next=None
        
class Solution:
    def reverseList(self,pHead):
        if not pHead or not pHead.next:
            return pHead
        last=None
        while pHead:
            tmp=pHead.next
            pHead.next=last
            last=pHead
            pHead=tmp
        return last
```

##### 类的加载和实例化过程

1. 在堆内存中生成class对象, 把静态变量和静态方法加载到方法区, 这个堆内存中的class对象是方法区数据的入口
2. 静态变量默认初始化
3. 静态变量显式初始化
4. 执行静态代码块
5. 成员变量默认初始化, 显示初始化
6. 执行构造函数

##### 手写一个队列
```python
class Queue(object):
    def __init__(self,size):
        self.queue=[]
        self.size=size
    def is_empty(self):
        return not bool(len(self.queue))
    def is_full(self):
        return len(self.queue)==self.size
    def enqueue(self,val):
        if not self.is_full():
            self.queue.insert(0,val)
            return True
        return False
    def dequeue(self):
        if not self.is_empty():
            return self.queue.pop()
        return None
s=Queue(2)
print(s.is_empty)
s.enqueue(1)
s.enqueue(2)
print(s.is_full())
print(s.dequeue())
print(s.dequeue())
print(s.is_empty())
```

##### python的底层网络交互模块有哪些
* socket，urllib，requests，pycurl

##### 简述OSI七层协议
[参考链接](https://zhidao.baidu.com/question/568531489.html)
* 为了实现计算机系统的互连，OSI参考模型把整个网络的通信功能划分为7个层次，同时也定义了层次之间的相互关系以及各层所包括的服务及每层的功能。OSI的七层由低到高依次为：物理层、数据链路层、网络层、传输层、会话层、表示层、应用层，下三层（物理层、数据链路层、网络层）面向数据通信，而上三层（会话层、表示层、应用层）则面向资源子网，而传输层则是七层中最为重要的一层。它位于上层和下层中间，起承上启下的作用。

##### 什么是C/S和B/S架构
[参考链接](https://www.cnblogs.com/1130136248wlxk/p/5192043.html)
* C/S 架构是一种典型的两层架构，其全称是Client/Server，即客户端服务器端架构，其客户端包含一个或多个在用户的电脑上运行的程序，而服务器端有两种，一种是数据库服务器端，客户端通过数据库连接访问服务器端的数据；另一种是Socket服务器端，服务器端的程序通过Socket与客户端的程序通信。
* B/S架构的全称为Browser/Server，即浏览器/服务器结构。Browser指的是Web浏览器，极少数事务逻辑在前端实现，但主要事务逻辑在服务器端实现，Browser客户端，WebApp服务器端和DB端构成所谓的三层架构。B/S架构的系统无须特别安装，只有Web浏览器即可。

##### 简述TCP三次握手，四次挥手的流程。
[参考链接](https://blog.csdn.net/qq_38950316/article/details/81087809)

* 三次握手
    * 第一次握手：客户端的应用进程主动打开，并向客户端发出请求报文段。其首部中：SYN=1,seq=x。
    * 第二次握手：服务器应用进程被动打开。若同意客户端的请求，则发回确认报文，其首部中：SYN=1,ACK=1,ack=x+1,seq=y。
    * 第三次握手：客户端收到确认报文之后，通知上层应用进程连接已建立，并向服务器发出确认报文，其首部：ACK=1,ack=y+1。当服务器收到客户端的确认报文之后，也通知其上层应用进程连接已建立。
* 四次挥手
    * 第一次挥手：数据传输结束以后，客户端的应用进程发出连接释放报文段，并停止发送数据，其首部：FIN=1,seq=u。
    * 服务器端收到连接释放报文段之后，发出确认报文，其首部：ack=u+1,seq=v。此时本次连接就进入了半关闭状态，客户端不再向服务器发送数据。而服务器端仍会继续发送。
    * 第三次挥手：若服务器已经没有要向客户端发送的数据，其应用进程就通知服务器释放TCP连接。这个阶段服务器所发出的最后一个报文的首部应为：FIN=1,ACK=1,seq=w,ack=u+1。
    *  第四次挥手：客户端收到连接释放报文段之后，必须发出确认：ACK=1,seq=u+1,ack=w+1。 再经过2MSL(最长报文端寿命)后，本次TCP连接真正结束，通信双方完成了他们的告别。

##### 如果已经建立了TCP连接，但是客户端突然出现故障了怎么办

* TCP还设有一个保活计时器，显然，客户端如果出现故障，服务器不能一直等下去，白白浪费资源。服务器每收到一次客户端的请求后都会重新复位这个计时器，时间通常是设置为2小时，若两小时还没有收到客户端的任何数据，服务器就会发送一个探测报文段，以后每隔75秒发送一次。若一连发送10个探测报文仍然没反应，服务器就认为客户端出了故障，接着就关闭连接。


##### 什么是arp协议

* ARP全称“Address Resolution Protocol”，地址解析协议。
* 实现局域网内通过IP地址获取主机的MAC地址。
* MAC地址48位主机的物理地址，局域网内唯一。
* ARP协议类似DNS服务，但不需要配置服务。
* ARP协议是三层协议。

##### TCP和UDP的区别
1. TCP面向连接（如打电话要先拨号建立连接）;UDP是无连接的，即发送数据之前不需要建立连接
2. TCP提供可靠的服务。也就是说，通过TCP连接传送的数据，无差错，不丢失，不重复，且按序到达;UDP尽最大努力交付，即不保证可靠交付
3. UDP具有较好的实时性，工作效率比TCP高，适用于对高速传输和实时性有较高的通信或广播通信。
4. 每一条TCP连接只能是点到点的;UDP支持一对一，一对多，多对一和多对多的交互通信
5. TCP对系统资源要求较多，UDP对系统资源要求较少。

##### 为什么基于tcp协议的通信比基于udp协议的通信更可靠

* TCP是面向连接的传输协议，每次都需要建立一个可以相互信任的连接，中间有个三次握手过程。而UDP是面向无连接的传输协议，不需要建立安全的连接，


##### 什么是局域网和广域网
* 局域网（Local Area Network），简称LAN，是指在某一区域内由多台计算机互联成的计算机组。“某一区域”指的是同一办公室、同一建筑物、同一公司和同一学校等，一般是方圆几千米以内。局域网可以实现文件管理、应用软件共享、打印机共享、扫描仪共享、工作组内的日程安排、电子邮件和传真通信服务等功能。局域网是封闭型的，可以由办公室内的两台计算机组成，也可以由一个公司内的上千台计算机组成。
* 广域网（Wide Area Network），简称WAN，是一种跨越大的、地域性的计算机网络的集合。通常跨越省、市，甚至一个国家。广域网包括大大小小不同的子网，子网可以是局域网，也可以是小型的广域网。
* 两者区别：
    * 范围不同，广域网比局域网广
    * 接口类型不同
    * 速率不同
    * 协议不同

##### 什么是socket？简述基于tcp协议的socket通信流程？
* socket通常也称作"套接字"，用于描述IP地址和端口，是一个通信链的句柄。
* 通信流程：
    1. 服务端创建一个ServerSocket对象,指定端口号,ServerSocket对象等待客户端的连接请求。
    2. 客户端创建一个Socket对象,指定主机地址和端口号,向服务端发出连接请求。
    3. 服务端接收到客户端的连接请求,建立一条TCP连接,再创建一个Socket对象与客户端的Socket对象进行通信。
    4. 服务端和客户端分别创建字节输入流和字节输出流,通过字节输入流获得对方发来的数据,通过字节输出流向对方发送数据。
    5. 当一方决定结束通信时,向对方发送结束信息;另一方接收到结束信息后,双方分别关闭各自的TCP连接。
    6. ServerSocket对象停止等待客户端的连接请求。

##### 什么是粘包？出现粘包的原因？
* 粘包：多个数据包被连续存储于连续的缓存中，在对数据包进行读取时由于无法确定发生方的发送边界，而采用某一估测值大小来进行数据读出，若双方的size不一致时就会使指发送方发送的若干包数据到接收方接收时粘成一包，从接收缓冲区看，后一包数据的头紧接着前一包数据的尾。
* 出现粘包现象的原因是多方面的，它既可能由发送方造成，也可能由接收方造成。
    * 发送方引起的粘包是由TCP协议本身造成的，TCP为提高传输效率，发送方往往要收集到足够多的数据后才发送一包数据。若连续几次发送的数据都很少，通常TCP会根据优化算法把这些数据合成一包后一次发送出去，这样接收方就收到了粘包数据。
    * 接收方引起的粘包是由于接收方用户进程不及时接收数据，从而导致粘包现象。这是因为接收方先把收到的数据放在系统接收缓冲区，用户进程从该缓冲区取数据，若下一包数据到达时前一包数据尚未被用户进程取走，则下一包数据放到系统接收缓冲区时就接到前一包数据之后，而用户进程根据预先设定的缓冲区大小从系统接收缓冲区取数据，这样就一次取到了多包数据。

##### 发生粘包现象如何处理？

1. 对于发送方引起的粘包现象，用户可通过编程设置来避免，TCP提供了强制数据立即传送的操作指令push，TCP软件收到该操作指令后，就立即将本段数据发送出去，而不必等待发送缓冲区满；
2. 对于接收方引起的粘包，则可通过优化程序设计、精简接收进程工作量、提高接收进程优先级等措施，使其及时接收数据，从而尽量避免出现粘包现象；
3. 由接收方控制，将一包数据按结构字段，人为控制分多次接收，然后合并，通过这种手段来避免粘包。

##### IO多路复用的作用？
* I/O多路复用是用于提升效率，单个进程可以同时监听多个网络连接IO。
* 与多进程和多线程技术相比，I/O多路复用技术的最大优势是系统开销小，系统不必创建进程/线程，也不必维护这些进程/线程，从而大大减小了系统的开销。

##### 什么是防火墙？防火墙的作用是什么？
* 在互联网上防火墙是一种非常有效的网络安全模型，通过它可以隔离风险区域(即Internet或有一定风险的网络)与安全区域(局域网)的连接，同时不会妨碍人们对风险区域的访问。所以它一般连接在核心交换机与外网之间。
* 防火墙的作用：
    1. 过滤进出网络的数据 
    2. 管理进出访问网络的行为 
    3. 封堵某些禁止业务 
    4. 记录通过防火墙信息内容和活动 
    5. 对网络攻击检测和告警

##### select、poll、epoll模型的区别
[参考链接](https://www.cnblogs.com/jeakeven/p/5435916.html)

1. 支持一个进程所能打开的最大连接数
    * select的最大连接数大概32*32，或者32*64
    * poll本质和select没区别，但是它没有最大连接数限制
    * epoll大概10万左右(1G的机器)
2. FD剧增后带来的IO效率问题
    * select和poll每次调用都会对连接进行线性遍历，所以会随着FD的增加会造成遍历速度慢的“线性下降性能问题”
    * epoll没有前两个的线性下降的性能问题，但是当socket都很活跃的情况下，可能会有性能问题。
3. 消息传递方式
    * select和poll内核需要将消息传递到用户空间，都需要内核拷贝动作。
    * epoll通过内核和用户空间共享一块内存来实现

##### 简述进程，线程，协程的区别以及应用场景？
* 区别：
    1. 线程是资源分配的单位
    2. 线程是操作系统调度的单位
    3. 进程切换需要的资源很大，效率很低
    4. 线程切换需要的资源一般，效率一般(在不考虑GIL的情况下
    5. 协程切换任务资源很小，效率高
    6. 多进程，多线程根据cpu核数不一样可能是并行的，但是协程是在一个线程中，所以是并发。)
* 应用场景
    1. 协程：当程序中存在大量不需要cpu的操作时，适用协程
    2. 计算密集型，用进程。IO密集型，用线程。
