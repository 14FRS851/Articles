# Articles
Some articles written as MD files for reminder use

# Projects and tools from 14FRS851

![14FRS851](/Me/14FRS851.jpg?raw=true)

------------------------------------------------------------------------------------------

* [My first project](/Project1)
* [My second project](/Project2)

# test gravizo

![Alt text](https://g.gravizo.com/svg?
  digraph G {
    aize ="4,4";
    main [shape=box];
    main -> parse [weight=8];
    parse -> execute;
    main -> init [style=dotted];
    main -> cleanup;
    execute -> { make_string; printf}
    init -> make_string;
    edge [color=red];
    main -> printf [style=bold,label="100 times"];
    make_string [label="make a string"];
    node [shape=box,style=filled,color=".7 .3 1.0"];
    execute -> compare;
  }
)

![Alt text](https://g.gravizo.com/svg?
 @startuml;

[*] --> State1;
State1 --> [*];
State1 : this is a string;
State1 : this is another string;

State1 -> State2;
State2 --> [*];

@enduml
)

