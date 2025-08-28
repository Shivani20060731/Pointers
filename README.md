# Pointers
Aim: To study and implement pointer concepts, pointer arithmetic, and memory management in C++.It allows direct access and manipulation of the data stored at that address.

Apparatus: VS Code or Online C++ Compiler
Theory:
Pointers are one of the most powerful and fundamental features in C++.
Theory

In C++, parameters can be passed to functions in three different ways:

1. Pass by Value – A copy of the variable is passed. Changes do not affect the original variable.


2. Pass by Pointer – The address of the variable is passed. Using *, the function can modify the original variable.


3. Pass by Reference – An alias of the variable is passed. Changes directly affect the original variable.



Key Differences:

Pass by Value → Safe but no changes in the original data.

Pass by Pointer → Original data can be modified using addresses.

Pass by Reference → Direct and efficient modification of original data without using pointers.



Programs & Algorithms

Program 1: Swapping Numbers (Pass by Value)

Algorithm:

1. Start


2. Declare integers a=5, b=10.


3. Call swap(a, b) where copies are passed.


4. Inside function: Swap the copies using a temporary variable.


5. Print a and b in main().


6. Stop



Expected Result: Values in main remain unchanged.


Program 2: Swapping Numbers (Pass by Pointer)

Algorithm:

Program-2: Swapping Numbers by Pass by Pointer
Description: Demonstrates Pass by Pointer. The swap function modifies the original variables by using their addresses.

Algorithm:

Declare two integer variables a and b.

Display values of a and b before swapping.

Call swap function, passing addresses of a and b.

Inside swap:

Store *x in a temporary variable.
Assign *y to *x.
Assign temp to *y.
Display swapped values in main().

Expected Result: Values are swapped permanently.


---

Program 3: Swapping Numbers (Pass by Reference)

Algorithm:

1. Start


2. Declare integers a=15, b=13.


3. Call swap(a, b) where parameters are references (&).


4. Inside function: Swap using temp variable.


5. Print updated a and b in main().


6. Stop



Expected Result: Values are swapped permanently.


Program 4: Salary Incrementation

Algorithm:

1. Start


2. Input salary, proj, pub, prof, new_proj.


3. Check performance conditions (any 3 criteria satisfied).


4. If satisfied → Call increment_ref(salary) to increase salary by 20%.


5. Else → Call increment_val(salary) (copy incremented, original unchanged).


6. Print final salary.


7. Stop



Expected Result: Salary changes only when passed by reference.


---

Program 5: Changing Array Elements

Algorithm:

1. Start


2. Declare integer array arr[5] = {1,2,3,4,5}.


3. Print initial array.


4. For each element, call change_val(arr[i], 1000) where function has reference parameter.


5. Print modified array.


6. Stop



Expected Result: All array elements change to 1000.

conclusion 
the experiments clearly show how different parameter passing techniques in C++ affect data manipulation inside and outside functions. When using pass by value, only copies of the variables are modified, leaving the original values unchanged. On the other hand, pass by pointer and pass by reference directly work with the original variables, making the changes permanent and efficient. Through programs like swapping numbers, incrementing salaries, and modifying arrays, it becomes evident that pass by value is useful for preserving data, while pointers and references are essential when direct modification of the original data is required.

