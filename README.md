# 工作记录
## 1. SSH免密登陆
  本地操作系统 ubutnu16.04LTS  
1. ```Ctrl```+```Alt```+```T```打开终端  
2. 终端输入```ssh-keygen -t rsa```  
3. 一直按回车，之后```cd .ssh/```，生成两个文件```id_rsa id_rsa.pub```  
4. 将pub的内容拷贝到服务器上```.ssh/```下的```authorized_keys```中，```authorized_keys```的权限需设置为600。  
  
## 2. PYTHON启动设置环境变量
```PY_ENV=test python run.py```  
## 3. Markdown语法
1. 标题  
使用#，一个#到六个#分别为一级标题至六级标题  
2. 列表    
无序列表和有序列表  
  ```  
  * 第一项  
  * 第二项  
  * 第三项  
  ```  
  ```  
  1. 第一项  
  2. 第二项  
  3. 第三项  
  ```  
3. 引用  
  引用只需在文本前加上```>```即可，```>```与文字之间需要加上空格  
  ```> 这是一个引用```效果如下：  
  > 这是一个引用  
4. 图片与链接  
图片：```![]()```  
链接：```[]()```  
5. 粗体与斜体  
两个```*```包含一段文本就是粗体的语法，用一个```*```包含一段文本就是斜体  
**这是一个粗体**  
*这是一个斜体*
6. 表格  
表格的上一行必须为空行  
```| Name     | Age      | Gender   |  
| -------- | -------- | -------- |  
| Xiaohong | 20       | Man      |  
| Xiaolv   | 19       | Women    | 
```  

| Name     | Age      | Gender   |  
| -------- | -------- | -------- |  
| Xiaohong | 20       | Man      |  
| Xiaolv   | 19       | Women    |    
7. 代码框  
``int a = 10; # 两个`包起来的效果``   
```int a = 10; # 三个`包起来的效果```  
好像没啥区别,还是两个方便一些  
8. 分割线  
分割线的语法只需要三个 * 号，比如  
***  
参考：[Markdown——入门指南 Te_Lee](https://www.jianshu.com/p/1e402922ee32/)  
# 4. Ubuntu16.04 LTS Mongodb  
1. 安装mongodb
从[官方下载](https://www.mongodb.org/dl/linux/x86_64-ubuntu1604)中下载对应安装包。  
下载完成后在终端中解压tar文件：  
``tar -zxvf mongodb-linux-x86_64-ubuntu1604-v3.2-latest.tgz``  
将解压后的文件夹移动到指定的目录：  
``mv mongodb-linux-x86_64-ubuntu1604-3.2.20-23-g96349e6/ /usr/local/mongodb``  
将Mongodb的可执行文件添加到PATH中：  
``export PATH=/usr/local/mongodb/bin/:$PATH``  
2. 创建数据库目录  
``mkdir -p /data/db``  
**/data/db 是 MongoDB 默认的启动的数据库路径(--dbpath)**  
3. 启动mongodb服务  
默认mongodb是启动着的  
手动启动的话``mongod``  
# 5. Git使用  
拷贝Git仓库 ``git clone [url]``  
添加文件至缓存 ``git add file_name1 [file_name2]``  
将缓存区内容添加到仓库 ``git commit -m "说明"``  
删除文件 ``git rm file``  
移动或重命名一个文件、目录、软连接 ``git mv a b``  
列出所有分支 ``git branch``  
创建分支 ``git branch (branchname)``  
创建新分支并立即切换到该分支下 `` git checkout -b (branchname) ``  
切换分支 ``git checkout (branchname)``  
删除分支 ``git branch -d (branchname)``  
合并分支 将b合并到a，在a中 ``git merge b``  
待学习完善  
# 6. To Do

