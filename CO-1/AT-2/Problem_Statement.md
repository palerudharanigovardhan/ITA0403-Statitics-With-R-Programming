SIMATS ENGINEERING

ASSESSMENT TOOL 2-Pseudocode Writing Task

COURSE NAME: R PROGRAMMING COURSE CODE: ITA04

COURSE OUTCOME COVERED
CO1: Apply R programming fundamentals including data structures, vectors, matrices, arrays,
and class types to perform mathematical operations and manage data effectively. Identify and
implement appropriate control structures to solve a particular programming problem
(Bloom Level -BL3- BL4)
Assessment Tool Weightage: 20%

QUESTIONS: 5 Questions Total Marks: 100

Code of Conduct:

I ___________________ _ (Name / Reg No) certify that this submission is my original
work and that I have adhered to the guidelines specified for this assessment.
I understand that any violation of academic integrity rules will result in disciplinary action.

Signature of the student:

Instructions to students: Write structured pseudocode (not R syntax) for each scenario. Clearly
show inputs, data structures used, control structures (decision, loop), processing steps, and
outputs. Marks: 10 per question.

Q1. Campus Canteen Billing (BL3: Vectors)
The campus canteen stores item prices in a numeric vector price and the quantity ordered in a
vector qty for one customer. Write pseudocode to compute the bill for each item, the total bill,
and apply a 10% discount if the total exceeds ₹500. Display the final payable amount.
Expected concepts: vector arithmetic, element-wise multiplication, sum, if-else.
Q2. Student Marks Analyser (BL3: Vectors, Control Structures)
A teacher stores the marks of 40 students in a vector. Write pseudocode to find (a) the class
average, (b) the highest and lowest mark, and (c) the count of students who scored below 40
(fail). Print &quot;Class Performance: Good&quot; if more than 80% have passed, otherwise &quot;Needs
Improvement&quot;.
Expected concepts: vector functions, logical indexing, counting with condition, if-else.
Q3. Hostel Room Allocation Matrix (BL3: Matrices)
A hostel has 4 floors and 5 rooms per floor. A 4×5 matrix stores 1 if a room is occupied and 0 if
vacant. Write pseudocode to display (a) the number of vacant rooms on each floor, (b) the total
vacant rooms in the hostel, and (c) the floor with the maximum vacancies.
Expected concepts: matrix creation, row-wise sums, nested loops or apply-style logic, finding
maximum.
Q4. Monthly Electricity Bill Calculator (BL3: Control Structures)
An electricity board charges ₹3/unit for the first 100 units, ₹5/unit for the next 100 units, and
₹8/unit beyond 200 units. Given the units consumed by a household, write pseudocode to
compute the total bill. Add a fixed charge of ₹50 and print the bill summary.
Expected concepts: nested if-else / if-else-if ladder, slab-based calculation.
Q5. Sales Report Using Matrix Operations (BL4: Matrices, Analysis)
A shop records the sales of 3 products over 4 weeks in a 3×4 matrix. Write pseudocode to (a)
compute the total sales per product, (b) compute the weekly total sales, (c) identify the best-
performing product and the best week, and (d) transpose the matrix so weeks appear as rows.
Expected concepts: matrix row/column sums, which.max-type logic, transpose, analysis of
results.
Q6. Library Book Management Using Lists (BL3: Class Types and Data Structures)
A library stores details of a book (title, author, year, availability as TRUE/FALSE) in a list.
Write pseudocode to (a) create a list of 5 such books, (b) display all books published after 2015,
and (c) update availability to FALSE when a user borrows a book by title. Show a message if the
title is not found.
Expected concepts: list of lists, loop traversal, condition checking, element update.

Q7. Temperature Data Cleaning (BL4: Vectors, Loops, Analysis)
A weather station records 30 days of temperature readings in a vector, but some entries are NA
(missing) due to sensor failure. Write pseudocode to (a) count the missing values, (b) replace
each missing value with the mean of the valid readings, and (c) classify each day as &quot;Cold&quot;
(&lt;20°C), &quot;Moderate&quot; (20–30°C), or &quot;Hot&quot; (&gt;30°C), storing the result in a new vector.
Expected concepts: NA handling, mean of valid data, loop with if-else ladder, building a new
vector.
Q8. Exam Seating Using 3D Arrays (BL4: Arrays)
An examination hall has 3 blocks, each with 4 rows and 5 columns of seats. A 3D array stores
the register number of the student seated in each position (0 for an empty seat). Write
pseudocode to (a) count the occupied seats in each block, (b) find the block with the highest
occupancy, and (c) display the register number at Block 2, Row 3, Column 4.
Expected concepts: 3D array indexing, nested loops across dimensions, counting non-zero
elements.
Q9. Employee Data Frame Processing (BL4: Data Frames and Class Types)
An HR department maintains a data frame with columns EmpID, Name, Department, and Salary.
Write pseudocode to (a) display employees from the &quot;IT&quot; department earning above ₹50,000, (b)
compute the average salary per department, and (c) give a 10% raise to employees earning below
₹30,000 and add a new column NewSalary.
Expected concepts: data frame filtering, grouping logic, conditional update, adding a column.
Q10. Prime Number and Series Generator for a Maths Club (BL3–BL4: Loops, Vectors)
A maths club needs a program that accepts a number N from the user. Write pseudocode to (a)
generate all prime numbers up to N and store them in a vector, (b) display the sum and count of
those primes, and (c) print the first N terms of the Fibonacci series, also stored in a vector.
Validate that N is a positive integer before proceeding.
Expected concepts: input validation, nested loops with a flag, while/for loops, vector appending,
algorithm design.

Criteria Weightage Level 4 –
Exemplary

Level 3 –
Proficient

Level 2 –
Developing

Level 1 –
Beginning

Problem
Understanding

20% Identifies all
inputs, outputs,
constraints
accurately

Minor
missing
elements

Partial
understanding

Incorrect
interpretation

Algorithm
Design

30% Complete, correct,
and logically
sound solution

Minor
logical gaps

Partially
correct logic

Incorrect
approach

Use of Control
Structures

20% Efficient and
appropriate use of
loops, conditions,
functions/modules
Minor
inefficiencies

Limited or
basic usage

Incorrect or
missing
constructs

Pseudocode
Structure

10% Well-structured,
clear, consistent
format, easy to
follow

Mostly clear
with minor
issues

Difficult to
follow in parts
Poorly
structured
and unclear

Completeness 20% Handles all cases;
optimized
approach

Handles
most cases;
reasonable
efficiency

Handles basic
cases only

Incomplete or
inefficient
