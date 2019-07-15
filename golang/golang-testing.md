
##### How to turn off the test cache

https://github.com/openshift/machine-config-operator/pull/873

The new way to disable the go testing cache is to use -count=1 in the go test command.

https://github.com/golang/go/issues/24573

For the top level Makefile for the flux project

```
export GO_TEST=env GO111MODULE=on go test -count=1 $(GO_ARGS)
```

#### Benchmark Testing

[count_test.go](https://github.com/influxdata/flux/blob/master/stdlib/universe/count_test.go)

```
gtvr BenchmarkCount -bench=BenchmarkCount
```
