# Tester

* för varje fil finns en motsvarande testfil 
* t.ex hej.go skulle ha hej_test.go som testfil

```go
func TestAbs(t *testing.T) {
    got := Abs(-1)
    if got != 1 {
        t.Errorf("Abs(-1) = %d; want 1", got)
    }
}
```
