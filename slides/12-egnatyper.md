# Egendefinierade typer

```go
type Greeting struct {
    // medlemmar med liten första bokstav = private
    language string
    // medlemmar med stor första bokstav = public
    Message string
}

func (g *Greeting) Perform() {
    fmt.Println(g.Message)
}

greeting := Greeting{
    language: "sv",
    Message: "Hej!",
}

greeting.Perform()
```
