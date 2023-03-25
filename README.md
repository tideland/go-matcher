# Tideland Go Matcher

[![GitHub release](https://img.shields.io/github/release/tideland/go-matcher.svg)](https://github.com/tideland/go-matcher)
[![GitHub license](https://img.shields.io/badge/license-New%20BSD-blue.svg)](https://raw.githubusercontent.com/tideland/go-matcher/master/LICENSE)
[![Go Module](https://img.shields.io/github/go-mod/go-version/tideland/go-matcher)](https://github.com/tideland/go-matcher/blob/master/go.mod)
[![GoDoc](https://godoc.org/tideland.dev/go/matcher?status.svg)](https://pkg.go.dev/mod/tideland.dev/go/matcher?tab=packages)
[![Workflow](https://img.shields.io/github/workflow/status/tideland/go-matcher/Go)](https://github.com/tideland/go-matcher/actions/)
[![Go Report Card](https://goreportcard.com/badge/github.com/tideland/go-matcher)](https://goreportcard.com/report/tideland.dev/go/matcher)

## Description

The **Tideland Go Matcher** provides a simple pattern matching. It matches
the following pattterns:

- ? matches one char
- * matches a group of chars
- [abc] matches any of the chars inside the brackets
- [a-z] matches any of the chars of the range
- [^abc] matches any but the chars inside the brackets
- \ escapes any of the pattern chars

## Examples

```go
if matcher.Matches("g*e g?", "Google Go", matcher.IgnoreCase) { ... }

if matcher.Matches("[oO][kK]", "ok", matcher.ValidateCase) { .... }
```

## Contributors

- Frank Mueller (https://github.com/themue / https://github.com/tideland / https://themue.dev)
