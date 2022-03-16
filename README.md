## staticcheck version

```
staticcheck -version
staticcheck 2021.1.2 (v0.2.2)
```

## go version

```
go version
go version go1.18 darwin/amd64
```

## Reproducible Steps

- `go install honnef.co/go/tools/cmd/staticcheck@v0.2.2`
- `staticcheck .`

## Expectation

I expect staticcheck to succeed.


## Actual behaviour

staticcheck fails with the following message:

```
-: cannot import "math/bits" (unknown iexport format version 2), export data is newer version - update tool (compile)
```