
[<< Day 29](../29_Day_Building_API/29_building_API.md)

# Day 30

## 结尾

在翻译、校对和补充这个Python系列的过程中，我学到了很多，同时也有不少读者和学习挑战群学习者的积极反馈，让我觉得做这件事有了更多意义。

如果你是一步步走到这里，那么同样也恭喜你。如果你已经完成了所有的练习和项目，现在你有能力进入数据分析、数据科学、机器学习或web开发的道路。此系列属于初中级的水准。
- 如果你想在某一方更深的发展，比如成为开发，那么还需要进行高阶的学习才行；
- 如果是作为一个测试开发，那么还要保持一定广度的学习。比如Python应用的自动化，测试平台开发等。

> 关于测试平台，测试自动化，性能测试等内容笔者在Github、博客、公众号都有不同的系列实战教程，欢迎继续来围观。

回归主题，接下来让我们对之前所学的内容进行一次快速地回顾和总结，看看都学到哪些 Python 知识点。

## 回顾
### Day01 认识 Python
首先，第一天中我们主要讲解了什么是Python语言，并说明了如何下载历史版本。笔者比较的推荐版本为`3.8`、`3.9`和`3.10`均可，最新的版本3.11.x虽然有语法和性能提升。但有些第三方库，尤其是一些小众的没那么快适配，或者干脆不会升级的。另外版本的最终选择也要看实际工作中公司内部的已有代码程序的Python版本。

其次，我们在python shell做了些简单的使用练习，这种方式常常用于快速调试。在平常的实际项目开发中一般会用 IDE 开发工具，本系列中推荐的是免费的微软旗下的VS Code。当然还有其他工具如 Pycharm、jupyter、spyder、anaconda 和 atom 等。

最后，实战中讲解了Python的注释，它们是 `# 单行注释内容` 和 `'''多行注释内容'''`，另外还讲到了Python中的缩进是表示 `块` 的概念。同时使用Python shell 和 VS Code 简单演示了一些数据运算，以及Python的数据类型。其中我们要着重对几种数据集类型加以不同点区分：
- list：有序，项可重复，数据可操作
- tuple：有序（python 3.6+），项可重复，_**数据不可改变**_
- dict：无序，_**项不可重复**_，数据可操作
- set：无序，项可重复，数据可操作

详细学习回顾请阅读：_[认识Python](../readme.md)_

### Day02 变量和内置函数
第2天，上来我们先讲了有关Python内置函数的知识点，内置函数是一种全局的函数，在代码里无需额外引用直接使用。比如`print()`,`range()` 等。

然后我们讲到了无处不在的`变量`,主要是讲解命名、声明、赋值，这里我们再次回顾下它的命名规则：
- 变量名必须以字母或下划线字符开头
- 变量名不能以数字开头
- 变量名只能包含字母、数字字符和下划线（Az、0-9 和 _）
- 变量名区分大小写，如firstname、Firstname、FirstName 和 FIRSTNAME 是不同的变量

详细学习回顾请阅读：_[变量与内置函数](../02_Day_Variables_builtin_functions/02_variables_builtin_functions.md)_

### Day03 布尔值和运算符
第3天，首先认识了数据类型中的布尔值。它只有两值，即 `真` 和 `假`。应用场景就是进行相关逻辑判断得到True或False来决定下一步的操作。值这里总结强调的是大多数值都为 `True`。

另外一个重点是讲解了Python运算：
- 算数运算：加减乘除..
- 比较运算：大小等于..
- 逻辑运算：与或非..

详细学习回顾请阅读：_[布尔值和运算符](../03_Day_Operators/03_operators.md)_

### Day04 字符串str
第4天，围绕Python字符串类型，分别讲解和示例操作如何创建、拼接、特殊字符转义、三种格式化、多种访问方式，还另外大量举例了字符串本身的一些内置方法。

详细学习回顾请阅读：_[字符串](../04_Day_Strings/04_string.md)_

### Day05 列表list
第5天，首先学习了Python四种集合类型中的list，重点记住它是有序和可修改的。列表可以为空，也可以有不同的数据类型项。列表同样可以像字符串一样进行一些列的操作。如声明，数据的增删改访问，排序，拷贝，拆包等等。它是由方括号包裹起来的，形如：

```py
[1,2,3,4,5,6,7,8,9]
fruits = ['banana', 'orange', 'lemon']
```

详细学习回顾请阅读：_[列表list](../05_Day_Lists/05_lists.md)_

### Day06 元组tuple
第6天，来到的集合的第二种类型：元组。它是由一个括号包裹起来，并且一旦创建不可更改。仅有少量的方法可操作，具体为：
- `tuple()`：创建一个空的元组
- `count()`：计算元组中指定项的个数
- `index()`：返回指定项的索引值
- `+` ：连接两个或以上的元组成为新的元组

```py
pets = ('cat', 'dog')
```

详细学习回顾请阅读：_[元组tuple](../06_Day_Tuples/06_tuples.md)_

### Day07 集合set
第7天，set用于存储唯一项，它是无序且没有索引的，可理解为数学中的合集。因此它可以在集合之间进行查找并集、交集、差集、对称差集、子集、超集和不相交集。由大括号 {} 包裹，形如：
```py
seasons = set('spring','summer','autumn',"winter")
```
set 和 list 可以互转，这里有一个很巧的用途就是列表转集合可以对其进行去重。

详细学习回顾请阅读：_[集合set](../07_Day_Sets/07_sets.md)_

### Day08 字典dict
第8天, 学习集合类型中的最后一种字典，它是无序、可修改可变、成对的数据类型集合。也用 `{}` 表示，但区别与set的地方是内部的项目是 key: value 的形式。就是我们平常看到的json形式。
```py
info = {"nickname":"Qi", "profession":"IT农民工"}
```
字典可以增、改、删、检查、复制、将key或value转换成列表等操作。

详细学习回顾请阅读：_[字典dict](../08_Day_Dictionaries/08_dictionaries.md)_

### Day09 条件语句
第9天，默认情况下，Python脚本中的语句从上到下依次执行。如果有逻辑处理需要，可以通过以下两种方式改变执行的顺序：
- 条件执行：如果某个表达式为真，则执行这个语句块；
- 重复执行：只要某个表式一直为真，则会重复执行一个语句或块。

Python中的提交语句关键词为：如果`if`、否则`else`、否则如果`elif`。并且可以与逻辑运算符组合，也可以进行多层的嵌套。

详细学习回顾请阅读：_[条件语句](../09_Day_Conditionals/09_conditionals.md)_

### Day10 循环语句
第10天，Python编程语言提供以下两种循环，用于处理重复性的逻辑：
- while 循环
- for 循环

在循环中有两个重要的关键词break和continue注意区分使用。前者表示跳出整个循环，后者表示跳过本次循环。另外在编程中使用 `while(True)` 注意内部条件的处理，尽量不要出现死循环。

循环可以嵌套使用，最后还有一个比较好用的 range 来实现范围操作。

详细学习回顾请阅读：_[循环语句](../10_Day_Loops/10_loops.md)_

### Day11 函数
第11天，在前面的学习中，演示了大量的内置函数。这些函数都是为了解决一些特定的问题或者做一些逻辑事情。在日常的程序编写中，我们也可以自己定义函数。所谓函数是为了执行特定任务而设计可重用代码块或编程语句。在Python要定义或声明一个函数，使用了 `def` 关键字。
```py
def function_name():
    # todo 内部代码

def function_with_params(param1,param2):
    # todo 内部代码
```

在函数这篇中，学习了如何定义、声明和调用。并且了解的函数可以无参和带参，以及如何传递参数。最后函数也可以有返回值。

函数对于编程来说太重要了，各位一定要掌握牢固，并在有精力的情况下深入挖掘一下更高级的一些用法。

详细学习回顾请阅读：_[函数](../11_Day_Functions/11_functions.md)_

### Day12 模块
第12天，基于函数往上就是模块。它是在应用程序中一个包含一组代码或一组函数的文件。模块可以是包含单个变量、函数或大型代码库的文件。

模块的使用是通过导入和调用的方式。我们可以自定义模块，也可以使用系统默认的模块，更可以使用第三方库下的各种模块。掌握其应用快速编程实现程序功能。

详细学习回顾请阅读：_[模块](../12_Day_Modules/12_modules.md)_

### Day13 列表推导式和lambda
第13天，基于Day2-Day11 基本上我们就掌握了Python的基础。接下来的就是要学一些高级的内容以及实战应用。今天就是认识两个：
- 列表推导式： 又称列表解析式，提供了一种快捷的方法来创建列表。
```py
# 经典举例：生成0到10的数字
numbers = [i for i in range(11)]  
```

- lambda：是一个没有名字的小型匿名函数
```py
# 经典举例：实现一个两个数相加的匿名函数
lambda a, b: a + b
```

以上两种都是多复杂形态的逻辑代码和函数的一种简化操作。如果再加上些起其他逻辑可能有些绕，因此可以通过此篇详细。通过拆解对比来辅助理解。

详细学习回顾请阅读：_[列表推导式和lambda](../12_Day_Modules/12_modules.md)_

### Day14 高阶函数和闭包
第14天，主要理解两个内容：
- 高阶函数：是指能够接收其他函数作为参数、或者返回一个函数作为结果的函数；
- Python闭包：是指一个函数能够访问并操作其外部作用域中的变量，即使在函数外部调用它时仍然有效。

其中还举例三个比较典型的内置高阶函数：map()，filter() 和 reduce()。

详细学习回顾请阅读：_[高阶函数和闭包](../14_Day_Higher_order_functions/14_higher_order_functions.md)_

### Day15 Python错误类型
第15天，罗列和具体举例了Python的各种错误类型。了解编程语言中不同类型的错误将帮助我们快速调试代码，使其我们写的代码更加健壮。
    - [ImportError](#importerror)
这些错误类型包括但不限于：SyntaxError，NameError，IndexError，ModuleNotFoundError，AttributeError，KeyError，TypeError，ValueError，ZeroDivisionError。

详细学习回顾请阅读：_[Python错误类型](../15_Day_Python_type_errors/15_python_type_errors.md)_

### Day16 Python日期时间
第16天，时间在任何一种语言编程均很重要，比如标记时间进行性能计算，日志打印时间等。本篇中主要讲解 datetime 模块使用。使用它的一些方法进行日期时间获取，格式化操作。

详细学习回顾请阅读：_[Python日期时间](../16_Day_Python_date_time/16_python_datetime.md)_

### Day17 异常处理&参数打解包&Spread&枚举&Zip
第17天，此篇中囊括了好几个知识点有点散，让我们来回顾三个比较能到的，如下：
- 异常处理：之前我们讲到了Python的一些异常类，但实际编程中不能遇见和解决所有的错误，因此需要 `try except` 进行捕获，避免程序异常退出；
- 参数打解包：常用于参数较多（含不定参）和快速拆分赋值用。典型的是列表和字典的操作；
- 枚举：如果我们对列表的索引感兴趣，我们使用 *enumerate* 内置函数来获取列表中每一项索引。

当然还有另外两个 Spread 和 zip 具体用法参考详细文章。

详细学习回顾请阅读：_[异常处理&参数打解包&Spread&枚举&Zip](../17_Day_Exception_handling/17_exception_handling.md)_

### Day18 正则表达式
第18天，很多语言都有正则表达式，Python也不例外，应用中常用于模糊匹配查找逻辑中。在本篇中，首先你应该了解后半部分的基本的正则语法，然后再学会用 re 模块下方法：
- *re.match*: 只在字符串的第一行开始搜索，如果找到则返回匹配的对象，否则返回None。
- *re.search*: 如果字符串(包括多行字符串)中有匹配对象，则返回匹配对象。
- *re.findall*: 返回包含所有匹配项的列表，如果没有匹配则返回空列表。
- *re.split*:	方法按照能够匹配的子串将字符串分割后返回列表。
- *re.sub*:  查找并替换一个或者多个匹配项。

详细学习回顾请阅读：_[正则表达式](../18_Day_Regular_expressions/18_regular_expressions.md)_

### Day19 文件处理
第19天，讲解了关于文件处理的Python代码示例。介绍了如何处理不同类型的文件，包括txt、json、csv、xlsx和xml文件。
- 首先，使用open()函数打开文件的不同模式（读取、追加、写入、创建）以及文本模式和二进制模式的区别。
- 接下来，展示了如何读取txt文件的内容，包括使用read()方法读取整个文件、readline()方法逐行读取文件和readlines()方法按行读取文件并返回一个行列表。
- 然后，展示了如何向已有的txt文件中追加内容，以及如何使用open()函数的mode='w'参数来覆盖写入文件。

文本中还介绍了如何使用json模块将JSON字符串转换为字典（json.loads()）以及将字典转换为JSON字符串（json.dumps()）。此外，还展示了如何将字典保存为JSON文件（json.dump()）。

其他还简单演示了：
- 对于csv文件，文本演示了如何使用csv模块读取csv文件，并遍历行和列数据。
- 对于xlsx文件，文本提到需要安装xlrd库，并演示了如何打开和读取xlsx文件。
- 最后，对于xml文件，文本使用xml.etree.ElementTree模块解析了xml文件，并展示了如何获取根标记、属性和子元素的信息。

详细学习回顾请阅读：_[文件处理](../19_Day_File_handling/19_file_handling.md)_

### Day20 PIP包管理
第20天，Python语言的广受大家欢迎的原因除了入门学习简单上手快，还有就是它有很多贡献者们发布的包。利用这些包可以快速实现自己代码程序。而这些包的管理最常用的包管理之一就是PIP。本文中我们详细讲解了安装、卸载、查看、生成项目包依赖，并且了解了如何能够创建自己的发布包。

详细学习回顾请阅读：_[PIP包管理](../20_Day_Python_package_manager/20_python_package_manager.md)_

### Day21 类和对象
第21天，Python程序中的每个元素都是类的对象，包括它的属性和方法。

本篇首先解释了什么是类和对象，类被定义为具有相似特征和行为的对象的模板，而对象是类的具体实例。然后，深入探讨了如何创建类和实例化对象，并介绍了类中常见的成员，如属性和方法。

接下来还讨论了类之间的继承关系，说明了如何创建子类以及如何继承和重写父类的属性和方法。它还介绍了多重继承的概念，并提供了一些注意事项和最佳实践。

详细学习回顾请阅读：_[类和对象](../21_Day_Classes_and_objects/21_classes_and_objects.md)_

### Day22 Web爬虫
第22天，简单介绍了数据抓取的编程方法。核心用到了两个包 `requests` 和 `BeautifulSoup`。最后在课后作业中给出了一个用于实际操作的练习靶场。数据爬虫是Python工程一个分支。本篇只是入门，如果想在此方面专项发展，还需要单独进行深入学习的。

详细学习回顾请阅读：_[Web爬虫](../22_Day_Web_scraping/22_web_scraping.md)_

### Day23 虚拟环境
第23天，虚拟环境可以创建一个隔离或分离的环境。这将帮助我们避免项目间依赖关系的冲突。常用并推荐的两个虚拟环境管理包：
- virtualenv
- anaconda

详细学习回顾请阅读：_[虚拟环境](../23_Day_Virtual_environment/23_virtual_environment.md)_

### Day24 Python统计分析
第24天，本篇主要介绍了statistics模块，它是计算数值数据的数学统计的函数，主要用于绘图和科学计算。另外还有NumPy是Python中科学计算的核心库，它提供了高性能的多维数组对象和处理数组的工具。同爬虫一样数据统计分析也是Python领域里一个分支。如果你想深造请学习更多内容。

详细学习回顾请阅读：_[Python统计分析](../24_Day_Statistics/24_statistics.md)_

### Day25 Pandas
第25天，Pandas是一个开源的Python库，提供了高效、灵活和易于使用的数据结构和数据分析工具。它是数据科学和数据分析中的常用工具之一，广泛应用于数据清洗、处理、转换和分析的任务。

详细学习回顾请阅读：_[Python Pandas](../25_Day_Pandas/25_pandas.md)_

### Day26 Python web
第25天，Python是个强大语言，同样可以用于Web服务的开发。本篇主要通过 Django和Flask 作为实战的例子进行简单的WEB开发。当然这篇中涉及到前端需要你了解一些HTML\CSS的基础。同样内容只是引路，在当今内卷的前端框架面前，有很多方案，比如vue、react等等。

详细学习回顾请阅读：_[Python web](../26_Day_Python_web/26_python_web.md)_

### Day27 Python MongoDB
第27天，有服务就会有数据的持久化。本篇主要介绍非关系型数据MongoDB，通过阅读这篇文章，可以了解如何使用Python与MongoDB进行交互，并掌握基本的插入、查询、更新和删除文档的操作。文内提供了丰富的示例代码和解释，帮助快速上手使用Python与MongoDB进行数据处理和管理。

详细学习回顾请阅读：_[Python MongoDB](../27_Day_Python_with_mongodb/27_python_with_mongodb.md)_

### Day28 Python Mysql
第28天，另外一个非常常用数据就是关系型的Mysql，笔者大奇额外补充了一篇。从环境搭建、配置，数据库创建、使用，表的增删改查都做了详细的演示。

详细学习回顾请阅读：_[Python Mysql](../28_Day_Python_with_mysql/28_python_with_mysql.md)_

### Day29 Python API
第29天，最后一篇算是综合应用。首先是讲解了HTTP的基础，回顾两个核心请求方法：
- GET：GET方法用于通过给定的URI从给定的服务器检索和获取信息。使用GET的请求应该只检索数据，并且不应对数据产生其他影响。
- POST：POST请求用于创建数据并将数据发送到服务器，例如，使用HTML表单创建新的帖子、文件上传等。

最最后，拿了学生数据的例子，综合数据操作实现一个 RESTful API 服务。

详细学习回顾请阅读：_[Python API](../29_Day_API/29_API.md)_

## 推荐&结束语

到这里，历时半年整个Python基础学习系列完结。但学习是永不能止步的，笔者会继续分享更多的内容。这里推荐我的另外一个真实战系列 https://github.com/QiCodeCN/TestProjectManagement ，它主要是通过0-1手把手教你实现的测试平台，其中后端服务就是Python实现。如果你感兴趣欢迎阅读它。并持续关注。

如果你对本系列表示有用，请给作者项目微不足道的小星星，也希望能推荐给更多人阅读学习。


[<< Day 29](../29_Day_Building_API/29_building_API.md)




