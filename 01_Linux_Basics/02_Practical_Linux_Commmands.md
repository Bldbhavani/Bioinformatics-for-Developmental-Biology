# Linux Practical Commands

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

---

# Step 2 - List the contents

## Action

Type:

```bash
ls
```

Press **Enter**.

---

## What does this command do?

Limux displays all files and folders inside my current directory.

---

## Expected output

The output will vay depending on what is stored in my Home directory.

Example:

```bash
Desktop
Documents
Downloads
Music
Pictures
Videos
```

## Why is this important?

Before creating a new project, I should know what folders already exists.

This prevents duplicate folders and helps keep my work organised.

---

## Bioinformatics Example

Before downloading RNA-seq data, I can use:

```bash
ls
```

to check whether a project folder already exists.

---

## Developmental Biology Example

```text
Embryo_RNAseq
```

I can use `ls` to verify whether I haved already created it.

---

## What did I see when I entered command `ls`?

R

This is because I am using Ubuntu inside WSL, not a full Ubuntu desktop installation.

WSL starts with a very minimal Linux environment. The only thing I've created so far is the R directory.

# Practical Session 4 - Creating My First Research Project (mkdir)

# Objective

Create my first developmental bioinformatics porject directory.

--- 

# Background

A directory (folder) is used to organise files.

Every research project should have its own directory.

Keeping projects organised makes analyses easier to reproduce and prevents files from becoming mixed together.

The `mkdir` command stands for **Make Directory**.

---

# Step 1 - Cehck my current location

Type 

```bash
pwd
```

---

## Why?

To confirm I am inside my Home directory before creating a new project.

---

# Step 2 - View existing folders

Type 

```bash
ls
```

## Why?

To check whether my project already exists.

---

# Step 3 - Create my project

```bash
mkdir Embryo_RNAseq
```

Press Enter.

---

## What does this do?

Creates a new folder named **Embryo_RNAseq** inside my Home directory.

---

## Why is this important?

Every bioinformatics project should have its own organised workspace.

---

# Viewing Linux files in Windows

Sometimes I may want to visually check whether a file or folder has been created.

Since I am using **Ubuntu through Windows Sybsystem for Linux (WSL)**, I can open my current Linux directory directly in Windows File Explorer.

---

# Step 1 - Confirm my current directory

Type:

```bash
pwd
```

Example output:

```bash
/home/bhavani
```

## Why am I doing this?

This tells me which Linux folder I am currently working in.

---

# Step 2 - Open the current directory in Windows

Type:

```bash
explorer.exe .
```

Press ** Enter**.

---

## What does this command do?

- `explorer.exe` launches Windows file explorer.
- `.` (dot) represents the **current directory**.

Together, this command opens the folder I am currently working in.

---

## Expected Result

Windows File Explorer opens and displays the contents of my Linux Home directory.

Example:

```text
Embryo_RNAseq
R
.config
.cache
.local
```

## Why is this useful?

- Verify that a new folder has been created.
- View Linux files using a familiaar windows interface.
- Easily copy or inspect files.
- Confirm that my project structures is correct.

---

## When will I use this?

After creating new folders using:

```bash
mkdir
```

or downloading datasets, I can use:

```bash
explorer.exe .
```

to visually confirm that everything is in the correct location.

---

## Important Note

This command works because I am using **Ubuntu through WSL**.

It is **not a standard Linux command** and will not work on a normal Ubuntu installation.

---

## Expected Output

After pressing **Enter**, Linux usually does **not** display any message.

Example:

```bash
bhavani@SRI:~$ mdkir Emrbyo_RNAseq
bhavani@SRI:~$
```

---

## What does this mean?

Linux successfully created the folder.

Unlike many Windows programs, Linux normally remains silent when a command executes successfully.

No output usually means **success**.

---

## How do I know it worked?

Type:

```bash
ls
```

Example output:

```bash
Embryo_RNAseq R
```

If `Embyro_RNAseq` appears, the folder has been created successfully.

---

## Why is this important?

Creating separate project folders keeps research organised.

Each bioinformatics project should have its own workspace to avoid mixing files from different analyses.

---

## Bioinformatics Example

Before starting a new RNA-seq analysis, I can create a dedicated project folder:

```bash
mkdir Embryo_RNAseq
```

All files related to this project will be stored inside this directory.

---

## Developmental Biology Example

Suppose I am studying gene expression during embryo implantation.

```text
Embryo_RNAseq
```

This folder will contain all sequencing data, quality control results, alignment files, gene counts, figures, and final resutls for this study.

---

## Common Beginner Mistakes

### Mistake 1

Trying to create a folder that already exists.

Example:

```bash
mkdir Embryo_RNAseq
```

Linux will display:

```text
mkdir: cannot directory `Emrbyo_RNAseq`: File exists
```

### Mistake 2

Forgetting to check whether the folder was created.

Always verify using:

```bash
ls
```

---

# Practical Session 5 - Changing Directories (`cd`)

# Objective

Learn how to move form on directory (folder) to another in Linux.

---

# Background

The `cd` comamnd changes my current working directory.

Instead of working in my Home directory all the time, I can move into my project folder.

`cd` stands for **Change Directory**.

 ---

 ## Action

 Type:

 ```bash
pwd
```

Press **Enter**.

---

## Expected Output

```bash
/home/bhavani
```

## Why am I doing this?

Before changing directories, I should know my current location.

---

Step 2 - View available foldersw

## Action

Type:

```bash
ls
```

Press **Enter**.

---

## Expected Output

Example:

```bash
Emrbyo_RNAseq R
```

---

## What does this command do?

Moves me from my current directory into the `Embryo_RNAseq` folder.

The command does not create or copy anything.

It simply changes my working location.

---

# Step 4 - Verify my new location

## Action

Type:

```bash
pwd
```

Press **Enter**.

---

## Expected output

```bash
/home/bhavani/Embryo_RNAseq
```

## What does this output mean?

I am now working inside my research project.

Every new folder and file I create will now be stored here unless I move somewhere else.

---

## Why is this important?

Linux always performs commands in the current directory.

If I am in the wrong location, I may accidentally create files in the wrong place or analyse the worng dataset.

---

## Bioinformatics Example

Before downloading sequencing data, I should first enter my project folder.

```bash
cd Embryo_RNAseq
```

Then all download files will remain organised inside this project.

---

## Developmental Biology Example

Suppose I am studying embryo implantation.

I first entr:

```bash
cd Emrbyo_RNAseq
```

Everything related to ths study-including RNA-seq data, quality control reports, alignments, and figures will be stored inside this project.

---

## Common Beginner Mistakes

### Mistake 1

Typing the folder name incorrectly.

Example:

```bash
cd embryo_rnaseq
```

Linux is case-sensitive.

Correct:

```bash
cd Embryo_RNAseq
```

---

### Mistake 2

Trying to enter a folder that does not exist.

Linux will display an error.

Always check using:

```bash
ls
```

---

# Practical Session 6 - Organising a Bioinformatics Project

# Objective

Learn how to organise a bioinformatics project by creating meaningful directories.

---

# Background

Research projects contain many different types of files.

Keeping them organised makes easier, prevents mistakes, and improves reproducibility.

Instead of storing in one folder,  each stage of the analysis should have its own directory.

---

# Step 1 - Confirm I am inside my project

Type:

```bash
pwd
```

Expected output:

```bash
/home/bhavani/Emrbyo_RNAseq
```

---

# Step 2 - Create project folders

Type the following commands one at a time:

```bash
mkdir 01_Raw_Data
mkdir 02_Quality_Control
mkdir 03_Trimmed_Data
mkdir 04_Alignment
mkdir 05_Counts
mkdir 06_Differential_Expression
```

## What does this do?

Creates a professional folder structure for an RNA-seq project.

Each folder represents one stage of the bioinformatics workflow.
