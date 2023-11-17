# Interfaces

```go
package main

import "fmt"

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
    print(duck)
}
```
