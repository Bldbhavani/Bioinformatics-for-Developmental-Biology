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
