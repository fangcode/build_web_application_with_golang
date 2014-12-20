#Go Web 編程筆記
---
#第二章

##2.1 START！

###1 print hello world

```
// just print hello world using golang

package main
import "fmt"

func main() {
	fmt.Printf("hello world!")
}

```

1. Go 語言程序是通過 package 來組織的。

2. package <pakname> 來說明當前文件屬於哪個包。如果包名是 main 的話則表示當前代碼是一個可獨立運行的包，編譯之後會產生可執行文件。

3. Go 語言使用 UTF-8 字符串和標識符。

---

##2.2 Go 語言基礎

### 1 定義變量

Go 語言中最基本的定義變量的方式是使用關鍵字 var 。

三種定義變量的方式：

- 利用關鍵字 var 。順序依次是關鍵字，變量名，類型，值。

```
var vname type value
//eg:
var myname string = "fang"
```

- 省略關鍵字 var。順序變成關鍵字，變量名，值。在這種定義方式中，Go 會根據初始化的值的類型推導出相應的類型。

```
var vname value
// eg:
var myname "fang"
```

- 利用符號 ‘:=’ 定義變量。順序爲變量名，‘:=’，值。在這種定義方式中，Go 會根據初始化的值的類型推導出相應的類型。但是這種方式只能用於函數內部，否則會導致編譯錯誤。

```
vname := value
// eg:
myname := "fang"
```

注：

1. _(下劃線)是一個特殊的變量名，所有賦給它的值都會被丟棄掉。
2. 聲明的變量沒有使用會導致編譯錯誤。


###2 常量

在 Go 語言中定義常量使用關鍵字 const。如有需要可以指定常量的類型。

```
const PI = 3.1415926
const myname = "fang"
```






