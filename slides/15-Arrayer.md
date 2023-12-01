# Arrayer

```go
list := make([]int) // skapar lista med ints
list := make([]int, 5) // skapar lista med 5 tomma platser för ints
list := make([]int, 0, 5) // skapar lista med 5 förallokerade platser

list = append(list, 123) // appenda värde till list
list = append(list, 123, 123, 123, 132) // appendar flera värden samtidigt

sublist := list[2:5] // tar en slice av listan 

length := len(sublist) // längd av listan

element := list[0] //ta ut värden ur listan

```
* vector.push_back() // C++
* [].append()  // Python
* list.add()  // Java