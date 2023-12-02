# Egendefinierade typer forts.

```go
type Id int

func calc(i int) {
    //gör någonting med i
}

var id Id = 0

calc(id) // fungerar inte

// explicit typomvandling
calc(int(id)) // fungerar
```
