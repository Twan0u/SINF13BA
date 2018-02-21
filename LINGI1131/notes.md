# Computer Language Concepts
## S3
### Determinstic Dataflow
#### Single assignement variables
Single assignement : une variable can ba bound to only one value un memory
data structures can contains unbound variables :
#### Partial values
ex:
``` oz
declare A B C L in
L=[ABC]
{Browse L} //display [_ _ _]
```
### Dataflow principle
**Concept of dataflow** : the availibility drives the execution
```
declare
Y=X+1 // X is unbound and the program will wait for X  
```
if we wait, someone else need to bound this variable. so we introduce the concept of thread (State of the execution). They can be multiple threads inside the program. The execution continue when the data becomes available

#### Concurrency and thread
be carefull whith this because you create a *activity* inside the system (thread) each time you unbound a varaible
**Thread** : sequence in execution
thread < S > end : create a thread.
We can have multiple threads simultaniously(+- because only one cpu)
the execution uses 'interleaving semantics' : one cpu, multiple threads that are sharing this calculation power at the same time. interleaving : the system will perform only one sequence of steps in the execution. concurrency does not apply parallelism. so no need of multiple cores.
parallelism : small number (4-8 cores so 4-8 processes at the same time)
concurrency : hundreds at the same time

each step is the thread is choose by the scheduller (ordonnanceur).

### the execution tree
it shows all possibile exécutions (all possible ways in the execution)
```
declare A B C in
thread A=1 end
thread B=2 end
thread C=A+B end
```

#### stream
a non nil list is used to pass informatin trough the program

#### ping-pong
a thread need to display ping pong, in alternance with thread1 saying ping and the other pong. how should threads do this ?
threads should communicate
```
declare
fun {Ping S}
  case S of ok|T then
  {browse ping}
  ok|{Ping T}
  end
end
fun {Pong S}
  case S of ok|T then
  {browse Pong}
  ok|{Pong T}
  end
end
declare S1 S2 in
thread S2={Ping ok|S1} end //ok| is used to initialise the ping pong
thread S1={Pong S2} end
```
