# Introduction to Linux

---

## Learning Objectives

By the end of this lesson I should be able to:

- Explain what an Operating System (OS) is.
- Explain What Linux is.
- Differentiate Linux, Ubuntu and WSL.
- Explain why Linux is widely used in bioinformatics.
- Understand how Linux fits into a bioinformatics workflow.

  ---

  ## Contents

  1. What is an Operating System?
  2. What is Linux?
  3. What is Ubuntu?
  4. What is WSL?
  5. Installing Ubuntu
  6. PowerShell Installation Method
  7. GUI Installation Method
  8. Linux Terminal
  9. Why Bioinformatics Use Linux
  10. Summary
  11. Practice Excercises

  ---

  ## Prerequisites

  Before starting this chapter, I should know:

  - Basic computer usage
  - Windows operating system
  - No previous Linux experience is required
 
---

## Key Takeaways

[] Linux is an Operating System.
[] Ubuntu is a Linux Distribution.
[] WSL allows Ubuntu to run inside Windows.
[] Linux is the preferred operating system for bioinformatics

---

## Developmental Biology Connection

Linux provides the computational environment used to analyse RNA sequencing, single-cell sequencing, single-cell sequencing, epigenomics, and imaging datasets in developmental biology research.

---

## Practice Excercises

(To be completed after the lesson)

## References

Workshop notes

Ubuntu Documentation

Microsoft WSL Documentation

NCBI

  > **Status:** Work in Progress

This chapter will be updated as I continue learning.

---

# 1. What is an Operating System (OS)?

## Definition

An **Operating System (OS)** is system software that manages a computer's hardware and software resources. It acts as an interface between the user and the computer, allowing programs to run efficiently.

Without an operating system, useres cannot easily interact with the computer or execute applications.

---

## Why is an Operating System Needed?

An operating system is responsible for:

- Managing computer memory (RAM)
- Managing files and folders
- Running applications
- Communicating with hardware devices
- Managing input and output devices
- Providing security and user management

Without an operating system, a computer cannot function in a practical way for everyday users.

---

## Common Operating Systems

Some of the most widely used operating systems are:

- Microsoft Windows
- Linux
- macOS

Although they perform similar funtions, they differ in design, features, and intended use.

---

## Analogy

Think of a research laboratory.

| Laboratory | Computer |
|------------|----------|
| Scientist   | User     |
| Laboratory  | Computer Hardware |
| Laboratory Manager | Operating System |
| Experiments | Software Applications |

Just as a laboratory manager organises equipment, schedules experiments, and ensures everything runs smoothly, the operating system manages the computer's resources and coordinates all running programs.

---

## Bioinformatics Perspective

Modern bioinformatics involves analysing large biological datasets such as RNA sequencing, DNA sequencing, and single-cell sequencing.

An operating system provides the environment in which bioinformatics software can run efficiently.

Although Windows and macOS can perform many tasks, Linux is the preferred operating system for most bioinformatics applications.

---

## Developmental Biology Connection

If I analyse RNA sequencing data from developing embryos or implantation studies, the sequencing files are processed using bioinformatics software that typically runs on Linux.

Understanding operating systems is therefore the first step towards learning computational biology.

---

## Key Takeaways

- An Operating System manages the computer.
- It acts as an interface between the user and the hardware.
- It controls files, memory, software, and hardware.
- Linux is one type of operating system commonly used in bioinformatics.

---

# 2. What is Linux?

## Definition

Linux is a free and open-source operating system based on the Linux Kernel. It is one of the most widely used operating systems in scientific research, cloud computing, and bioinformatics.

Unline Windows and macOS, Linux allows users greater control over the system and is highly customizable.

---

Computer

|

|--- Windows
|
|--- macOS
|
|___ Linux
       |
       |--- Ubuntu
       |--- Debian
       |--- Fedora
       |--- Red Hat
       |___ Kali Linux

## History

Linux was created in **1991** by ** Linus Torvalds**, a Finnish computer science student.

His goal was to develop a free operating system that anyone could use, modify, and improve.

Today, Linux is maintained by a global community of developers and is widely used in universities, research institutes, and technology companies.

---

## What is the Linux Kernel?

The **Kernel** is the core component of an operating system.

It acts as a bridge between software and hardware by managing:

- CPU
- Memory (RAM)
- Storage
- Input and Output devices

Linux is built aroudn the Linux kernel.

---

## Why is Linux Popular?

Linux is widely used because it is:

- Free
- Open-source
- Stable
- Secure
- Higly customizable
- Efficient for large-scale computing

These features make Linux the preferred operating system for scientific research and bioinformatics.

---

## Bioinformatics Perspective

Most bioinformatics software is developed for Linux because it provides:

- Better performance
- Easy atomation using shell scripts
- Access to powerful command-line tools
- Compatibility with high-performances coputing (HPC) clusters

Many sequencing analysis pipelines are designed specifically for Linux environments.

---

## Developmental Biology Connection

As a developmental biologist, I may analyse RNA sequencing or single-cell sequencing datasets generated from embryos, stem cells, or implantation studies.

These analyses are commonly performed on Linux systems using bioinformatics software such as FastQC, STAR, HISAT2, Samtools, and R.

Learning Linux is therefore an essential skill for modern developmental research.

---

## Key Takeaways

- Linux is an operating system.
- It was created by Linus Torvalds in 1991.
- Linux is based on the Linux Kernel.
- Linux is free and open-source.
- Most bioinformatics software is designed to run on Linux.

  
