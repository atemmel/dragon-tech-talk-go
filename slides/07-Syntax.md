# Syntax

```go
x := 0
var x int = 0
var x = 0
```
```go
func swap(x, y string) (string, string) {
    return y, x
}
```
```go
func main() {
    i, j := 42, 2701

    p := &i         // point to i
    fmt.Println(*p) // read i through the pointer
    *p = 21         // set i through the pointer
    fmt.Println(i)  // see the new value of i

    p = &j         // point to j
    *p = *p / 37   // divide j through the pointer
    fmt.Println(j) // see the new value of j
}
```
