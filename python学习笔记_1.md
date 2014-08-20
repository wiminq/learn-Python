#python学习笔记 1

<python基础教程 第二版>

## 1基础知识


1/2 	3.0之前的整数除法

__future__

整数除法://

-3**2 等价于 -(3**2)

长整类型:L

3.0中print是函数 需要print (42) 而不是print 42

x=input ("x:")

函数:

模块:import导入模块 然后按照模块.函数的格式使用
import math
math.floor(32.9)

如果确定函数名不会重复就可以采用 from math import sqrt 的方式可以不需要模块名再写了 >>>sqrt(9)


引号问题:

	\反斜线转义
	"\"hello \"she said"
	
	
str和repr

	str让字符串更易于阅读,repr让结果字符串转换为合法的python表达式
	
	print str("hello ") 	hello
	print repr("hello")  'hello'
	
	
input 和raw_input

	如果不是必须最好使用raw_input input需要输入的类型必须是合法的表达式(双引号)
	

长字符串 换行

	用三个引号 或者\反斜线换行
	
原始字符串
	
	不会转义 例如 hello\nworld 但是如果想真的使用\n就需要要么使用\\转义或者 print r'c:\nowhere'(但是最后一个字符不能是反斜线,如果必须有可以把反斜线单独作为一个字符串来处理)
	
	'c\pro' '\\'
	
	
	
	
	
	
	
		
	
	
	
	
	
	
	
	
	
	