# nolint analyzer issue

This command should not raise any issue:

```console
$ go run main.go ./test
test/foo.go:6:7: unchecked error
exit status 3
$ sed -n 6p test/foo.go
        pouet() //nolint:errcheck
```
