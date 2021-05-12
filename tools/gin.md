# How to use [gin](https://github.com/codegangsta/gin) for code hot reload when dev.
# 开发过程中如何用 [gin](https://github.com/codegangsta/gin) 来做代码热重启

- go get github.com/codegangsta/gin
- add .env file, put your env variables.
- main.go add this:

```go
if *configPath == "" {
  *configPath = os.Getenv("CONFIG_PATH")
}
```

- add run.sh
- in your iTerm2, run this:
```shell
chmod 777 run.sh
```
```shell
./run.sh
```
- in your .gitignore add this, to ignore gin-bin file
```shell
gin-bin
```

# Happy Coding!
