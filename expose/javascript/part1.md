1. What is printed by line 9? If the code returns an error, explain why.
   values added: 20
2. What is printed by line 13? If the code returns an error, explain why. 
   final result: 20
3. Why should you not use var? Explain why. 
   It does not have block scope, which can lead to unexpected behavior or bug, such as accidentally accessing or overwriting variables.
4. What is printed by line 9? If the code returns an error, explain why.
   values added: 20
5. What is printed by line 13? If the code returns an error, explain why. 
   This will throw an error because result is not defined outside the if statement.
6. What is printed by line 9? If the code returns an error, explain why.
   This will throw an error because result is defined as const and const means the variable cannot be reassigned, and the code is attempting to reassign result
7. What is printed by line 13? If the code returns an error, explain why. 
   This will throw an error because this code is trying to access result outside of its block scope, and const is block-scoped, so result is not defined.