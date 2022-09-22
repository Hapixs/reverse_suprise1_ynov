# Fonction Suprise(a []int) int


```go
package main

import "fmt"

func Surprise(a []int) int { 
	if len(a) < 1 {
		return 0
	}
	if len(a) == 1 {
		return a[0]
	} else {
		return a[0] + Surprise(a[1:])
	}
}

func main() {
	fmt.Println(Surprise([]int{4,3,4,5,10,10,16,4,6}))
}
```


>Cette fonction à pour but d'ajouter tout les nombre d'un tableau ensemble d'une façon récursive et de retourner le réultat

* ### **Example 1**
    ```go
    Surprise([]int{1, 2, 3, 10, 4, 10})
    ```
    Opérations
    ```
    1+2+3+10+4+10
    ```
    Résultat = ```30```<br> 
    <br
* ### Example 2
    ```go
    Surprise([]int{45, 2000, 2+8, 20, 0, 1})
    ```
    Opérations
    ```
    45+2000+10+20+0+1
    ```
    Résultat = ```2076```<br>
    <br>

* ### **Example 3**
    ```go
    Surprise([]int(nil))
    ```
    Opérations
    ```
    (rien)
    ```
    Résultat = ```0```

* ### **Example 4**
    ```go
    Surprise([]int{53})
    ```
    Opérations
    ```
    53+0
    ```
    Résultat = ```53```

<br><br><br><br><br><br><br><br><br>

![alt text](https://c.tenor.com/6RQruxVwKZgAAAAC/rainbow-reverse.gif)![alt text](https://c.tenor.com/6RQruxVwKZgAAAAC/rainbow-reverse.gif)![alt text](https://c.tenor.com/6RQruxVwKZgAAAAC/rainbow-reverse.gif)