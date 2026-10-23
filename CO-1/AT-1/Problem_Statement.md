# SIMATS ENGINEERING

## ASSESSMENT TOOL 1 – Constraint-Based Problem Solving (Level 1)

**Course Name:** R Programming  
**Course Code:** ITA04  
**Assessment Tool Weightage:** 20%  
**Total Questions:** 5  
**Total Marks:** 100 (5 × 20)

### Course Outcome Covered

Apply R programming fundamentals, including data structures, vectors, matrices, arrays, and class types, to perform mathematical operations and manage data effectively.

**Bloom's Taxonomy Level:** BL2–BL4

---

## Question 1: Vectors – Weekly Sales Analysis

### Problem Statement

A shop records the number of units sold on each day of a week: Monday – 12, Tuesday – 18, Wednesday – 9, Thursday – 25, Friday – 30, Saturday – 14, and Sunday – 22.

### Constraints
- Store the data in a single named vector using `c()`.
- Do not use any loop (`for`, `while`, or `repeat`).
- Use logical indexing instead of manually selecting positions.
- Round the average to two decimal places.

### Tasks
(a) Create the named vector of sales.  
(b) Calculate the total and average sales for the week.  
(c) Display only the days whose sales are above the weekly average.  
(d) Find the name of the day with the highest sales.

---

## Question 2: Lists – Student Record

### Problem Statement

A teacher wants to maintain a record for a student named Asha, who scored 78, 85, and 92 in three tests and has passed the course.

### Constraints
- Use a single list to store the name (character), marks (numeric vector), and passed (logical).
- Access elements only with `$` or `[[ ]]`.
- Add the new element by assignment without rebuilding the list.
- Do not use a data frame.

### Tasks
(a) Create the list named `student`.  
(b) Calculate the average of the marks using the list element.  
(c) Add a new element named `grade`: `"A"` if the average is 85 or above; otherwise, `"B"`.  
(d) Display the number of elements in the list and their names.

---

## Question 3: Matrices – Operations on Two Matrices

### Problem Statement

Matrix A contains the numbers 1 to 9 arranged row by row in a 3 × 3 grid. Matrix B is a 3 × 3 matrix containing the row-wise values 1, 0, 2, 0, 1, 0, 3, 0, and 1.

### Constraints
- Create both matrices using `matrix()` with the `byrow = TRUE` argument.
- Do not use loops.
- Use `*` for element-wise multiplication and `%*%` for matrix multiplication.
- Use base R functions only.

### Tasks
(a) Create matrices A and B.  
(b) Compute the element-wise product of A and B.  
(c) Compute the matrix product of A and B.  
(d) Find the transpose of A and the row sums of A.

---

## Question 4: Arrays – Three-Dimensional Data

### Problem Statement

A warehouse stores 12 item counts in a three-dimensional structure with 2 rows, 3 columns, and 2 layers. The counts are the numbers 1 to 12.

### Constraints
- Create the structure using `array()` with the `dim` argument.
- Do not use loops.
- Extract values using comma-separated index notation, such as `arr[row, col, layer]`.
- Use `apply()` to calculate the layer totals.

### Tasks
(a) Create the array named `arr` with `dim = c(2, 3, 2)`.  
(b) Display the entire second layer.  
(c) Extract the element in row 2, column 3, of layer 1.  
(d) Calculate the sum of each layer.

---

## Question 5: Class Types and Coercion – Price List

### Problem Statement

Prices read from a text file have been stored in R as the character vector `"120"`, `"85.5"`, and `"200"`. The shop needs to calculate the total bill after applying a 10% discount.

### Constraints
- Do not retype the prices as numbers; convert the existing vector.
- Use `as.numeric()` for conversion.
- Check the type using `class()` before and after conversion.
- Do not use loops.

### Tasks
(a) Create the character vector and display its class.  
(b) Convert the vector to numeric and display the new class.  
(c) Calculate the total and the discounted total.  
(d) Create `c(1, "a", TRUE)`, state its class, and explain why R chose it.

---

## Code of Conduct

I, ______________________________ (Name / Registration Number), certify that this submission is my original work and that I have adhered to the guidelines specified for this assessment.

I understand that any violation of academic integrity rules will result in disciplinary action.

**Signature of the Student:** ______________________________

---

## Assessment Criteria

| Criteria | Weightage | Level 4 – Exemplary | Level 3 – Proficient | Level 2 – Developing | Level 1 – Beginning |
|---|---:|---|---|---|---|
| Problem Understanding | 20% | Identifies all inputs, outputs, and constraints accurately | Minor missing elements | Partial understanding | Incorrect interpretation |
| Algorithm Design | 30% | Complete, correct, and logically sound solution | Minor logical gaps | Partially correct logic | Incorrect approach |
| Use of Control Structures | 20% | Efficient and appropriate use of loops, conditions, functions, and modules | Minor inefficiencies | Limited or basic usage | Incorrect or missing constructs |
| Pseudocode Structure | 10% | Well-structured, clear, consistent, and easy to follow | Mostly clear with minor issues | Difficult to follow in parts | Poorly structured and unclear |
| Completeness | 20% | Handles all cases with an optimized approach | Handles most cases with reasonable efficiency | Handles basic cases only | Incomplete or inefficient |
