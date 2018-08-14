# Working-experience
## 1. SSH免密登陆
  本地操作系统 ubutnu16.04LTS  
1.```Ctrl```+```Alt```+```T```打开终端  
2.终端输入```ssh-keygen -t rsa```  
3.一直按回车，之后```cd .ssh/```，生成两个文件```id_rsa id_rsa.pub```  
4.将pub的内容拷贝到服务器上```.ssh/```下的```authorized_keys```中，```authorized_keys```的权限需设置为600。  
  
## 2. PYTHON启动设置环境变量
```PY_ENV=test python run.py```  
## 3. 
