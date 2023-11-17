# Channels

```go
package main

import "fmt"

func send(c chan string) {
    c <- "Järnjätten"
}

func main() {
    c := make(chan string)

    send(c)

    msg := <- c

    fmt.Println(msg)
}
```
