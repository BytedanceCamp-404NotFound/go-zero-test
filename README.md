# go-zero-test
测试传代码


# 编译
```shell
cd greet
go run greet.go -f etc/greet-api.yaml
```

# 调试
在任何位置启动F5都可以使用，但是需要先编译


## 创建go-zero
```shell
goctl api new great   # 多了一个整个great文件夹
go mod tidy
```

## 修改API
goctl api go -api greet.api -dir . -style go_zero
goctl api go -api greet.api -dir . -style gozero

# 启动go-zero
```shell
cd greet
go run greet.go -f etc/greet-api.yaml
```
# 测试go-zero
```shell
curl -i -X GET http://localhost:8888/from/you
```
浏览器中打开
http://[自己IP地址]:8080/from/you


# 未来计划

增加Action自动化构建

# 参考资料

https://go-zero.dev/cn/docs/quick-start/monolithic-service
https://go-zero.dev/cn/docs/goctl/goctl/
https://go-zero.dev/cn/docs/goctl/goctl/