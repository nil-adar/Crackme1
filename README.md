Crackme 1 – Reverse Engineering Analysis
🧠 Overview

This project analyzes a simple crackme binary using static analysis.

The goal was to understand the program logic and find the correct input.

🔍 Analysis Process
Step 1 – Identifying Input

The program receives user input and passes it to a validation function.

Step 2 – Key Assembly Snippet
mov eax, [ebp+8]
add eax, 5
cmp eax, 20
jne fail
Explanation
The input is loaded into eax
5 is added
Compared to 20
💡 Logic Reconstruction (C-like)
if (input + 5 == 20)
    success();
🔓 Solution

The correct input is:

15
🧠 Key Takeaways
Learned to identify arithmetic patterns in assembly
Understood how function arguments are accessed via stack
Practiced translating assembly to high-level logic
