# first order functions

```go
func caller (fn func()){
    fn()
}

x := func(){
	 fmt.Println("printing x")
}

caller(x)
```