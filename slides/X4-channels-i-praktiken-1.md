# Channels i praktiken

Den här applikationen är multitrådad!

Vid uppstart så:

1. Läses det in ett slidemanifest (kraftfil)
2. En ny goroutine skapas per slide i kraftfil
3. Huvudrutinen inväntar svar via en channel
