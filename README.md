# Go Programming Language
![alt text](http://www.unixstickers.com/image/cache/data/stickers/golang/golang.sh-600x600.png "Golang Mascot")


## Intro to Golang
- “Go is an open source programming language that makes it easy to build simple, reliable, and efficient software.”
- Functional language
- Speed
- Really good for stand alone command line scripts (No interpreter needed unlike PHP)
- Very simular to C
---

## Differences
- Not Object Oriented
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
- [Beego](http://beego.me/ target="_blank")
- [Macaron](https://go-macaron.com/ target="_blank")
- [Web.io](http://webgo.io/ target="_blank")
---

### Back end APIs
- [Gorilla](http://www.gorillatoolkit.org/ target="_blank")
