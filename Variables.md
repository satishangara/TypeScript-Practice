					VARIABLES

Variable is a container - which can hold/store some data.
Keywords: 3 types.
Var
Let
Const
Syntax:
Keyword VariableName :data type=value
Ex:	 var age :number=30
TS specifying the datatype is optional.
Ex: 	var age=30
—-------------------
var age=30;
Console.log(age);
—--------------------
Var 	(vs)	let	(vs)	Const

Scope of the variable.
Declaration/ value assignment.
Re-Declaration
Re-Initilization/Re-assignment
Hoisting
Info:
Var keyword is never recommended to use in TS and JS.
Let keywords be used when you need a variable that can change.
Const keyword used when the variable value should not change.

Scope of the variable
Accessible area/ Scope:
Functional scope (var)
Block scope (let & block)
Function scope: - create any variable in the function is called function scope.
function test()
{
}
Block scope: - Create any variables in the block of if / for or other looping blocks.
if(condition)
{
}
 Info: Var is a functional scope and let & const comes under block scope.
Example1: var (Functional scope)



Example2: Let & Const (Block scope)


Example3: Combinations of scope differences.



Declarations and Initializations of variables

Var and let key words are able to declare without initialization.


Const keyword must be initialized at the time of declaration, without initialization can't declare variables.








Re-Declarations

Var- allows redeclaration.
Let & Const - not allowed the re-declaration. (making code safer)

Redeclaration :  whatever variable declared once, again reused the same variable with different value is redeclaration.

Var - allows re-declaration


Let - not allow re-declaration:



Const - not allowed re-declaration



Re-Initilization / Re-assignment

Var & Let - re-assignment allowed.
Const - re-assignment not allowed. (only constants allowed - cannot change the value)

Var - allows 






Let - allows



Const - Not allowed 



Hoisting
Var is hoisted with ‘Undefined’
Let & Const are hoisted with ‘Not initialized’.

Try to execute a variable, before declaring.







Var - Undefined hoisting


Let - not initializing hoisting

Const - not initializing hoisting
 
-----------------------------------------------------------------------------------------------------------
//Example1: Functional scope (Var variable)

/* function varscope()
{
    if(true)
    {
        var message="hello satish-var";
       // console.log(message);
    }
    console.log(message);
}
varscope(); */

//Example2: Block Scope (Let & Const variables)
/*function blockScope()
{
    if(true)
    {
        let text="let test message";
        const num="test const";

       // console.log(text);
        // console.log(num);
    }
    console.log(text);
    console.log(num);
}
blockScope()*/

//Example 3: Scope differences

/* function scopedifferene()
{
    if(true)
    {
        var num1=10;
        let num2=20;
        const num3=30;

        //console.log(num1);
        //console.log(num2);
       //console.log(num3);
    }
    console.log(num1);
    console.log(num2);
    console.log(num3);
}
scopedifferene() */




