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

# Practival Session 1 - Linux File System

## Learning Objectives

By the end of this practical session I should be able to:

- Navigate through Linux directories
- Identify my current working directory
- Create folders
- Create files
- Copy, move and delete files
- Understand the Linux file hierarchy
- Organise a bioinformatics project

---

## Understanding the Linux File System

Linux stores everything inside one main directory called the **Root Directory**.

```bash
/
```

Every file and directory originates from the root.

Example:

```
/
├── home
├── usr
├── bin
├── etc
├── tmp
└── var
```

---

## Home Directory

Each Linux user has a personal workspace.

Example:

```bash
/home/bhavani
```

Shortcut:

```bash
~
```

Everything related to my bioinformatics projects will normally be stored here.

Example:

```
/hone/bhavani/Embryo_Project
```

---

## Why is this important?

Before running any bioinformatics software, I should know where my files are stored.

A well-organised directory structure makes projects easier to analyse and reproduce.

---

## Developmental Biology Example

```
Embryo_Project/

├── Raw_FASTQ/

├── FastQC/

├── Alignment/

├── Counts/

├── Results/

└── Figures/
```

