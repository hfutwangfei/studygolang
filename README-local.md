### 步骤

1. 将项目`studygolang`拷贝至`$GOPATH`目录下

    > 参考`db/conn.go`中调用包`github.com/polaris1119/config`对配置文件的路径解析

2. 项目目录下执行`go mod tidy`

3. 按步骤`make build`, `make start`即可
    > 注意: 先创建数据库和表
    > > mysql> source $GOPATH/studygolang/config/db.sql
    > >
    > > mysql> source $GOPATH/studygolang/config/init.sql
    > >
    > > 在config目录中添加配置文件`env.init`, 其中注意修改mysql相关配置
