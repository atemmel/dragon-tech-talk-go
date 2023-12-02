# Egendefinierade typer forts.

```go
type Id int

func (i *Id) Print() {
    fmt.Println("Id är", i)
}

var id Id = 0

id.Print()
```
