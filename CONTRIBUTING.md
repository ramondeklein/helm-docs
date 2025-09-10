# Contributing to helm-docs

## Build
To build from source in this repository:

```bash
cd cmd/helm-docs
go build
```

Or you can install from source:

```bash
GO111MODULE=on go get github.com/ramondeklein/helm-docs/cmd/helm-docs
```

## Testing

### Benchmarks

If you are working on a feature that is likely to impact performance, consider running benchmarks
and comparing the results before and after your change.

To run benchmarks, run the command:

```
go test -run=^$ -bench=. ./cmd/helm-docs
```

### Github Actions
You may use [act](https://github.com/nektos/act) to test

locally the workflow.By issuing the following command you can
see if a release will work as expected.
```bash
act -j release
```
