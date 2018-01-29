trezord-go
===

```
go build
./trezord-go -h
```

Quick guide to cross-compiling
----
Prerequisities:

* install go
* install docker
* `docker pull karalabe/xgo-latest` 
* `go get github.com/karalabe/xgo`

Then:
* `xgo --targets=windows/amd64,windows/386,darwin/amd64,linux/amd64,linux/386 github.com/trezor/trezord-go`
 or any subset of the targets
  * if you want to build locally (e.g. with changes), do `go get github.com/trezor/trezord-go` and `xgo --targets=windows/amd64 .` in the directory instead
