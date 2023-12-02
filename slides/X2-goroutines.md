# Goroutines

```go
package main

import (
    "fmt"
    "time"
)

func task(seconds time.Duration, msg string) {
    time.Sleep(time.Second * seconds) // sov
    fmt.Println(msg) // skriv ut meddelandet
}

func main() {
    // kör den här funktionen i en ny goroutine
    go task(2, "Hello")
    // - " -
    go task(1, "World")

    // invänta
    time.Sleep(2 * time.Second)
}
```
