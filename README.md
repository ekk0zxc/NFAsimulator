NFA Simulation (Java)

Description
This program simulates a simple Nondeterministic Finite Automaton (NFA) that checks whether a given string contains the substring "ab"*.

It takes a string input from the user and outputs Accepted if `"ab"` appears anywhere in the string; otherwise, it outputs Rejected.

Features
- Accepts any string as input.
- Uses Java’s `String.contains()` to simulate NFA substring detection.
- Outputs whether the input string is Accepted or Rejected based on the presence of `"ab"`.

NFA Description
Language Accepted:  
All strings over `{a, b}` that contain `"ab"` as a substring.

NFA Definition
- Alphabet (Σ): {a, b}  
- States (Q): {q0, q1, q2}  
- Start State: q0  
- Final State: q2  

Transition Table

| Current State | Input | Next State |
|----------------|--------|-------------|
| q0 | a | q1 |
| q0 | b | q0 |
| q1 | a | q1 |
| q1 | b | q2 |
| q2 | a | q2 |
| q2 | b | q2 |

Accepted Strings Examples:  
- `ab`  
- `aab`  
- `babab`  
- `cabd` (contains “ab”)  
Rejected Strings Examples:
- `a`  
- `b`  
- `aa`  
- `bbbbb`  

### 1. Save the file as:
