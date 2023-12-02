# first order functions

```go
// funktion som tar in en funktion
func caller (fn func()) {
    fn()
}

// funktion som ett uttryck
x := func() {
    fmt.Println("Nu körs x")
}

caller(x)
```
