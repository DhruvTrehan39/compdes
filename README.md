# Regular Expression to DFA Converter

This code implements a C++ program that converts a regular expression into an NFA (Non-deterministic Finite Automaton) and then into a DFA (Deterministic Finite Automaton). The code allows users to input a regular expression and test strings to verify whether they belong to the language defined by the regular expression.

## Features

- Preprocessing: Converts the regular expression into a form suitable for parsing.
- Postfix Conversion: Transforms the regular expression into postfix notation.
- NFA Construction: Builds an NFA from the postfix expression.
- DFA Conversion: Converts the NFA into a DFA.
- String Simulation: Accepts strings and checks if they match the regular expression based on the constructed DFA.


To compile and run this code, you need:

- A C++ compiler (like `g++` or any IDE with C++ support).
- Standard C++ libraries.

### How to Run

1. Clone the repository (or download the file):
    ```bash
    git clone https://github.com/your-repo/regex-to-dfa
    ```
    Or simply download the `regex-to-dfa.cpp` file.

2. Compile the code** using a C++ compiler. For example:
    ```bash
    g++ regex-to-dfa.cpp -o regex-to-dfa
    ```

3. Run the executable:
    ```bash
    ./regex-to-dfa
    ```

4. Input a regular expression** in the format supported by the program:
    - Supports input characters like `a`, `b`, concatenation (`.`), union (`|`), and Kleene star (`*`).

5. Check strings: Enter strings to verify if they belong to the language defined by the regular expression.

6. Exit by entering `1` as the string when prompted.

### Example

Sample input:

```
Input a regular expression: (a|b)*abb
```

**Output:**

```
Transition table for the NFA of the given regex
...

Transition table for the DFA of the given regex
...

Input a string to check: ababb
Given string belongs to the given regular expression.
```

## Code Structure

- initialise(): Initializes the NFA transition table.
- preprocessor(): Processes the regular expression to add concatenation operators.
  postfix(): Converts the regular expression into postfix notation.
- reg_nfa(): Constructs the NFA from the postfix expression.
- print_nfa_table(): Displays the transition table for the NFA.
- nfa_dfa(): Converts the NFA into a DFA.
- print_dfa_table(): Displays the DFA transition table.
- simulator(): Simulates the DFA on user-provided input strings.
- main(): Manages the input and execution flow.

## License

This project is for educational purposes. Feel free to modify and distribute.

## Author

- Dhruv Trehan
