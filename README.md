# Python基础考察

## 1.可变类型和不可变类型
##### python所谓的可变不可变，是指其内存存储那块区域是否可变
* 不可变类型：数值、字符串、元祖  
* 可变类型：列表、字典  
**对于不可变类型：**  
```a = 1```  
```b = 1 #a,b指向同一个内存对象```  
```a is b```   
```Out: True```  
这里a和b都是对同一块内存‘1’的引用  
![blockchain](https://raw.githubusercontent.com/WeiHsuBH/Python-Learning/master/imgs/a%3Db%3D1.png)  
若再令  
```b = 3.14159```   
b更改为对‘3.14159‘的引用  
![blockchain](https://raw.githubusercontent.com/WeiHsuBH/Python-Learning/master/imgs/a%3D1b%3D314159.png)  
改变不可变类型的值，其实是让引用指向另外一个对象  
**对于可变类型：**  
先拿列表来举个例子  
```a = [1, 2, 3]```  
此时列表a在内存中的结构如下图所示：  
![blockchain](https://raw.githubusercontent.com/WeiHsuBH/Python-Learning/master/imgs/list1.png)  
列表中直接存储的是元素的地址，并不直接存储元素  
此时若令  
```a[0] = 10```  
![blockchain](https://raw.githubusercontent.com/WeiHsuBH/Python-Learning/master/imgs/list3.png)  
改变的是该列表对象的第一个元素指向的地址  
若对a重新赋值  
```a = [1, 2, 3]```  
![blockchain](https://raw.githubusercontent.com/WeiHsuBH/Python-Learning/master/imgs/list2.png)  
此时新建一个列表对象，但是其内的元素地址还是原来的地址，因为数值类型是不可变类型

## 2.python的参数传递
