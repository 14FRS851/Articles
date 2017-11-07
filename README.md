# Articles
Some articles written as MD files for reminder use

# Projects and tools from 14FRS851

![14FRS851](/Me/14FRS851.jpg?raw=true)

------------------------------------------------------------------------------------------

* [My first project](/Project1)
* [My second project](/Project2)

![Alt text](https://g.gravizo.com/svg?
@startuml;

actor User;
participant "First Class" as A;
participant "Second Class" as B;
participant "Last Class" as C;

User -> A: DoWork;
activate A;

A -> B: Create Request;
activate B;

B -> C: DoWork;
activate C;

C --> B: WorkDone;
destroy C;

B --> A: Request Created;
deactivate B;

A --> User: Done;
deactivate A;

@enduml)
