# Go Programming Language
![alt text](http://www.unixstickers.com/image/cache/data/stickers/golang/golang.sh-600x600.png "Golang Mascot")


## Intro to Golang
- “Go is an open source programming language that makes it easy to build simple, reliable, and efficient software.”
- Functional language
- Speed
- Really good for stand alone command line scripts
- Very simular to C


```js

package main

import "fmt"

func main() {
    fmt.Println("Hello World")
}
```

---

## Differences
- Not Object Oriented
- More scalable
- Concurrency: Progress on more than one task at the same time. (Goroutines)

```js

package main

import "fmt"

func f(n int) {
  for i := 0; i < 10; i++ {
    fmt.Println(n, ":", i)
  }
}

func main() {
  go f(0)
  var input string
  fmt.Scanln(&input)
}
```

---

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
---

## Sample Back end
```js
m.Group("/books", func() {
    m.Get("/:id", GetBooks)
    m.Post("/new", NewBook)
    m.Put("/update/:id", UpdateBook)
    m.Delete("/delete/:id", DeleteBook)

    m.Group("/chapters", func() {
        m.Get("/:id", GetBooks)
        m.Post("/new", NewBook)
        m.Put("/update/:id", UpdateBook)
        m.Delete("/delete/:id", DeleteBook)
    }, MyMiddleware3, MyMiddleware4)
}, MyMiddleware1, MyMiddleware2)
```
---

### Front end APIs
- [Beego](http://beego.me/)
- [Macaron](https://go-macaron.com/)
- [Web.io](http://webgo.io/)
- [Gorilla](http://www.gorillatoolkit.org/)

---
---
- [Go Programming Tutorial](http://www.newthinktank.com/2015/02/go-programming-tutorial/)
- [Golang-book.com](https://www.golang-book.com)
