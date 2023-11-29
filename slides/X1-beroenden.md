# Beroenden

```go
package main // berättar vilket paket nuvarande fil hör till

import (
    // eventuella beroenden
    "github.com/veandco/go-sdl2/sdl"
)

func main() {
    sdl.Init(sdl.INIT_EVERYTHING)
    defer sdl.Quit()
    window, _ := sdl.CreateWindow("Hello, World", 0, 0, 400, 300, 0)
    defer window.Destroy()
    surface, _ := window.GetSurface()
    surface.FillRect(nil, sdl.MapRGB(surface.Format, 255, 0, 255))
    window.UpdateSurface()
    sdl.Delay(5000)
}
```
