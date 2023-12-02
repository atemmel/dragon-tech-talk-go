# Channels

```go
package main

import "fmt"

func send(c chan string) {
    // skicka meddelande till kanal
    c <- "Järnjätten"  
}

func main() {
    // skapa en ny kanal
    c := make(chan string)

    go send(c)

    // läs ut meddelande ur kanalen
    msg := <- c

    fmt.Println(msg)
}
```
