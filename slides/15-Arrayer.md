# Arrayer

```go
list := []int{}           // skapar array med ints
list := make([]int, 5)    // skapar array med 5 tomma platser för ints
list := make([]int, 0, 5) // skapar array med 5 förallokerade platser

length := len(list)   // längd av arrayen

element := list[0]    // ta ut värden ur arrayen

sublist := list[2:5]  // tar en slice av arrayen 

list = append(list, 123)        // appenda värde till list
list = append(list, 1, 2, 3, 4) // appendar flera värden samtidigt
```
* vector.push_back() // C++
* [].append()        // Python
* list.add()         // Java
