# python-interview

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
        * 公用一个值
        * 这两个变量的内存地址一样
        * 对其中一个变量的值改变，另外一个变量的值也会改变
* 深拷贝是一个变量对另外一个变量的值拷贝
    * 深拷贝的特点：
        * 两个变量的内存地址不同
        * 两个变量各有自己的值，且互不影响
        * 对其任意一个变量的值的改变不会影响另外一个


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
