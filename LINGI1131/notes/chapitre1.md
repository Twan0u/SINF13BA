## 1. Declarative Model and Kernel language
### 1.1  Kernel language VS practical language
The **practical language** is an easy way to code. It provides usefull abstractions for the programmer and it can be extended with linguistic abstractions (and syntaxic sugar). The *practical language* can always be translated into **kernel Language**. 

**Kernel Language** is a minimal set of intuitive concepts that are easy for the programmer to understand and that has a formal semantic (not always easy to work with).


This exemple in practical language :
```
fun {Sqr X} X*X end
B={Sqr {Sqr A}}
```
can be translated into this in Kernel language
```
proc {Sqr X Y}
  {'*' X X Y}
end

Local T in
  {Sqr A T}
  {Sqr T B}
end
```
### 1.2 Single assignement
A variable in the single assignement store is unbound or a value. if it's a value, this value can only be bound one time

### 1.3 Kernel language

<Statement>	 ::= 	<Statement1> <Statement2>  
	 | 	X = f(l1:Y1 ... ln:Yn)  
	 | 	X = <number>  
	 | 	X = <atom>  
	 | 	X = <boolean>  
	 | 	{NewName X}  
	 | 	X = Y  
	 | 	local X1 ... Xn in S1 end  
	 | 	proc {X Y1 ... Yn} S1 end  
	 | 	{X Y1 ... Yn}  
	 | 	{NewCell Y X}  
	 | 	Y=@X  
	 | 	X:=Y  
	 | 	{Exchange X Y Z}  
	 | 	if B then S1 else S2 end  
	 | 	thread S1 end  
	 | 	try S1 catch X then S2 end  
	 | 	raise X end  

### 1.4 Partial values
   ex:
```
declare A B C L in
   L=[ABC]
   {Browse L} //display [_ _ _]
```   
### 1.5 Dataflow principle
   **Concept of dataflow** : the availibility drives the execution

   ```
   declare
   Y=X+1 // X is unbound and the program will wait for X  
   ```

If we wait, someone else need to bound this variable. so we introduce the concept of thread (State of the execution). They can be multiple threads inside the program. The execution continue when the data becomes available

