
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
