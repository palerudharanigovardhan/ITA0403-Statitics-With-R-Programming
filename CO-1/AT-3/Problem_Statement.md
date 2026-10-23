# SIMATS ENGINEERING

# R PROGRAMMING – ASSESSMENT QUESTIONS

**Course Code:** ITA04  
**Topics Covered:** Matrices, Arrays, and Classes in R

---

# Topic 1: Creating Matrices and Operations on Matrices

## Q1. [Level 3 – Apply]

A shop records the quarterly sales of three products as:

`c(120,150,130,160,90,110,100,115,200,210,190,220)`

Write R code to create a 3 × 4 matrix from this vector filled row-wise, and assign the row names Product1 to Product3 and column names Q1 to Q4. Using `apply()`, compute the total sales of each product and the average sales of each quarter. Display the matrix and show the expected output of each computation.

## Q2. [Level 4 – Analyze]

Consider `A <- matrix(1:6, nrow=2)` and `B <- matrix(1:6, nrow=3)`. Analyze why `A * B` produces an error whereas `A %*% B` executes successfully. Determine the dimensions of the result of `A %*% B` and state the dimension rule that governs matrix multiplication. Then modify `B` so that element-wise multiplication with `A` also becomes possible, and justify how the change satisfies the rule for the `*` operator.

## Q3. [Level 3 – Apply]

Create the 3 × 3 matrix:

`M <- matrix(c(2,1,1,1,3,2,1,0,0), nrow=3, byrow=TRUE)`

Write R code to find its transpose, determinant, and inverse using the appropriate built-in functions. Verify the inverse by multiplying `M` with its inverse using `%*%` and show that the product is the identity matrix. Mention why `round()` may be needed to display the verification result cleanly.

## Q4. [Level 4 – Analyze]

The equations `2x + y + z = 7`, `x + 3y + 2z = 13`, and `x = 1` are written as a coefficient matrix `A` and a vector `b = c(7,13,1)`. Use `solve(A, b)` to obtain the values of x, y, and z. Now replace the third row of `A` with `c(2,6,4)`, which is twice the second row, and analyze why `solve()` fails. Relate your explanation to the determinant and the rank of the matrix.

## Q5. [Level 3 – Apply]

Given `X <- matrix(1:12, nrow=3)`, write R code to extract the second row, the third column, and the sub-matrix formed by rows 1 to 2 and columns 2 to 4. Also extract all elements of `X` that are greater than 6 using a logical condition. Finally, add a new row using `rbind()` and a new column using `cbind()`, and display `dim()` of the matrix after each change.

## Q6. [Level 4 – Analyze]

Let `m <- matrix(1:6, nrow=2)`. Predict and analyze the result of `rbind(m, 7:8)`, noting that `m` has three columns while the added vector has only two elements. Explain the recycling rule applied by R, the values placed in the new row, and the warning message generated. Compare this with `rbind(m, 7:9)` and suggest how a programmer can avoid unintended recycling errors.

## Q7. [Level 3 – Apply]

Create a 4 × 4 matrix using `matrix(1:16, nrow=4)`. Write R code to extract the diagonal elements with `diag()` and compute their sum (the trace). Use `upper.tri()` to extract the elements above the diagonal, and then replace all elements below the diagonal with zero. Display the original and the modified matrix, and state the purpose of the logical matrix returned by `upper.tri()`.

## Q8. [Level 4 – Analyze]

For `M <- matrix(1:9, nrow=3)`, compare the outputs of `apply(M, 1, sum)`, `apply(M, 2, sum)`, `rowSums(M)`, and `colSums(M)`. Analyze how the `MARGIN` argument decides the direction of the operation and what type of object each call returns. Explain a situation where `apply()` with a user-defined function such as `function(x) max(x) - min(x)` is necessary because `rowSums()` cannot be used.

## Q9. [Level 3 – Apply]

The marks of five students in three subjects are stored in a 5 × 3 matrix named `marks`. Write R code to add a fourth column containing the total marks using `rowSums()`, and a fifth column containing the percentage out of 300. Use `which()` to identify the students whose percentage is 60 or above, and use `colMeans()` to find the class average in each subject. Show the expected form of the output.

## Q10. [Level 4 – Analyze]

A programmer executes:

`cbind(marks, Result = c("Pass","Fail","Pass","Pass","Fail"))`

on a numeric marks matrix. Analyze what happens to the numeric values after the call, and explain the rule of type coercion in matrices. Examine the effect of this change on arithmetic operations such as `rowSums()`. Suggest an alternative data structure that stores mixed types correctly and justify your choice.

---

# Topic 2: Creating Arrays and Operations on Arrays

## Q1. [Level 3 – Apply]

Write R code to create a three-dimensional array using `array(1:24, dim=c(3,4,2))`. Assign `dimnames` so that rows are named R1 to R3, columns C1 to C4, and the two matrices are named Sheet1 and Sheet2. Display the array, find its `dim()` and `length()`, and access the element in the second row and third column of Sheet2 using both index numbers and dimension names.

## Q2. [Level 3 – Apply]

A company records sales of 3 branches over 4 quarters for 2 years, stored in:

`sales <- array(1:24, dim=c(3,4,2))`

Using `apply()` with suitable `MARGIN` values, write R code to compute the total sales of each branch, the total sales of each quarter, and the total sales of each year. State which `MARGIN` value is used for each task and show the expected output of the three calls.

## Q3. [Level 4 – Analyze]

For `a <- array(1:24, dim=c(2,3,4))`, analyze the results of `a[1,,]`, `a[,2,3]`, and `a[2,3,4]`. Determine the dimensions and type of object returned by each expression and explain how R drops dimensions of length one. Show how the argument `drop=FALSE` changes the result of `a[1,,]`, and discuss a situation where preserving the dimensions is important.

## Q4. [Level 3 – Apply]

Create two arrays:

`a1 <- array(1:12, dim=c(2,3,2))`

`a2 <- array(12:1, dim=c(2,3,2))`

Write R code to compute their sum, their element-wise product, and the logical array `a1 > a2`. Use `sum()` to count how many elements of `a1` exceed the corresponding elements of `a2`, and use `which()` to find the positions of elements of `a1` equal to 6. Display each result.

## Q5. [Level 4 – Analyze]

Analyze the behaviour of `array(1:5, dim=c(2,3,2))` and `array(1:30, dim=c(2,3,2))`. For the first call, determine how many elements are required, how R recycles the data, and which values appear in the second matrix. For the second call, explain what happens to the extra values. Discuss why silent recycling or truncation can introduce errors in data analysis programs.

## Q6. [Level 3 – Apply]

Let `a <- array(1:24, dim=c(2,3,4))`. Write R code to rearrange its dimensions using `aperm(a, c(2,1,3))` and display the new `dim()`. Verify with code that the element `a[1,2,3]` appears at position `[2,1,3]` in the new array. Then use `aperm(a, c(3,1,2))` and state the new dimensions. Explain, in one sentence, how `aperm()` differs from `t()` for matrices.

## Q7. [Level 4 – Analyze]

Two matrices:

`m1 <- matrix(1:6, nrow=2)`

`m2 <- matrix(7:12, nrow=2)`

are combined using `array(c(m1, m2), dim=c(2,3,2))`. Analyze how the elements of the two matrices are ordered in the resulting array, and compare it with the output of `cbind(m1, m2)` and `rbind(m1, m2)`. Verify using `is.matrix()` and `is.array()` that a matrix is a special case of an array, and explain why.

## Q8. [Level 3 – Apply]

Daily temperatures of 3 cities for 7 days across 2 seasons are stored in an array `temp` of dimension `c(3,7,2)`. Write R code to compute the mean temperature of each city, the highest temperature recorded in each season, and the day number on which the highest temperature occurred in Season 1 using `which.max()`. Also print the temperatures of City 2 for the second season.

## Q9. [Level 4 – Analyze]

For `arr <- array(1:24, dim=c(2,3,4))`, compare the outputs of `apply(arr, 3, sum)` and `apply(arr, c(1,2), sum)`. Determine the dimensions and the values of each result and analyze how a `MARGIN` vector decides which dimensions are retained and which are collapsed.

Predict the output of `apply(arr, c(1,3), sum)` and justify your prediction with the dimensions involved.

## Q10. [Level 3 – Apply]

An array:

`arr <- array(c(-3,5,-1,8,2,-7,4,-6,9,-2,1,-5), dim=c(2,3,2))`

stores profit and loss figures. Write R code to replace all negative values by zero using logical indexing, multiply the entire second matrix layer by 10, and compute the total sum of the array before and after modification. Display the final array and count how many elements were changed.

---

# Topic 3: Classes in R – S3 Class, S4 Class and Reference Class

## Q1. [S3 – Level 3 – Apply]

Create an S3 class `student` by building a list with the elements `name`, `rollno`, and `marks`, and assigning the class attribute using `class()`. Write a `print.student` method that displays the details in a readable format, and a `summary.student` method that returns the grade based on marks. Create two student objects, call `print()` on them, and explain how R selects the correct method.

## Q2. [S3 – Level 4 – Analyze]

A generic function is defined as:

`info <- function(x) UseMethod("info")`

with methods `info.student`, `info.teacher`, and `info.default`. Analyze which method is called for objects of class `student`, `teacher`, and a numeric vector. For an object of class `c("grad_student","student")`, trace how dispatch proceeds when `info.grad_student` calls `NextMethod()`, and predict the order of the printed messages.

## Q3. [S3 – Level 3 – Apply]

Write R code to create an S3 class `employee` with fields `name` and `salary`, and a child class `manager` created by setting:

`class(obj) <- c("manager","employee")`

Define a generic `pay()` with a method for `employee` that returns the salary. Override it for `manager` so that it calls `NextMethod()` and adds a bonus of 10%. Create one object of each class and display the output of `pay()`.

## Q4. [S3 – Level 4 – Analyze]

In S3, the statement:

`s <- structure(list(name="Ravi", marks="abc"), class="student")`

executes without any error. Analyze why S3 does not check the types of its elements, and write a constructor function `new_student()` and a validator function `validate_student()` using `stopifnot()` to enforce a character name and numeric marks. Compare this approach with the built-in validation offered by S4 classes.

## Q5. [S4 – Level 3 – Apply]

Define an S4 class `Person` using `setClass()` with slots `name` of type character and `age` of type numeric. Create an object using `new()`, access and modify a slot using the `@` operator, and display the object. Define a generic `greet` using `setGeneric()` and implement a method with `setMethod()` that prints a greeting using the name slot. Check the class of the object using `is()`.

## Q6. [S4 – Level 4 – Analyze]

An S4 class `Person` is defined with a validity function that returns an error message when age is negative. Predict the outcome of `new("Person", name="Asha", age=-5)`. Then analyze why `p@age <- -10` on an existing object does not raise an error, and explain how `validObject(p)` handles this. Discuss what this behaviour tells about the strictness of validation in S4 compared with S3.

## Q7. [S4 – Level 3 – Apply]

Create an S4 class `Student` that inherits from `Person` using `contains="Person"` and adds a numeric slot `marks`. Write a `show` method for `Student` that calls `callNextMethod()` to print the person details and then prints the marks. Create an object, display it, and use `is(obj, "Person")` to test inheritance. Also write code to list all slots of the class using `slotNames()`.

## Q8. [Reference Class – Level 3 – Apply]

Using `setRefClass()`, define a class `Account` with a numeric field `balance` and the methods `deposit()` and `withdraw()`. Use the `<<-` operator inside the methods to modify the field, and make `withdraw()` display a message when the balance is insufficient. Create an object with balance 1000, deposit 500, withdraw 2000 and withdraw 300, and show the final balance after each operation.

## Q9. [Reference Class – Level 4 – Analyze]

Two Reference class objects are created as:

`a <- Account$new(balance=1000)`

`b <- a`

`c <- a$copy()`

After executing `a$deposit(500)`, analyze and predict the balances of `a`, `b`, and `c`. Explain why modification through `a` affects `b` but not `c`, and contrast this reference behaviour with the copy-on-modify behaviour seen in S3 and S4 objects.

## Q10. [S3 vs S4 vs Reference – Level 4 – Analyze]

A bank application requires objects whose state changes over time, a parent-child hierarchy of account types, and strict checking of field types. Analyze how S3, S4, and Reference classes meet each requirement by comparing class definition syntax, method ownership (generic function versus object), mutability, and validation. Justify, with short code outlines, which system suits this application best and state one drawback of your choice.

---

**End of Assessment Questions**
