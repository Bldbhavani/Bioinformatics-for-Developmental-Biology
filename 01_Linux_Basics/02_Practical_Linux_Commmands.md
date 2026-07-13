# Linuxd Practical Commands

This file contains the practical Linux commands I learned during the Bioinformatics workshop.

Unlike a normal Command list, each command includes:

- What the command does
- Syntax
- Example
- Bioinformatics application
- Developmental biology application
- My own practice

---

# Practival Session 1 - Opening Ubuntu and Understanding the Linux Environment

---

# Objective

Open Ubuntu successfully and understand the Linux environment before running any bioinformatics software.

---

# Background

Ubuntu is a Linux operating system.

Throughout this bioinformatics course, every software tool (FastQC, SRA Toolkit, HISAT2, FeatureCounts, R etc.) will be executed inside Ubuntu.

Therefore, before learning any commands, I must know how to enter the Linux environment correctly.

---

# Step 1 - Turn on the computer

## Action

Swith on the laptop.

Log in to Windows.

---

##  What does this do?

Starts Windows.

Ubuntu runs inside Windows using WSL (Windows Subsystem for Linux).

Therefore Windows must start first.

---

## Why is this important?

Ubuntu cannot run until Windows has started.

---

# Step 2 - Open Ubuntu

## Action

Click the Windows Start Menu.

Search

Ubuntu

Click Ubuntu.

---

## What does this do?

Launches the Ubuntu Linux terminal.

Linux is now preparing my working environment.

---

## Why is this important?

Every bioinformatics analysis will be performed here.

# Step 3 - Enter password

## Action

Type my Ubuntu password.

Press Enter.

---

## What does this do?

Logs into my Linux user account.

---

## Important

Linux Does NOT display characters while typing the password.

This is ocmpletely normal.

Simply type the password and press Enter.

---

# Step 4 - Wait for the prompt

Expected screen

```bash
bhavani@SRI:~$
```

---

## What does this mean?

bhavani

↓

My username

---

SRI

↓

My computer name (host name)

---

~

↓

My Home Directory

---

$

↓

Linux is waiting for my command.

Congratulations!

Ubuntu is now ready.

---

# WHy is Ubuntu used in Bioinformatics?

Most bioiformatics software is developed for Linux.

Example include: 

- FastQC
- SRA Toolkit
- HISAT2
- Bowtie2
- STAR
- Samtools
- FeatureCounts
- BCFtools

Learning Ubuntu means I can use the same tools that researchers use in universities and research institutes.

---

# Developmental Biology Connection

Suppose I am studying embryo implantation using RNA sequecing.

My workflow might be:

Ubuntu

↓

Download sequencing data

↓

Quality Control

↓

Alignment

↓

Gene counting

↓

Differential Expression

↓

Identify genes involved in implantation failure

Everything begins inside Ubuntu.

---

# At this stage I should be able to 

- Open Ubuntu
- Enter my password
- Understand the Linux prompt
- Explain what ~ means
- Explain what $ means

---

## My Experience

**Date:** 13/Jul/2026
**Time:** 11:03 am

---

### Did it work? 
Yes

---

### Did I encounter any errors?
No

---

### What did I learn today?

Every bioinofrmatics analysis begins inside Ubuntu.

Before runnint tools such as FastQC, SRA, Toolkit, HISAT2, STAR, or R, I must first enter the Linux environment correctly.

---

### Confidence level

⭐⭐⭐⭐⭐ (5/5)

I can confidently open Ubuntu without referring to the notes.

---

# Practical Session 2 - Finding My Current Working Directory (pwd)

# Objective

Learn how to identify my current working directory before performing any bioinformatics analysis.

---

# Background

Linux organises files and folders into directories.

Before running any command, I should know where I am currently working.

The `pwd` command helps me identify my current location in the Linux file system.

`pwd` stands for **Print Working Directory**

---

# Step 1 - Open Ubuntu

## Action

Open Ubuntu.

Enter my password.

Wait until the linux prompt appears.

Expected prompt:

```bash
bhavani@SRI:~$
```

---

## What does this do?

This open my Linux environment and prepares it to receive commands.

---

# Step 2 = Type the command

## Action

Type:

```bash
pwd
```

Press **Enter**.

---

## What does this command do?

The `pwd` command asks Linux:

> "Which directory am I currently working in?"

Linux then prints the full path of my current directory.

---

# Step 3 - Observe the Output

## Expected Output

```bash
/home/bhavani
```

Your output might be slightly different if you are already inside another folder.

---

## What does the output mean?

Example:

```bash
/home/bhavani
```

Break it dows:

- `/` -> Root directory
- `home` -> Folder containint all user accounts
- `bhavani` -> My personal Home directory

This means I am currently working inside my own user folder.

---

# Why is this important?

Imagine I want to analyse RNA-seq data.

If I accidentally run FastQC from the wrong folder, Linux will not find my sequencing files.

Therefore, before running any analysis I should first check my location using:

```bash
pwd
```

---

# Bioinformatics example

Before running FastQC:

```bash
pwd
```

Output:

```bash
/home/bhavani/Embryo_Project/Raw_Fastq
```

Now I know FastQC will analyse the correct sequencing files.

---

# Developmental Biology Example

Future project:

```
Embryo_RNAseq/
├── Raw_FASTQ
├── FastQC
├── Alignment
├── Counts
├── Results
└── Figures
```

If I want to analyse the raw sequencing reads, I should first move into:

```bash
/home/bhavani/Emrbyo_RNAseq/Raw_FASTQ
```

Running `pwd` confirms that I am inside the correct project folder.

# Common Begginer Mistakes

Typing:

```bash
PWD
```

Linux is case-sensitive.

Correct:

```bash
pwd
```

---

Forgetting to press **Enter** after typing the command.

---

Assuming I know where I am without checking.

Always verify with:

```bash
pwd
```

# Practice

1. Open Ubuntu.
2. Enter your password.
3. Type:

```bash
pwd
```
4. Press **Enter**.
5. Observe the output.
6. Write the output below.

My Output:

```bash
/home/bhavani
```

# My experience

**Date:** 13-07-2026

**Time:** 11:35 am

### Did it work?

Yes

### Did I encounter any errors?

No

### What did I learn today?

Logging into Ubuntu  and checking which directory I am in

### Confidence level

⭐⭐⭐⭐⭐
