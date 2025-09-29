# Exception-Handling-in-CPP

# Aim: 
To study and implement Exception Handling in C++ for error detection, handling, and program stability.

# Tools Used: 
IDE, C++ compiler, try-catch blocks, throw statements, exception classes.

# Theory:

In C++, Exception Handling is a mechanism to handle runtime errors, allowing programs to continue execution or terminate gracefully. It separates normal logic from error-handling logic.

-Exceptions are unexpected or unusual situations that occur during program execution, like division by zero, file not found, or invalid input.

-Exception handling provides a structured way to detect and respond to these errors.

-The mechanism uses three keywords: try, catch, and throw.

-The try block contains code that may cause an exception.

-The throw statement signals the occurrence of an exception.

-The catch block handles the exception and provides corrective measures.

# 🔹 Key Features of Exception Handling:

Provides a way to handle runtime errors without crashing the program.

Separates normal code from error-handling code.

Allows propagation of exceptions to higher-level functions if needed.

Supports multiple types of exceptions for different error conditions.

# 🔹 Syntax of Exception Handling in C++:

try {
   // Code that may cause exception
   if(condition) {
       throw exception_type;
   }
} 
catch(exception_type e) {
     // Code to handle exception
}
# 🔹 Types of Exceptions:

Standard Exceptions – Predefined in C++ standard library (e.g., std::overflow_error, std::runtime_error).

User-defined Exceptions – Custom exceptions defined by the programmer using classes or other data types.

Multiple Exceptions – Catching different types of exceptions using multiple catch blocks.

# 🔹 Advantages of Exception Handling:

Improves program reliability and stability.

Prevents program crashes due to runtime errors.

Makes debugging easier by providing detailed error information.

Supports modular and maintainable code by separating normal and error-handling logic.

Divide by 0 Error:
This program demonstrates how exceptions can be used to handle runtime errors. It checks for division by zero using a try block. If the divisor is zero, an exception is thrown and caught by a catch block, preventing the program from crashing and displaying an appropriate error message.

# ALGORITHM:

1> Start

2> Declare variables n1, n2, and ans.

3> Prompt the user to input two numbers.

4> Use a try block to check if n2 is zero.

If n2 is zero, throw n2 as an exception.

Otherwise, calculate ans = n1 / n2 and display the result.

5> Use a catch block to handle the exception and display an error message if division by zero occurs.

6> End

Access Code:
This program demonstrates how exceptions can be used to validate input. It checks whether the entered code matches the predefined private code. If the code is incorrect, an exception is thrown and caught by a catch block, displaying an error message. If the code is correct, access is granted.

# ALGORITHM:

1> Start

2> Declare a variable code to store user input.

3> Prompt the user to enter the private code.

4> Use a try block to check if the entered code is correct.

If the code is not equal to 9762, throw the entered code as an exception.

Otherwise, display "Access Granted".

5> Use a catch block to handle the exception and display an error message if the entered code is incorrect.

6> End

# Conclusion:
Exception handling in C++ provides a robust way to manage runtime errors, ensuring programs can handle unexpected situations gracefully without crashing. By using try, throw, and catch, developers can separate normal logic from error-handling code, improving program reliability, maintainability, and ease of debugging. This mechanism allows both standard and user-defined exceptions to be handled efficiently, enhancing overall program stability.
