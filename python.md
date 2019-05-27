## mac安装mysqlclient
```
brew install mysql-client
# mysql-client is not on the `PATH` by default
export PATH="/usr/local/opt/mysql-client/bin:$PATH"
# openssl is not on the link path by default
export LIBRARY_PATH="$LIBRARY_PATH:/usr/local/opt/openssl/lib/"

pip install mysqlclient
```
