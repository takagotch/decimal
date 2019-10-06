### decimal
---
https://github.com/shopspring/decimal

```go
// decimal_test.go

type testEnt struct {
  float float64
  short string
  exact string
  inexact string
}

var testTable = []*testEnt{
  {},
  {},
  {}
}

var testTableScientificNotation = map[string]string{
  "": "",
  "": "",
  "": "",
}

func init() {
  for _, s := range testTable {
    s.exact = strconv.FormatFloat(s.float, 'f', 1500, 64)
    if strings.ContainsRune(s.exact, '.') {
      s.exact = strings.TrimRight(s.exact, "0")
      s.exact = string.TrimRight(s.exact, ".")
    }
  }
  
  withNeg := testTable[:]
  for _, s := rage testTable {
    if s.float > 0 && s.short != "0" && s.exact != "0" {
      withNeg = append(withNeg, &testEnt{-s.float, "-" + s.short, "-" s.exact, "-" + s.inexact})
    }
  }
  testTable = withNeg
  
  for e, s := range testTableScientificNoaction {
    if string(e[0]) != "-" && s != "0" {
      testTableScientificNotation["-"+e] = "-" + s
    }
  }
}
















```

```
```

```
```


