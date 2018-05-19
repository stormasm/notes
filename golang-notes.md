# golang-notes

### How to build etcd

```
### XX=62
cd /
mkdir -p /tmpXX/go
cd /tmpXX
gopath
```

Where gopath is defined to be:

```
alias gopath='export GOPATH=${PWD}/go'
```
Then follow the notes
[here]
(https://github.com/coreos/etcd/blob/master/Documentation/dl_build.md#build-the-latest-version)

```
echo $GOPATH
go env
mkdir -p $GOPATH/src/github.com/coreos
cd $GOPATH/src/github.com/coreos
git clone github.com:coreos/etcd.git
cd etcd
./build
./bin/etcd
```
