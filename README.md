Infix to Postfix Expression Converter

A C program that converts mathematical expressions from infix notation to postfix notation (Reverse Polish Notation) using the Stack data structure.

📌 Overview

Infix notation (e.g., A+B) is easy for humans to read but difficult for computers to evaluate directly due to operator precedence and parentheses. Postfix notation (e.g., AB+) removes this complexity by placing operators after their operands, making it ideal for compilers, calculators, and expression evaluators.

This project implements the classic stack-based infix-to-postfix conversion algorithm in C.

✨ Features


Converts any valid infix expression to postfix notation
Handles operator precedence (^ > *, / > +, -)
Supports parentheses ()
Implements core stack operations: push, pop, peek
Simple, modular, and beginner-friendly C code


🧠 How It Works


Scan the infix expression from left to right.
If the character is an operand, add it directly to the postfix output.
If the character is (, push it onto the stack.
If the character is ), pop from the stack and add to output until ( is found.
If the character is an operator, pop operators with equal or higher precedence from the stack to the output, then push the current operator.
After scanning, pop any remaining operators from the stack to the output.


🗂️ Project Structure

ModuleDescriptionInput ModuleReads the infix expression from the userStack ModuleImplements push, pop, and peek operationsOperator Handling ModuleManages operator precedence and associativityConversion ModuleCore logic that performs infix → postfix conversionOutput ModuleDisplays the resulting postfix expressionError Handling ModuleValidates input and detects mismatched parentheses

🛠️ Tech Stack


Language: C
Data Structure: Stack (array-based implementation)


🚀 Getting Started

Prerequisites


A C compiler (GCC, Turbo C, or any standard C IDE)


Compilation & Execution

bashgcc infix_to_postfix.c -o infix_to_postfix
./infix_to_postfix

Example

Input:

Enter Infix Expression: (A+B)*(C-D)/E(F*G-H)

Output:

Postfix Expression: AB+CD-*EFG*H-/

📈 Future Enhancements


Postfix expression evaluation
Infix to prefix conversion
Graphical User Interface (GUI)
Support for multi-character operands and floating-point numbers


📚 References


Fundamentals of Data Structures in C – Ellis Horowitz, Sartaj Sahni, Susan Anderson-Freed
Data Structures Using C – Reema Thareja
Programming in ANSI C – E. Balagurusamy
Let Us C – Yashavant Kanetkar
Data Structures with C (Schaum's Outline Series) – Seymour Lipschutz
The C Programming Language – Brian W. Kernighan, Dennis M. Ritchie


👥 Authors


Vikasini Shanmugam
K.E. Ramalakshmi
Subha Kumaresan


Guided by: Mrs. S. Prabavathi, M.E., Assistant Professor/CSE
Department: Freshman Engineering, M. Kumarasamy College of Engineering (Autonomous), Karur

📄 License

This project was developed for academic purposes as part of the CGB1122 – Data Structures course.
