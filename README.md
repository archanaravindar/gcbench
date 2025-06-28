# gcbench
GC benchmarks collection pulled from older Go GC benchmarks and recent ones

bintree/
To use this benchmark simply run 
go build bintree.go 
./bintree 

garbage/ 
requires golang.org/x/benchmarks as indicated by go.mod file 
you might have to run go mod tidy -e 
go build garbage.go nethttp.go 
./garbage

oldbench/
Simply running make will build the binaries
and they can be run one by one by
./peano 
./parser
./tree 
./tree2
