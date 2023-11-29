# Egendefinierade typer

```go
type Halsning struct {
sprak string
meddelande string
}

func (h *Halsning) Perform() {
fmt.Println(h.meddelande)
}
```