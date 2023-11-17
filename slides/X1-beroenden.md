# Beroenden

```go
package main // berättar vilket paket nuvarande fil hör till

import (
    // eventuella beroenden
    "github.com/veandco/go-sdl2/sdl"
)

func main() {
    sdl.Init(sdl.INIT_EVERYTHING)
    window, err := sdl.CreateWindow("Hello, World", 0, 0, 400, 300)
    defer window.Destroy()

    screenSurface = SDL_GetWindowSurface(window);
    SDL_FillRect(screenSurface, NULL, SDL_MapRGB(screenSurface->format, 255, 255, 255));
    SDL_UpdateWindowSurface(window);
    SDL_Delay(2000);
    SDL_DestroyWindow(window);
    SDL_Quit();
}
```
