---
layout: project
type: project
image: img/calc.png
title: "Calculator"
date: 2024
published: true
labels:
  - Java
summary: "This Java program implements a stack-based calculator that performs basic arithmetic operations using a custom stack class to handle numbers and operators in a Last-In-First-Out (LIFO) order."
---

<img class="img-fluid" src="../img/calculatorImage.png">

This program implements a stack-based calculator using Java, allowing users to input numbers and operators to perform basic arithmetic operations in a Last-In-First-Out (LIFO) manner. It uses a custom stack class (ArrayStack<E>) to store and manipulate values, supporting standard stack operations such as push(), pop(), peek(), and size checking.

### Key Components:
1. **StackCalculator Class**: 
   - Uses a stack to perform operations.
   - Supports arithmetic operations such as addition, subtraction, multiplication, division, modulus, and exponentiation. 
   - Uses an input loop that allows users to enter numbers and operators interactively. Results of operations are stored back into the stack.

2. **ArrayStack<E> Class**: 
   - Implements the StackInterface<E> for generic stack operations.
   - Manages an array to store the stack's elements, with functionality to push, pop, and peek values.
   - Includes logic to handle exceptions like FullStackException and EmptyStackException.

3. **Main Execution**: 
   - Users can enter numbers to be pushed onto the stack or operators to perform calculations on the top two numbers in the stack.
   - The calculator keeps running until the user inputs "=" to terminate.

4. **Error Handling**: 
   - If the stack is full, a FullStackException is thrown.
   - If there are insufficient numbers for an operation, a message is displayed.

### Example Usage:
- The user enters numbers and operators (+, -, *, /, %, ^), and the program performs the operation on the top two numbers in the stack.
- It provides real-time feedback, displaying the result after each operation, and continues to prompt for inputs until the user ends the program.

This program illustrates how stack-based calculators work and handles basic arithmetic using a LIFO stack mechanism.
 
Source: <a href="https://github.com/theVacay/vacay">theVacay/vacay</a>
