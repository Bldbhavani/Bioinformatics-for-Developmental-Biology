# Useful Tips and shortcuts

This page contains useful Linux, WSL and Terminal tips that I discover throughout my bioinformatics learning journey.

These are not part of any single lesson, but they make working in Linux much easier.

---

# WSL Tips

## 1. Open the Current Linux Folder in Windows

### Command

``` bash
explorer.exe .
```

### What does this do?

- Opens the current Linux directory in Windows File Explorer.
- `exolorer.exe` launches Windows Explorer.
- `.` (dot) represents the current directory.

### What does this do?

- Opens the current Linux directory in Windows File Explorer.
- `explorer.exe` launches Windows Explorer.
- `.` (dot) represents the current directory.

### When will I use this?

- After creating folders using `mkdir`.
- After downloading datasets.
- To visually confirm my project structure.

### Example

Current directory:

```bash
/home/bhavani/Emrbyo_RNAseq
```

opens the `Emrbyo_RNAseq` folder directly in Windows Explorer.

### Important Note

This command works only because I am using Ubuntu through WSL.

It will not work on a normal Ubuntu installation.

---

# Terminal Tips

## 2. Clear the Terminal

### Command

```bash
clear
```

or Press

```text
Ctrl + L
```

### What does this do?

Clears the terminal screen without deleting command history.

### When will I use this?

Whenever my terminal becomes cluttered.

---

## 3. Stop a Running Command

### Shortcut

```text
Ctrl + c
```

### What does this do?

Stops the currently running program.

### When will I use this?

If I accidentally start a command that is taking too long or I entered the wrong command.

---

## 4. Auto-complete Commands and Folder Names

### Shortcut

```text
Tab
```

### What does this do?

Automatically completes fiel and folder names.

### Example

Instead of typing:

```text
Emrbyo_RNAseq
```

I can type:

```text
Emb
```

then press **Tab**.

Linux automatically completes the rest.

---

## 5. View previously Executed commands

### Command

```bash
histroy
```

### What does this do?

Displays all commands that I have previously executed.

### When will I use this?

If I forget a command that I used earlier.

---

## 6. View the Current Working Directory

### Command

```bash
ls
```

### Linux usually stays siletnt when a command succeeds.

Example:

```bash
mkdir Embryo_RNAseq
```

No output usually means the command worked successfully.

---

## Linux is case-sensitive.

Correct:

```bash
PWD
```

---

## Check my location before creating files or folders.

Always use:

```bash
pwd
```
before creating new folders.

---

## Verify before continuing.

After creating something, use:

```bash
ls
```

to confirm it exists.

---

## The terminal prompt tells me where I am.

Example:

```bash
bhavani@SRI:~/Embryo_RNAseq$
```

This means I am currently inside:

```text
/home/bhavani/Embryo_RNAseq
```

---

# Good Research Habits

- Organise every project into its own folder.
- Keep raw data separate from processed data.
- Check my location before running commands.
- Verify that files exist before analysing them.
- Use meaningful folder names.
- Never overwrite raw data.

# My Favourite Commands

As I continue learning Linux, I will add the commands that I use most frequently.

| Command | Purpose |
|---------|---------|
| pwd | Show current director |
| ls | List files | 
| mkdir | Create folder |
| cd | Change directory |
