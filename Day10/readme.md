# Linux Practice Lab – Users, Directories & Files

## Hands-On Linux Filesystem Practice

> Date 18th May, 2026 - Day 10

> Objective: Practice Linux navigation, user management, directory creation, file creation, and filesystem visualization.

---

# Task 1 - Verify Current Logged-in User

## Run:

```bash
whoami
```

## Questions

- What username is displayed?
- Are you logged in as root or a normal user?

---

# Task 2 - Navigate to the /home Directory

## Run:

```bash
cd /home
```

## Verify Your Current Location

Run:

```bash
pwd
```

Expected output:

```bash
/home
```

---

# Task 3 - List the Contents of /home

## Run:

```bash
ls -l
```

## Observation

- What do you see?
- Are there any user directories already created?

> NOTE: On a fresh installation there should normally be NO regular user directories unless users were already created earlier.

---

# Task 4 - Create Two Users

## Run:

```bash
useradd student
useradd Alice
```

## Verify the Users Were Created

Run:

```bash
ls -l /home
```

Expected output should now include:

```bash
student
Alice
```

---

# Task 5 - Navigate to Alice's Home Directory

## Run:

```bash
cd /home/Alice
```

## Verify Your Current Location

Run:

```bash
pwd
```

Expected output:

```bash
/home/Alice
```

---

# Task 6 - Check the Contents of Alice's Directory

## Run:

```bash
ls -l
```

## Observation

- What do you see?
- There should be nothing inside Alice's home directory initially.

---

# Task 7 - Create Multiple Directories Using mkdir -p

## Run: You can create all these directories in one go!

```bash
mkdir -p projects docs images
```

## Verify the Directories

Run:

```bash
ls -l
```

Expected directories:

- projects
- docs
- images

---

# Task 8 - Navigate to the projects Directory

## Run:

```bash
cd projects
```

## Verify the Contents

Run:

```bash
ls -l
```

OR

```bash
ll
```

## Observation

- Is the directory empty?

---

# Task 9 - Create a File

## Run:

```bash
touch report.txt
```

## Verify the File Was Created

Run:

```bash
ls -l
```

Expected output should include:

```bash
report.txt
```

---

# Task 10 - Move One Level Up

## Run:

```bash
cd ..
```

## Verify Your Current Location

Run:

```bash
pwd
```

Expected output:

```bash
/home/Alice
```

---

# Task 11 - List the Contents Again

## Run:

```bash
ls -l
```

## Observation

You should now see:

- projects
- docs
- images

---

# Task 12 - Navigate to the images Directory

## Run:

```bash
cd images
```

## Verify the Directory Contents

Run:

```bash
ls -l
```

## Observation

- Is the images directory empty?

---

# Task 13 - Create an Image File

## Run:

```bash
touch logo.png
```

## Verify the File

Run:

```bash
ls -l
```

Expected output:

```bash
logo.png
```

---

# Task 14 - Return to Your Home Directory

## Run:

```bash
cd
```

## Questions

- Do you see the tilde symbol `~`?
- The tilde `~` means you are inside your home directory.

---

# Task 15 - Verify Your User and Current Directory

## Run:

```bash
whoami
pwd
```

## Questions

- Which user are you logged in as?
- Which home directory are you currently inside?

---

# Task 16 - Install the tree Package

## Run:

```bash
dnf install -y tree
```

## Important Practice

During installation:

Press:

```bash
Ctrl + C
```

## Observation

- What happened?
- The installation should stop/interupt.

---

# Task 17 - Install tree Again

## Run:

```bash
dnf install -y tree
```

## This Time

Allow the installation to complete successfully.

---

# Task 18 - Display the Linux Directory Hierarchy

## Run:

```bash
tree -d /home
```

## Observation

- Do you see the directory hierarchy?
- Can you identify:
  - Alice
  - projects
  - docs
  - images

---

# Final Questions

1. What does `whoami` do?
2. What does `pwd` display?
3. What does `cd ..` mean?
4. What does `cd` by itself do?
5. What is the purpose of `touch`?
6. Why is `tree` useful?
7. What does the tilde `~` represent?
8. What does `mkdir -p` do?

---

# Final Reflection

Write a short paragraph explaining:

- What you learned from this lab
- Which command was most useful
- Which command was difficult
- Why Linux filesystem navigation is important

---
