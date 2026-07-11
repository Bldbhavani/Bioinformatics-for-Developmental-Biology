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

│

├── Windows
│
├── macOS
│
└── Linux
      │
      ├── Ubuntu
      ├── Debian
      ├── Fedora
      ├── Red Hat
      └── Kali Linux

---

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

---

# 3. What is Ubuntu?

## Definition

Ubuntu is a **Linux distrubution (Linux idstro)** based on the Linux operating system. It provides a user-friendly interface and comes with pre-installed software, making Linux easy to install and use.

Ubuntu is one of the most popular Linux distributions for beginners, researchers, and bioinformaticians.

---

## Relationship between Linux and Ubuntu

Linux is the operating system (Kernel).

Ubuntu is a distribution built using the Linux Kernel.

---

Ubuntu is **not a different operating system**. It is one version of Linux.

---

Ubuntu is widely used because it is:

- Free and open source
- Beginner-friendly
- Stable and secure
- Regularly updated
- Compatible with most bioinformatics software

For these reasons, Ubuntu is commonly recommended for bioinformatics training and research.

---

## Bioinformatics Perspective

Many bioinformatics tools are developed and tested on Ubuntu

Examples include:

-FastQC
-SRA Toolkit
-BWA
-Bowtie2
-HISTA2
-SRAR
-Samtools

Installing Ubuntu provides and environment where these tools can be installed and executed easily.

---

## Developmental Biology Connection

During my future PhD, I may analyse sequecing datasets from embryos, stem cells, placental tissue, or infertility studies.

Ubuntu provides the computational environment required to run the bioinformatics software used in these analyses.

---

## Key Takeaways

- Ubuntu is a Linux distribution.
- Ubuntu is based on the Linux kernel.
- Ubuntu is beginner-friendly
- Ubuntu is widely used in bioinformatics.

---

# 4. What is WSL (Windows Sybsystem for Linux)?

## Definition

Windows Subsystem for Linux (WSL) is a copatibility feature developed by Microsoft that allows users to run a Linux environment directly on Windows without installing a separate operating system or using a virtual machine.

WSL enable Linux commands, applications, and tools to run alongside Windows.

---

## Why was WSL Developed?

Many scientific, engineering, and software development tools are designed for Linux.

Instead of requiring users to install Linux separately or dual boot their computers, Microsoft introduces WSL so that Linux could run directly within Windows.

---

## How Does WSL Work?

WSL acts as a bridge between Windows and Linux.

---

Windows
    │
    ▼
Windows Subsystem for Linux (WSL)
    │
    ▼
Ubuntu
    │
    ▼
Linux Terminal

---

When youn open Ubuntu on your Windows computer, WSL allows Ubuntu to communicate with your computer's hardware.

---

## Why do we use WSL?

Using WSL allows us to:

- Run Linux commands on Windows
- Install bioinformatics sofware
- Execute Linux-based workflows
- Access Linux tools without leaving Windows

This makes learning bioinformatics much easier for Windows users.

---

## Bioinformatics Perspective

Most bioinformatics software is developed for Linux.

WSL allows Windows users to install and use these tools without needing a separate Linux computer.

Examples include:

- FastQC
- SRA Toolkit
- STAR
- HISAT2
- Samtools
- BWA

---

## Key Takeaways

- WSL stands for Windows Subsytem for Linux.
- WSL allows Linux to run inside Windows.
- WSL is not a virtual machine.
- WSL allows Ubuntu to run on Windows.
