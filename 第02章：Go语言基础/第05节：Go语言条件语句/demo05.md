```go
func main() {
	var x interface{}
	switch i := x.(type) {
	case nil:
		fmt.Printf("x的类型为: %T", i)
	case int:
		fmt.Printf("x的类型是 int 类型")
	case float64:
		fmt.Printf("x的类型是 float 64 ")
	case func(int) float64:
		fmt.Printf("x 的类型是 func(int)")
	case bool, string:
		fmt.Printf("x的类型是 bool 或者string")
	default:
		fmt.Printf("未知型")
	}
}
```