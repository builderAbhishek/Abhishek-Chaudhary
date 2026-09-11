# Week 1 — Engineering Journey

**Phase:** Phase 0 — Setup & Developer Environment  
**Focus:** Linux & Developer Environment  
**Week:** 1  
**Days:** 1–7  
**Status:** 🟡 In Progress

---

## 🎯 Week Goal

Build a working Linux development environment and become comfortable with basic Linux filesystem operations through hands-on practice.

---

## 🗺️ Weekly Progress

| Day | Focus | Status |
|---|---|---|
| Day 1 | WSL2, Ubuntu & Linux Navigation | ✅ Complete |
| Day 2 | Linux Files & Directories | ✅ Complete |
| Day 3 | Linux Search & Text Processing | ✅ Complete |
| Day 4 | File Permissions | ✅ Complete |
| Day 5 | Pipes & Redirection | ⬜ |
| Day 6 | Linux Practice Lab | ⬜ |
| Day 7 | Weekly Review & Documentation | ⬜ |

---

# 📚 Day 1 — WSL & Linux Navigation

### Learned

- WSL2
- Ubuntu on WSL
- Linux home directory
- `pwd`
- `ls`
- `ls -la`
- `cd`
- `cd ..`
- `cd ~`
- Basic Linux filesystem navigation

### Practical Work

Created:

```text
/home/abhishek/engineering-lab
```

### Key Learning

Linux has its own filesystem and home directory structure. The Linux home directory for the current user is:

```text
/home/abhishek
```

---

# 📚 Day 2 — Linux Files & Directories

### Learned

- Creating files with `touch`
- Creating directories with `mkdir`
- Reading files with `cat`
- Copying with `cp`
- Moving with `mv`
- Renaming with `mv`
- Removing files with `rm`
- Basic output redirection using `>`

### Practical Work

Created and manipulated a project structure:

```text
engineering-lab/
└── project/
    ├── README.md
    ├── src/
    │   └── main.cpp
    ├── docs/
    │   └── notes.txt
    └── backup/
        └── main-backup.cpp
```

### Key Learning

Linux filesystem operations can be understood as:

```text
Create → Read → Copy → Move → Rename → Delete
```

---

# 🧠 Engineering Lessons

### 1. Terminal errors are useful

During Day 1, I accidentally typed:

```bash
pwsd
```

instead of:

```bash
pwd
```

The terminal suggested the correct command.

**Lesson:** Read error messages before searching for solutions.

### 2. Practice matters more than memorization

Commands become easier to remember when they are used to solve an actual filesystem problem.

### 3. Understand the operation

Instead of memorizing commands independently:

```text
mkdir → create directory
touch → create file
cat → read
cp → copy
mv → move / rename
rm → delete
```

the goal is to understand the underlying filesystem operation.

---

# 🧪 Hands-On Work

- [x] WSL2 verified
- [x] Ubuntu installed
- [x] Linux terminal configured
- [x] Linux home directory explored
- [x] Engineering workspace created
- [x] Files created
- [x] Directories created
- [x] Files copied
- [x] Files moved
- [x] Files renamed
- [x] Files deleted
- [x] File contents read
- [x] Basic redirection practiced

---

# 📈 Week 1 Status

**Days Completed:** 4 / 7

**Phase 0 Progress:** 🟡 In Progress

**Current Focus:** Linux Basics

---

# 🔜 Upcoming

The next focus will be Linux tools for:

- Searching files
- Searching text
- Filtering output
- Understanding file permissions
- Pipes and redirection

---

## 🔗 Daily Logs

- [Day 1 — WSL & Linux Navigation](./day1.md)
- [Day 2 — Linux Files & Directories](./day2.md)
- [Day 3 - Linux Search & Text Processing](./day3.md)
- [Day 4 - File Permissions](./day4.md)
- [Day 5](./day5.md)
- [Day 6](./day6.md)
- [Day 7](./day7.md)
