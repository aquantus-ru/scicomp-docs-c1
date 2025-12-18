# CHAPTER 4: Programming Paradigms

A programming paradigm is a style or way of programming. Different problems require different approaches.

## 1. Procedural vs. Functional Programming
- **Procedural (Imperative)**: Based on procedure calls. The program is a sequence of steps altering the state of the machine. Focus is on "how" to do tasks. (e.g., C, Pascal).
- **Functional (Declarative)**: Treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data. Focus is on "what" to solve. (e.g., Haskell, Lisp).
  - Key concepts: Higher-order functions, Immutability, Recursion over loops.

## 2. Object-Oriented Principles (Encapsulation, Inheritance)
**OOP** models software around "objects" combining data and methods.
- **Encapsulation**: Bundling data and methods that operate on that data within a single unit (class) and restricting access to some of the object's components (private/public). This hides internal complexity.
- **Inheritance**: A mechanism where a new class derives properties and behavior from an existing class. Promotes code reuse.
- **Polymorphism**: The ability of different classes to be treated as instances of the same general class (e.g., method overriding).

## 3. State Management and Side Effects
- **State**: The stored information to which a program has access at a given time.
- **Side Effect**: When a function or expression modifies some state outside its local environment (e.g., changing a global variable, writing to a file).
- **Management**: Functional programming aims to minimize side effects ("Pure functions") to make code more predictable and testable. In complex UI applications, state management patterns (like Redux) centralize state to ensure consistency.

## 4. Declarative vs. Imperative Logic
- **Imperative**: Describes the control flow. "Go to the kitchen, open the fridge, take out milk."
- **Declarative**: Describes the desired logic without control flow. "I want milk." (e.g., SQL, HTML).
Declarative code is often more concise and easier to reason about, as the implementation details are abstracted away.
