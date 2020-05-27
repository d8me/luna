## Luna
#### Alice inspired chaining for Fasthttp(https://github.com/valyala/fasthttp).
Luna provides a way to chain 

In short, it transforms

```go
Middleware1(Middleware2(Middleware3(App)))
```

to

```go
luna.New(Middleware1, Middleware2, Middleware3).Then(App)
```