1st go program
--
package main

import "fmt"

func main() {
	fmt.Print("Hello Pavan")
}

```
1) In any programming language to run the program the language will find entrypiont of it
where entire program will start executing. Ex: in java PSVM in Go also same it uses
func main(){
}

2) To get or find print statement we have inform the program that print method is in
"fmt" package, import "fmt" -- it will provides methods to print the string.
we need to use fmt.Print("Hello Go")

3) Now we need to mention which main method, Like main maybe present in many places.
Main method make sure it should be in main package, Go will find main package and execute the
main method.
package main -- it will find entry point and execute it
```
To Run go lang program or code 
--
```
go run app.go
app.go -- is program name
```
VARIBLES
--
We define varibles using var keyword and bydefault the value of int and string is 
0 and "empty space" for string.

NOTE: If we have declared any variable and we are not using in program then
at the time of comilation it will raise an error. If we are not using then remove
it.

```
package main

import "fmt"

func main() {

	// 1st method
	var a int //declaration
	a = 77    // initalization

	// 2nd method
	var b int = 500 //declaration with initalization

	var c = 1000 // less verbose // declaration with initalization
	// based on righthand side it will decided the datatype of c leftside

	// 3rd method
	d := 1111 //declaration with initalization in easyway

	// fmt.Println("Hello Pavan")
	fmt.Println(a)
	fmt.Println(b)
	fmt.Println(c)
	fmt.Println(d)

}

```


