# 使用 Go 构建分布式服务

## 运行

```cmd
cd proglog
go run main.go
```

## 测试

使用 HTTPie 发送 post 请求，请求地址`http://locahost:8080`

请求参数:

```json
{
  "record": {
    "value": "tertet"
  }
}
```

响应参数：

```text
{"offset":0}
{"offset":1}
{"offset":2}
...
```

每次请求 offset 的值都会递增
