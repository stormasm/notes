
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
