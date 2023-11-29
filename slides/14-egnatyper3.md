# Egendefinierade typer forts.

```go
type Id int

func (i *Id) print() {}

func calc(siffra Id){
//gör någonting med siffran
}

var id Id = 0

id.print()

calc(id) // borde fungera
```
