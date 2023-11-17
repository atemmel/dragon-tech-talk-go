# Channels i praktiken, forts.

```go
type Result struct {
    Slide
    Number int
}

// skapa upp en kanal
channel := make(chan Result)

// kraftfilen återfinns i files
for i, file := range files {
    // inläsning delegeras till ny goroutine
    go readSlide(channel, file, i)
}

// skapa upp array av storlek N att hålla resultaten
slides := make([]Slide, len(files))

// invänta N resultat från kanalen
for i := 0; i < len(files); i++ {
    result := <-channel
    slides[result.Number] = result.Slide
}

// klart!
```
