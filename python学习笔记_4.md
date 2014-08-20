#python学习笔记 4

## 4字典

	原来的方式:
	names = ['a','b','c']
	numbers = ['23','34','45']
	numbers[names.index('c')]
	
###4.2
phonebook={'a':'12','b':'23','c':'34'}

####4.2.1 dict函数

	通过其他映射或者键值这样的序列建立字典
	items = [('name','a'),('age','20')]
	d = dict(items)
	d['name']  --> a
	或者这样:
	d = dict(name='gary',age=42)	
	d -->{'age':42,'name':gary}
	
	
	
	
	
----

下面这部分不是很清楚 没有仔细看


####4.2.2 基本字典操作

	与序列(sequence)类似
	
	P57
	
####4.2.3 字典的格式化字符串


####4.2.4 字典方法
	
	clear
	
	copy
	
	fromkeys
	
	get
	
	has_key
	
	items iteritems
	
	pop
	
	popitem
	
	setdefault
	
	update
	
	values itervalues
	
	
	
	

