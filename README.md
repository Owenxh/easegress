# EaseGateway [![Build Status](https://travis-ci.com/hexdecteam/easegateway.svg?token=bgrenfvQpzZ8JoKbi6uX&branch=master)](https://travis-ci.com/hexdecteam/easegateway) [![codecov](https://codecov.io/gh/hexdecteam/easegateway/branch/master/graph/badge.svg?token=HAR3ZmYoQG)](https://codecov.io/gh/hexdecteam/easegateway)

# Introduction

`EaseGateway` is a generic gateway system, support standalone and cluster both running modes.
For more design details, please see [easegateway design](./doc/easegateway_design.md)

# Build
```shell
make vendor_clean
make vendor_get
make clean
make build
```

# Run
```shell
make run
```

# Security
You can use [generate_cert.go](https://golang.org/src/crypto/tls/generate_cert.go) to generate certificate files.

```shell
    go run generate_cert.go -ca -host localhost,127.0.0.1 -start-date 'Jan 1 15:04:05 2016' -duration 87600h
```
