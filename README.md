# reimagined-design-patterns

Give a summary description of Four design patterns that you choose from the following design patterns: **Adapter,  Builder, Composite, Decorator, Observer, Interpreter, State, Mediator, Memento, Prototype, Proxy**. In your summaries say:

- what kind of problem(s) you can solve with that pattern and when you use it, maybe with a short example
- how the pattern works, what the basic idea of the pattern is
- what the main advantage and what the the main disadvantage is of using this pattern
- Write a short summary for each of the four patterns, about half a page for each pattern (rather less than more). 

> Do not add diagrams, and do not try to give a complete description of the patterns as found in the books. Rather think of how you would explain the essential ideas of these patterns in a few sentences to a colleague while drinking coffee.

**ADAPTER**
Adapter design pattern is one of the structural design pattern and its used so that two unrelated interfaces can work together. The object, that joins these unrelated interfaces, is called an Adapter.

Example: Using a camera memory card in a laptop. We cannot use it directly simply because there is no port in laptop which accept it. We must use a compatible card reader. We put the memory card into the card reader and then inject the card reader into the laptop. This card reader can be called the adapter.

Advantages :

    Reusability of existing interfaces
    Adaptability as per client need. Adaptor class can be modified without modifying existing code

Drawbacks :

    Increase in code size and complexity
    Many adaptions in Adaptor class might required to meet requirement

**State**
The state pattern is a behavioral design pattern.A state allows an object to alter its behavior when its internal state changes. The object will appear to change its class.

Real life example:
TV box operated with remote controller. We can change the state of TV by pressing buttons on remote. But the state of TV will change or not, it depends on the current state of the TV. If TV is ON, we can switch it OFF, mute or change aspects and source. But if TV is OFF, nothing will happen when we press remote buttons.

Advantages :

    We can easily add new states and new behaviors in the application without impacting other components.

Drawbacks :

    The state pattern is also known as objects for states. So, more states need more codes, and the obvious side effect is difficult maintenance. 
    
**Mediator**
Mediator pattern defines an object that encapsulates how a set of objects interact. Mediator promotes loose coupling by keeping objects from referring to each other explicitly, and it lets vary their interaction independently.

Real word example:
Traffic control room at airports. If all flights will have to interact with each other for finding which flight is going to land next, it will create a big mess.
Rather flights only send their status to the tower. These towers in turn send the signals to conform which airplane can take-off or land. We must note that these towers do not control the whole flight. They only enforce constraints in the terminal areas.

Advantages :

    1.Using mediator pattern, we can reduce the complexity of communication between objects in a system.
    2.Mediator helps in replacing “many-to-many” relationship with “one-to-many” relationships, so it is much easier to read and understand.

Drawbacks :

    1.The mediator object’s architecture may become complex if we put too much logic inside it.
    
**Memento**
Memento design pattern is behavioral pattern and is used to restore state of an object to a previous state. It is also known as snapshot pattern.
The intent of memento pattern is to capture the internal state of an object without violating encapsulation and thus providing a mean for restoring the object into initial state when needed.

Real life example:
1.In calculator applications, we can revisit all the calculations in memory with simple button press.
2.In code editors, we can revert or apply any code change with simple commands to undo and redo.

Advantages :

    1.The biggest advantage is that you can always discard the unwanted changes and restore it to an intended or stable state.
    2.Provides an easy recovery technique

Drawbacks :

    1.A high number of mementos require more storage. At the same time, they put additional burdens on a caretaker.
    2.The additional time to save the states decreases the overall performance of the system.


