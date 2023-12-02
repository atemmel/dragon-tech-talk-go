# Interfaces

```go
package main

import "fmt"

// skapa ett interface
type Animal interface {
    Noise() string
}

type Duck struct {}

func (d *Duck) Noise() string {
    return "Kvack!"
}

func print(animal Animal) {
    fmt.Println("Djuret säger", animal.Noise())
}

func main() {
    duck := &Duck{}
    // Duck blir implicit ett Animal, eftersom den
    // tillfredsställer alla metoder Animal begär
    print(duck)
}
```
