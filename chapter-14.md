# CHAPTER 14: Theory of Computation

The mathematical study of what can be computed.

## 1. Finite Automata and Regular Expressions
- **Deterministic Finite Automaton (DFA)**: A state machine that accepts or rejects strings of symbols. Has finite memory.
- **Regular Expressions**: A notation for defining regular languages (patterns). Equivalent to Finite Automata. Used in text searching and lexical analysis.

## 2. Turing Machines and Computability
- **Turing Machine**: An abstract mathematical model of a general-purpose computer. It has an infinite tape and a read/write head.
- **Church-Turing Thesis**: Anything that can be effectively computed can be computed by a Turing machine.

## 3. The Halting Problem
- **Problem**: Can we write a program that determines if any given program will eventually stop (halt) or run forever?
- **Answer**: Alan Turing proved it is undecidable. There is no algorithm that can solve the Halting Problem for all possible input programs. This defines the limits of computation.

## 4. Complexity Classes (P vs. NP)
- **P (Polynomial time)**: Problems solvable quickly (efficiently).
- **NP (Nondeterministic Polynomial time)**: Problems for which a solution can be verified quickly.
- **P vs NP Question**: Is P = NP? (Can every problem whose solution can be quickly verified also be solved quickly?). It is one of the greatest unsolved problems in mathematics. Most believe P != NP.
