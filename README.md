# gcbench
GC benchmarks collection pulled from older Go GC benchmarks and recent ones

1. bintree/
To use this benchmark simply run 

go build bintree.go 

./bintree 

2. garbage/ 

requires golang.org/x/benchmarks as indicated by go.mod file 

you might have to run go mod tidy -e 

go build garbage.go nethttp.go 

./garbage

3. oldbench/

Simply running make will build the binaries

and they can be run one by one by

./peano 

./parser

./tree 

./tree2


