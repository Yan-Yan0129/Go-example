```go
package main

//Address 地址结构体
type Address struct {
	Province string
	City     string
}

//User 用户结构体
type User struct {
	Name    string
	Gender  string
	Address Address
}

func main() {
	user1 := User{
		Name:   "GIao哥",
		Gender: "男",
		Address: Address{
			Province: "河北",
			City:     "秦皇岛",
		},
	}
	fmt.Printf("user1=%#v\n", user1)//user1=main.User{Name:"Giao哥", Gender:"男", Address:main.Address{Province:"河北", City:"秦皇岛"}}
}
```