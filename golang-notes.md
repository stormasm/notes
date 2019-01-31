
#### Example Go builds

We will use
[istio](https://github.com/istio/istio) as an example
of how to build a Golang app that does not have go.mod
at the top level in its repository.

```
mkdir src
cd src
mkdir istio.io
cd istio.io
git clone https://github.com/istio/istio
make depend
make build
```

We will use
[hugo](https://github.com/gohugoio/hugo) as an example
of how to build a Golang app that does have it...

```
mkdir $HOME/src
cd $HOME/src
git clone https://github.com/gohugoio/hugo.git
cd hugo
go install
```

[Here are the instructions for Hugo](https://github.com/gohugoio/hugo#fetch-from-github)

#### Setup from Scratch

Assuming you do not have a go.mod in your repository  
At the top level of any repo type this command

```
go mod init github.com/stormasm/redishacker
```

#### Testing

```
go test -run TestBulkStringRequestSetString
```

#### Running

```
cd fetch
go run fetch.go
```

#### Building

```
go build -o myfetch ./fetch/.
```
