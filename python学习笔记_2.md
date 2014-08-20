#python学习笔记 2

## 2列表和元组

	
最基本的数据结构:序列

序列简介 对所有序列(包括元组和列表)都通用的操作,这些操作也适用于字符串.

然后开始学习使用列表,元组

6种内建序列 包括最常用的列表 元组,还有 字符串(下章) Unicode buffer对象 xrange对象

例如:
	
	edward = ['Edward Gumby',42]
	john = ['john',50]
	database = [edward,john]
	database

###2.2通用序列操作:
	
	索引
	分片
	加
	乘
	成员资格
	计算长度
	找最大最小元素
	迭代(5.5)

索引:

[x]
	
	greeting = 'hello'
	greeting[0]  -->H
	greeting[-1]  -->o
	
	还可以直接对返回结果操作
	fourth = raw_input('year:')[3]
	year=2005 fourth -->5
	
	还有这个 1-31日结尾
	endings = ['st','nd','rd'] + 17 * ['th'] \
		+['st','nd','rd'] +7 * ['th'] \
		+ ['st']
		
	
分片:
 
访问一定范围内的元素

	tag = 'http:www.sagagasdgas.com/asgfasgd'
	tag[9:30]
	tag[32:-4]
	
	number = [1,2,3,4,5,6,7,8,9]
	number[3,6] 含第一个元素,第二个不包含 456
	number[-3:] 倒数第三个到最后一个 number[:3]
	步长:
	number[3:6:3]	距离内间隔
	number[::4]		每隔指定间隔
	number[10:0:-3] 还可以倒着来

序列相加:
	
	'hello'+'world'
	'helllo'+[1,2,3]
	
乘法:

	重复n遍:
	'python' * 5   -->'python......'
	[42] * 10  [42,42....]
	' ' * text_width来打印格式宽度
	
成员资格:

	in运算符
	
	permission = 'rw'
	'w' in permission true
	
	database = [
	['a','pass1'],
	['b','pass2'],
	['c','pass3']
	]
	username = row_input('user name')
	pass = row_input('PIN code')
	if [username,pass] in database:print 'ok'
	
	
长度和最大值 最小值

	max len min
	max(number)
	

	
### 2.3列表

列表:

	list函数
	
	列表基本操作:改变;删除;分片:赋值.替换.插入.删除
	
	列表方法:append;count;extend;index;insert;pop;remove;reverse;sort;高级排序
	
	
list函数:

	字符串有时不能被方便的修改所以需要有时候由字符串创建列表
	list('hello') --> ['h','e','l','l','o']
	list函数适用于所有类型的序列,而不只是字符串
	
基本操作:
	
	改变:即第一章的赋值 :x[1]=2
	删除:del name[2]name = ['a','b','d']
	分片:分片赋值(插入 删除 替换均可实现):name=list('perl');name[2:]=list('ar') ;name[1:1]=[2,2,3]
	
列表方法:
	
	方法是与某些对象有紧密联系的函数,对象可能是列表数字也可能是字符串或者其他类型的对象
	对象的调用:对象.方法(参数)
	
	1st = [1,2,3]
	1st.append(4) 追加
	
	count:x.count(1)

	extend a.extend(b) 和连接操作的区别:修改了原列表 同a[len(a):] = b
	
	index 找出第一个匹配项的索引位置	night.index('harry')
	
	insert number.insert(3,'four') 等同于number[3:3] = ['four']
		
	pop x.pop() 出栈
	
	remove 移除列表中某个值的第一个匹配项 没有返回值 x.remove('be')
	
	reverse 将元素反向存放 没有返回值  x.reverse();
	
	sort 	没有返回值,如果想得到排序后的并且和原列表不变 y=x.sort(); 不可以 需要先把x副本给y再排序
		y=x[:] 或者 sorted函数 y=sorted(x)
		
	高级排序:
		x.sort(key=len)
		
			
	
	
		
	
	
	
### 2.4元组

不可变序列(字符串也是这样)	
	圆括号 逗号括起来(一个值也得有逗号)
	(1,2,3)
	
	3*(40+2)=126
	3*(40+2,) -->(42,42,42)
	
tuple函数:

	与list函数基本一致,将一个序列作为参数并转为元组 
		tuple([1,2,3])
	
作用:
	元组可以在映射中当做键使用而列表则不行
	??
	
	
	
----
