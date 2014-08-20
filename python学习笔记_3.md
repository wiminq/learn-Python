#python学习笔记 3
## 3使用字符串
	
所有的标准序列操作(索引.分片.乘法.判断成员资格.求长度.取最小值和最大值)字符串同样适用.但是字符串是不可变的

字符串格式化操作:
	
	%s 转换说明符
	>>>format = "hello %s,%s "
	>>>values = ('qin','chenbo')	
	>>>print format % values
	%.3f	
	
模板字符串:

	string模块 substitute模块方法 类似shell 的变量替换
	
	>>>from string import Template
	>>>s = Template('$x.glorious $x!')
	>>>s.substitute(x.'slurm')
	'slurm,glorious slurm'
	
	....
	
字符串格式化操作:

	>>>'%s plus %s equals $s ' % (1,2,3)
		1 plus 2 equals 3
	>>>'%s plus %s equals $s ' % 1,2,3  wrong
	
	转换标志:-左对齐;+表示转换前加上正负号;....
	最小字段宽度:转换后的字符串至少应该具有该指定的宽度
	.后跟精度值 小数点位数;最大字段宽度;
	转换类型:d e s r...等
	
	例如:'%-10.2f' % pi	字宽10 精度2
	print ('%+5d' % 10) +'\n' + ('%+5d' % -10)
	
	书上的例子搞得不是很清楚
	
### 3.4字符串方法

字符串方法实在太多 可以在附录中找

	string模块不仅包含字符串方法,还有一些不能作为字符串方法适用的常量和函数
	例如string.digits 常量
	
	find
		'with a here bird '.find('bird')
		title = "monty 's flying"
		title.find('monty')
		subject.find('!!!',0,16)
	join
		split的逆方法,用来在队列中添加元素
		seq = [1,2,3]
		sep = '+'
		seq.join(sep) #连接数字列表,不对
		seq = ['1','2','3']
		seq.join(sep) #连接字符串列表,对
				
	lower
		返回字符串小写
		name =
		names = 
		if name.lower() in names:print 'find it'
		
	replace
		'this is a test'.replace('is','eez')
		
	split
		默认为所有的空格
		'1+2+3+4'.split('+')
		['1','2',..]
	strip
		去除两侧的指定符号(默认为空格)
	translate
		只替换字符串中的某些部分,单个字符,但是可以多个替换
	
	
	
	
	
	
	
