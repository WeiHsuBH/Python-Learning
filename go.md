# golang安装配置  
1. 官网下载安装包  
下载地址：``https://golang.org/dl/``  
终端进入下载的目录，运行以下命令  
``sudo tar -C /usr/local -xzf xxxxxxxx.tar.gz``  
``xxxxxxxx.tar.gz``为对应安装包名称  
将``/usr/local/go/bin``添加进环境变量  
在``/etc/profile``或者``$HOME/.profile``里  
``export PATH=$PATH:/usr/local/go/bin``  
若有多个项目需要添加$GOPATH,ubuntu系统下使用``:``分割  
``export PATH=$PATH:/usr/local/go/bin:/home/asd/``  


2. vscode配置golang调试  
首先安装dlv  
``go install github.com/derekparker/delve/cmd/dlv``  
安装完成启动dlv  
``dlv debug --headless --listen=:2345 --log``  
之后配置文件的设置如下  
```
{
    "version": "0.2.0",
    "configurations": [
        {
            "name": "Launch",
            "type": "go",
            "request": "launch",
            "mode": "debug",
            "remotePath": "",
            "port": 2345,
            "host": "127.0.0.1",
            "program": "${fileDirname}",
            "env": {
                "GOPATH":"D:/Develop/vscodegolang"
            },
            "args": [],
            "showLog": true
        }
    ]
}
```  
其中``program``为主go程序的地址  
``args``里配置启动命令行其他参数文件的地址  
比如``"args": [
                "/home/xw/xx/xx-go-projects/conf/server-v1-test.toml"
            ]``
