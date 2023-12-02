# Felhantering

```go
// os.ReadFile har signaturen:
// func ReadFile(filename string) ([]byte, error)

// error är en unik typ som antingen får innehålla 
// ett felmeddelande eller nil
// (nil är Go's svar till null, None, nullptr, etc...)

bytes, err := os.ReadFile("minfil.txt")
if err != nil {
    panic(err)
}

// gör något med bytes...
```
