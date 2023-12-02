# Pointers

```go
func main() {
    i, j := 42, 2701

    p := &i                  // peka på/referera till i
    fmt.Println("*p är", *p) // läs i genom pointern
    *p = 21                  // skriv till i genom pointern
    fmt.Println("i är", i)   // skriv ut i

    p = &j                   // peka på/referera till j istället
    *p = *p / 37             // dividera j genom pointern
    fmt.Println("j är", j)   // skriv ut det nya värdet på j
}
```
