# Python基础考察

## 1.可变类型和不可变类型
##### python所谓的可变不可变，是指其内存存储那块区域是否可变
* 不可变类型：数值、字符串、元祖  
* 可变类型：列表、字典  
**对于不可变类型：**  
```a = 1```  
```b = 1```  
```a is b```   
```Out: True```  
这里a和b都是对同一块内存‘1’的引用  
![blockchain](https://raw.githubusercontent.com/WeiHsuBH/Python-Learning/master/imgs/a%3Db%3D1.png)  
若再令  
```b = 3.14159```  
此时将在内存开辟出新的一块，里面内容为‘3.14159‘  
b更改为对‘3.14159‘的引用  
![blockchain](https://raw.githubusercontent.com/WeiHsuBH/Python-Learning/master/imgs/a%3D1b%3D314159.png)  
**对于可变类型：**  
