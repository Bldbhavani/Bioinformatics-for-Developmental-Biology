# Laboratory Practical 2 - First R program

---

## Objective

By the end of this practical, I should be able to:

- Open RStudio
- Run my first R commands
- Understand how R perform calculations
- Interpret the output shown in the Console

## Opening RStudio

1. Open Ubuntu.
2. Log in.
3. Open the Terminal.
4. Type:

```bash
rstudio
```

5. Press **Enter**.

Expected Result:

- RStudio opens successfully.
- The console is ready to accept commands.

---

## Our first R command

In the Console, type:
2+2
Press **Enter**.
Expected Output:
[1] 4

### Explanation

- `2` and `2` are numbers.
- `+` tells R to perform addition.
- R calculates the results and prints it in the Console.

### Note

The output begins with:

```r
[1]
```

This means the first value being displayed starts at position 1.

It is normal and does **not** indicate an error.

---

## Check the Working Directory

Command:

```r
getwd()
```
Purpose:

Displays the current working directory used by R.

Example Output:

```r
[1] "/home/bhavani"
```
Note:

This is equivalent to the Linux command:

```bash
pwd
```

The full path of the folder where R is currently reading and writing files.

---

## Variables

Variables allow us to store information in memory so that it can be reused later in the program.

Instead of typing the same value repeatedly, we can save it with a meaningful name.

Example:

```r
a <- 10
```

To display the value stored in the variable:

```r
a
```

Output:

```r
a
```

R displayed the value stored inside the variable.

### Why is this useful?

Variable make programs easier to read and modify.

Instead of remembering numbers, I can use meaningful names such as:

```r
gene_expression
emrbyo_count
control_emrbyos
```

Which makes the code much easier to understand.

---
## Different Types of Data

A variable can store different kinds of information.

### Integer / Numeric

```r
a <- 10
```

### Decimal

```r
a <- 2.5
```

### Text (Character)

```r
a <- "Bhavani"
```

Text must always be enclosed inside quotation marks.

---

## Mistakes I made

I typed:

```r
a <- Bhavani
```

Error:

```r
Error: object 'Bhavani' not found
```

Why did this happen?

R interpreted 'Bhavani' as the name of another variable instead of text.

How I fixed it:

```r
a <- "Bhavani"
```

Lesson Learned:

Text values must always be enclosed in quotation marks.

---

### Mistake 2

I typed:

```r
total_embryos
```

before creating it.

Error:

```r
Error: Object 'total_embryos' not found
```

Why did this happen?

The variable had not yet been created.

How I fixed it:

```r
total_embryos <- crontrol_emrbyos + treated_embryos
```

Lesson Learned:

A variable must exist before it can be used.

---

## Built-in Functions

Functions allow R to perform operations automatically.

Functions I learned today:

| Function | Purpose |
| 'sqrt()' | Square root |
| 'mean()' | Calculate average |
| 'sum()' | Add values |
| 'max()' | Largest value |
|'min()' | Smallest value |
| 'length()' | Count the number of values |

---

## My First Vector

Command:

```r
gene_expression <- c(gene_A, gene_B, gene_C)
```

Output:

```r
[1] 150 220 275
```

What is `c()`?

The `C()` function combines multiple values into a single object called a **vector**.

Why is this important?

Real bioinformatics datasets contain thousands of values.

Instead of creating thousands of variables, R stores them together inside vectors.
