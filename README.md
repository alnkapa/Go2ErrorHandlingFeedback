```
func printSum(a, b string) error {
check1 := func (x int, err error) { // function with any name
  fmt.Println("result err:",err)
  return x 
}
x := check1 strconv.Atoi(a) // on err != nil return from function "printSum"
y := check1(strconv.Atoi(b)) // on err != nil continue execute function "printSum"
fmt.Println("result:", x + y)
return nil
}
```

