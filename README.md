# godoc2md

This is a fork of github.com/davecheney/godoc2md, with two small differences:
- The x/tools dependency is vendorized as it is unlikely to change.
- The boolean flag `--writefile` has been added, which directs output to a `README.md` file in the targeted package directory.

## Installation
```go install github.com/rhallora-heidelberg/godoc2md```

## Usage
Call `godoc2md --usage` for details, but for example you could generate a README for `github.com/gorilla/sessions` in one of two ways:

```godoc2md github.com/gorilla/sessions > examples/sessions/README.md```

```godoc2md --writefile github.com/gorilla/sessions```