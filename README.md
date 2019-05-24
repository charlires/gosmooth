# Smooth Streaming parser library

[![Reference](https://godoc.org/github.com/davimdo/gosmooth?status.svg)](https://godoc.org/github.com/davimdo/gosmooth)

Godash is a go module to parse ISM files that corresponds to the Microsoft 
Smooth Streaming protocol

## Example

```go
ssm, err := gosmooth.Unmarshal(ism)
if err != nil {
    t.Fatal(err)
}
fmt.Println(ssm)

b, err := ssm.Marshal()
if err != nil {
    t.Fatal(err)
}
fmt.Println(string(b))
```