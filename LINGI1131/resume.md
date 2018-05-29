# Computer Language Concepts

## 1. Declarative Model and Kernel language

The **practical language** is an easy way to code. It provides usefull abstractions for the programmer and it can be extended with linguistic abstractions (and syntaxic sugar). 

**Kernel Language** is a minimal set of intuitive concepts that are easy for the programmer to understand and that has a formal semantic (not always easy to work with).

**Concept of dataflow** : the availibility drives the execution

```
declare 
Y=X+1 // X is unbound and the program will wait for X  
```

If we wait, someone else need to bound this variable. so we introduce the concept of thread (State of the execution). They can be multiple threads inside the program. The execution continue when the data becomes available