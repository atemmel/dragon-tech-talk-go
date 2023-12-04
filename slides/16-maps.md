# map

```go
table := map[string]int{}     // skapa en string -> int mappning
table := make(map[string]int) // -"-

table["hej"] = 5 // sätt in värden i map

fmt.Println(table["hej"]) // hämta värde och skriv ut

// kontroll ifall nyckeln finns
value, ok := table["hello"]
if ok {
    fmt.Println("hello är", value)
} else {
    fmt.Println("hello finns inte som nyckel i table")
}
```
