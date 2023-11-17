# Goroutines

```go
package main

import (
    "fmt"
    "time"
)

func task(seconds time.Duration, msg string) {
    time.Sleep(time.Second * seconds)
    fmt.Println(msg)
}

func main() {
    go task(2, "Hello")
    go task(1, "World")

    time.Sleep(2 * time.Second)
}
```
