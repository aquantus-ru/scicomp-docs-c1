# CHAPTER 1: Foundations of Computational Logic

This chapter establishes the bedrock of computer science: the mathematical and logical systems that allow us to represent information and perform computations.

## 1. Boolean Algebra and Logic Gates
**Boolean algebra** is the branch of algebra in which the values of the variables are the truth values **true** and **false**, usually denoted 1 and 0 respectively. It provides the framework for modeling the logical operations of digital circuits.

The fundamental operations are:
- **AND (Conjunction)**: Returns true only if both operands are true. Represented by a series circuit or the symbol `&`.
- **OR (Disjunction)**: Returns true if at least one operand is true. Represented by a parallel circuit or the symbol `|`.
- **NOT (Negation)**: Returns the inverse of the operand.

**Logic gates** are the physical implementation of these operations using transistors. Complex circuits, such as adders and multiplexers, are built by combining NAND, NOR, XOR, and XNOR gates. The universality of NAND and NOR gates means that any boolean function can be implemented using only one of these types of gates.

## 2. Truth Tables and Circuit Simplification
A **truth table** is a mathematical table used in logic to compute the functional values of logical expressions on each of their functional arguments. For a function with *n* variables, the table has 2^*n* rows, covering every possible combination of inputs.

Circuit simplification is crucial for optimizing performance and reducing power consumption. Techniques include:
- **Algebraic Manipulation**: Using laws like De Morgan's Laws (e.g., `NOT(A AND B) = NOT A OR NOT B`) to reduce expressions.
- **Karnaugh Maps (K-Maps)**: A visual method for simplifying boolean expressions without extensive algebraic calculations. K-maps utilize Gray code ordering to group adjacent cells containing 1s, identifying common terms that can be eliminated.

## 3. Binary, Hexadecimal, and Floating-point Representation
Computers operate on **binary data** (base-2).
- **Binary**: Uses digits 0 and 1. It is robust against noise in physical circuits.
- **Hexadecimal (base-16)**: Uses digits 0-9 and A-F. It is used as a human-friendly shorthand for binary, as one hex digit represents exactly four binary bits (a nibble).

**Floating-point representation** (IEEE 754 standard) allows computers to approximate real numbers. It divides a number into three parts:
- **Sign bit**: 0 for positive, 1 for negative.
- **Exponent**: Encodes the magnitude.
- **Mantissa (Significand)**: Encodes the precision.
This format involves a trade-off between range and precision and can lead to rounding errors in calculation.

## 4. Information Theory and Entropy
Claude Shannon's **Information Theory** quantifies the storage and transmission of information.
- **Bit**: The fundamental unit of information.
- **Entropy**: A measure of the uncertainty or "surprise" associated with a random variable. High entropy implies high unpredictability.

Shannon's **Source Coding Theorem** establishes limits on possible data compression (lossless compression cannot reduce data below its entropy), while the **Noisy-Channel Coding Theorem** determines the maximum rate at which information can be transmitted reliably over a noisy channel.
