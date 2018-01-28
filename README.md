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
* `go get github.com/jpochyla/trezord-go`
* install docker
* `docker pull karalabe/xgo-latest`
* `go get github.com/karalabe/xgo`

Then:
* `cd ~/go/src/github.com/jpochyla/trezord-go`
* `xgo -ldflags '-w -s' --targets=windows/amd64,windows/386,darwin/amd64,linux/amd64,linux/386`
 or any subset of the targets
  * `-ldflags '-w -s'` is for omitting symbol table, which makes the binary smaller. In case of problems remove it `
