# Novaro-Backend

## Login

http://127.0.0.1:8080/v1/auth/ to login with twitter directly

http://127.0.0.1:8080/v1/auth?icode=12345678 to login with invitation code firstly and then with twitter

## Invitation Codes

### Generate

```
GET http://127.0.0.1:8080/v1/api/invitation/codes/add

Cookie: {cookie}
```

Get the cookie after you login

### Check the exist invitation codes

invitation_codes table in the db


1.Run
```
go mod tidy
go run src/main.go | tee out.log
```

2.[REST API](./api/REST-API.http)

Windows本地运行Go项目

```
# 安装后端依赖包
go mod tidy

# 启动后端服务
go run cmd/main.go
```
