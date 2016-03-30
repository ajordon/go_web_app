# go_web_app
go_web_app

## Intro to Golang
- “Go is an open source programming language that makes it easy to build simple, reliable, and efficient software.”
- Functional language
- Speed
- Really good for stand alone command line scripts (No interpreter needed unlike PHP)
- Very simular to C

## Sample Font end
```js

package main

import "net/http"

func main() {
    http.HandleFunc("/", someFunc)
    http.ListenAndServe(":8080", nil)
}

func someFunc(w http.ResponseWriter, req *http.Request) {
    w.Write([]byte("Hello universe"))
}
```

