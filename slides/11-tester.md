# Tester

* för varje fil finns en motsvarande testfil 
* t.ex hej.go skulle ha hej_test.go som testfil

```go
// testing.T är ett allmänt testobjekt som Go's runtime
// tillhandahåller varje funktion som innehåller tester

func TestAbs(t *testing.T) {
    got := Abs(-1)
    if got != 1 {
        t.Errorf("Abs(-1) = %d; want 1", got)
    }
}
```
