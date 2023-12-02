# Channels i praktiken

Den här applikationen är multitrådad!

Vid uppstart så:

1. Läses det in ett slidemanifest (kraftfil)
2. Slidemanifestet innehåller en lista av markdownfiler (slides)
2. En ny goroutine skapas per slide i kraftfilen
2. Goroutinen öppnar filen samt läser och parsar dess innehåll
2. När goroutinen är klar skickar den ett meddelande via en kanal
3. Huvudrutinen som skapat alla goroutiner inväntar allas svar
