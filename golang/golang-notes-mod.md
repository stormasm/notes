
Last updated Oct 24, 2019

If go.mod is already in the repo...

```
git clone git@github.com:expectedsh/go-sonic.git
cd go-sonic
go build ./...
go test ./...
go run cmd/example/main.go
```

#### Golang Environment Variables

[From Here](https://golang.org/cmd/go/#hdr-Environment_variables)

GOBIN
	The directory where 'go install' will install a command.

#### For repos that have go.mod

The model is https://github.com/gohugoio/hugo#fetch-from-github

Another model is https://github.com/pelletier/go-toml#tools

If you have go.mod in your repo then you can just do this...

```
go install github.com/pelletier/go-toml/cmd/tomljson
```

And if GOBIN is not set the binaries will end up here...

~/go/bin

Example for https://github.com/asdine/storm

```
cd /tmpXXX
gopclean
gopc
mkdir src
cd src
gc git@github.com:asdine/storm.git
cd storm
go install
go test -v
```

References (in helpfulness order)

[Medium](https://medium.com/@fonseka.live/getting-started-with-go-modules-b3dac652066d)

[Stackoverflow](https://stackoverflow.com/questions/24069664/what-does-go-install-do)
