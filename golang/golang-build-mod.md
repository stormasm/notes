

#### Golang Environment Variables

[From Here](https://golang.org/cmd/go/#hdr-Environment_variables)

GOBIN
	The directory where 'go install' will install a command.

#### For repos that have go.mod

The model is https://github.com/gohugoio/hugo#fetch-from-github

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
