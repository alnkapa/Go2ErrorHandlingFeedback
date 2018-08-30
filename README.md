Why do I need a handle?
```func printSum(a, b string) error {
  handle err { return err }
  x := check strconv.Atoi(a)
  y := check strconv.Atoi(b)
  fmt.Println("result:", x + y)
  return nil
  }```  

simplify used function check for last value:
```func printSum(a, b string) error {
  check err { return err }
  x := check strconv.Atoi(a)
  y := check strconv.Atoi(b)
  fmt.Println("result:", x + y)
  return nil
  }```
or like this:
```func printTest(a string) error {
  errorCheck err { return err }
  rune, multibyte, tail := errorCheck strconv.UnquoteChar(a)
  fmt.Println("result:", rune, multibyte, tail)
  return nil
  }```
