# Punkter att ta upp

* typsystem
* semantik/mönster
* parallelism
* modulsystem

# Kåhre

* egendefinierade typer

type Halsning struct {
    sprak string
    meddelande string
}

func (h *Halsning) Perform() {
    fmt.Println(h.meddelande)
}

type Id int

func (i *Id) print() {}

* arrayer

list := make([]int)
list := make([]int, 5)
list := make([]int, 0, 5)

vector.push_back
[].append
list.add

list = append(list, 123)
list = append(list, 123, 123, 123, 132)

for i := range x {} (arrays, string, maps)
sublist := list[2:5]
(gäller även strängar)

* map
table := make(map[string]int)

* first order functions
