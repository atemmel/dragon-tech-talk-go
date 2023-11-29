# Egendefinierade typer forts.

```go
type Id int

func calc(siffra int){
//gör någonting med siffran
}

var id Id = 0

calc(id) // borde inte fungera



```
func (i *Id) print() {}