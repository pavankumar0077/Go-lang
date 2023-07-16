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
Varible Scope
--

```
package main

import "fmt"

//Global
Val2 := 100

//Package level -- (Camel Case)
var myVal := 150 

func main() {

	// Local 	-- It will be inside the function always 


	// Global	-- It will be present outside the function -- It must be Pascal Case that means Uppercase letter for 1st letter
	// Upto package level in the program, Like it will accessable under the main package only for this example
	// For any number of methods present under main package Global variable is accessable


	// Package_Level  --   It will start with Camel case 1st letter lower and rest upper Ex: myVal
	// This variable is accessable throught the program as well as other packages as well, In different package as
	// it is accessable

	
	// Local varible
	val1 := 55

	fmt.Println(val)

}
```
Shodowing.
--
```
package main

import "fmt"

//Shadowing -- It is nothing but if we have same variable in local inside the func and outside the func, Then
// It will use or print which is present inside the method variable only
// Becoz val1 is near which is in method and global is outside the fucn, The prority will be to be inside method
// variable only

var val1 int = 100

func main() {

	val1 := 55

	fmt.Println(val1)

}
```
NOTE: When we are using global variable then we must use var keyword  
var val1 int = 100 works
val1 := 100 will not works here

```
package main

import "fmt"

//Shadowing -- It is nothing but if we have same variable in local inside the func and outside the func, Then
// It will use or print which is present inside the method variable only
// Becoz val1 is near which is in method and global is outside the fucn, The prority will be to be inside method
// variable only

// NOTE: When we are using global variable then we must use var keyword  
// var val1 int = 100 works
// val1 := 100 will not works here

var val1 int = 100

func main() {

	val1 := 55

	fmt.Println(val1)

}

```


