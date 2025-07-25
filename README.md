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

4. sweet suite is an integration test of sorts and tests various layers of Go along with the GC 

git clone https://go.googlesource.com/benchmarks
Inorder to run sweet on powerpc, patch the file to exclude cockroachdb 

cp exclude-cockroachdb.patch benchmarks/sweet # required only for powerpc
cd benchmarks/sweet 
patch -p1<exclude-cockroachdb.patch # required only for powerpc 
Follow the instructions in benchmarks/sweet/README.md

