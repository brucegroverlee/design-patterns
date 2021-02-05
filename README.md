# Design Patterns and SOLID with Deno

## Gamma Categorization
Design Patterns are typically split into three categories.

This is called Gamma Categorization after Erich Gamma, one of GoF authors.

### 1. Creational Patterns
Deal with the creation (contruction) of objects.

Explicit (constructor) vs. implicit (DI, reflection, etc).

Wholesale (single statement) vs. piecewise (step-by-step)

### 2. Structural Patterns
Concerned with the structure (Ex: class members)

Many patterns are wrappers that mimic the underlying class' interface

Stress the importance of good API design.

### 3. Behavioral Patterns
They are all different. No central theme.

## List

### 1. Builder
Separate component for when object construction gets too complicated.

Can create mutually cooperating sub-builders.

Often has a fluent interface.

### 2. Factories
Factory method more expressive than constructor.

A separate class with factory methods is a Factory.

Class hierarchies can have corresponding hierarchies of factories (Abstract Factory).

### 3. Prototype
Creation of object from an existing object.

Requires either explicit deep copy or copy through serialization.

Additional work required to preserve type.

### 4. Singleton
When you need to ensure just s single instance exists.

Can return same object from contructor on every call.

Direct dependence on a Singleton is dangerous.

### 5. Adapter
Converts the interface you get to the interface you need.

### 6. Bridge
Decouple abstraction from implementation.

### 7. Composite
Allows clients to treat individual objects and compositions of objects uniformly.

### 8. Decorator
Attach additional responsabilities to objects without modifying those objects or inheriting from them.

Decorators are composable with each other.

### 9. Facade
Provide a single unified interface over a set of systems/interfaces.

### 10. Flyweight
Memory saving technique.

Efficiently support very large numbers of similar objects.

### 11. Proxy
Provide a surrogate object that forwards calls to the real object while performing additional functions.

E.g. access control, communication, logging, etc.

### 12. Chain of Responsability
Allow components to process information/events in a chain.

Each element in the chain refers to next element or ...

Make a list and go through it.

### 13. Command
Encapsulate a request into a separate object.

Good for audit, replay, undo/redo.

Part of CQS/CQRS.

### 14. Interpreter
Transform textual input into object-oriented structures.

Used by interpreters, compilers, static analysis tools, etc.
Compiler Theory is a separate branch of Computer Science.

### 15. Iterator
Provides an interface for accessing elements of an aggregate object.

Objects can be made iterable (for loop).

### 16. Mediator
Provides mediation serives between two objects.

E.g. message passing, chat room.

### 17. Memento
Yields tokens representing system states.

Tokens do not allow direct manipulation, but can be used in appropiate APIs.

### 18. Observer
Allow notifications of changes/happenings in a component.

### 19. State
We model systems by having one of a possible states and transitions between these states.

Such a system is called a state machine.

Special frameworks exists to orchestrate state machines.

### 20. Strategy and Template Method
Both define a skeleton algorithm with details filled in by implementor.

Strategy uses ordinary composition, template method uses inheritance.

### 21. Visitor
Allow non-intrusive addition of functionality to hierarchies.

