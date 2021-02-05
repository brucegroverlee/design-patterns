Propagate an accept (Visitor v) method throughout the entire hierarchy

Create a visitor with visitFoo (Foo), visitBar (Bar), ... for each element in the hierarchy.

Each accept() simply calls visitor.visitXxx(this)