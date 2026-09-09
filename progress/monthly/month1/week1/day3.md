# 💻 Day 3 — Linux Search & Text Processing

**Phase 0 → Linux Basics**

Day 3 focused on searching files and finding specific information inside files using Linux command-line tools.

The main goal was to understand the difference between searching the **filesystem** and searching **file contents**.

---

## 🎯 Goals

- Learn `grep` for searching text inside files.
- Learn `grep -i` for case-insensitive searches.
- Learn `grep -n` for displaying matching line numbers.
- Learn `find` for searching files and directories.
- Understand the difference between `find` and `grep`.
- Practice searching through log files.
- Understand basic output redirection using `>`.

---

## 🖥️ Environment

- **OS:** Windows 10
- **Linux Environment:** WSL 2
- **Distribution:** Ubuntu
- **Working Directory:** `/home/abhishek/engineering-lab`

---

# 🔎 1. `grep` — Search Inside File Content

`grep` is used to search for specific text or patterns inside files.

Basic syntax:

```bash
grep "text" filename
```

Example:

```bash
grep "ERROR" server.log
```

Mental model:

```text
File
 ↓
grep
 ↓
Matching lines
```

---

## 🔤 2. Case-Insensitive Search

Used:

```bash
grep -i "error" server.log
```

The `-i` option makes the search case-insensitive.

Therefore, it can match:

```text
error
Error
ERROR
```

---

## 🔢 3. Search With Line Numbers

Used:

```bash
grep -n "ERROR" server.log
```

The `-n` option displays the line number along with the matching line.

This is especially useful when debugging logs or large text files.

---

# 📁 4. `find` — Search Files & Directories

`find` is used to search the filesystem for files and directories.

### Find all files

```bash
find ~/engineering-lab -type f
```

### Find all directories

```bash
find ~/engineering-lab -type d
```

Mental model:

```text
-type f → file
-type d → directory
```

### Find specific file types

For example, to find `.txt` files:

```bash
find ~/engineering-lab -type f -name "*.txt"
```

---

# 🔥 5. `find` + `grep`

A practical engineering use case is combining filesystem search with content search.

The objective was to understand:

```text
find → Where is the file?
grep  → What is inside the file?
```

This distinction is important when working with large projects, server logs, debugging environments, and infrastructure systems.

---

# 🧪 Practical Lab

Created a `logs` directory:

```bash
mkdir logs
cd logs
```

Created log files:

```bash
touch app.log server.log crash.log
```

Added sample log information using `echo` and output redirection:

```bash
echo "Info Server Started Sucessfull" > app.log
echo "Server has been crashed by chuliyapa.com" > crash.log
echo "Server has been restarted but one problem fount to be resolve" > server.log
```

Verified their contents using:

```bash
cat app.log
cat crash.log
cat server.log
```

Then practiced searching for specific text:

```bash
grep "crashed" crash.log
```

and:

```bash
grep "Server" crash.log
```

---

# ⚠️ Important Lesson — `>` Redirection

During the lab, I accidentally used:

```bash
grep "crashed" > crash.log
```

without specifying an input file.

This helped me understand that:

```bash
>
```

redirects command output into a file and can **overwrite existing content**.

The correct search command was:

```bash
grep "crashed" crash.log
```

This was an important practical lesson because the mistake demonstrated the difference between **searching a file** and **redirecting command output**.

---

# 🧠 Key Concepts Learned

```text
cat
 ↓
Read file content

grep
 ↓
Search text inside file

find
 ↓
Search files/directories

>
 ↓
Redirect output to a file
```

### Core distinction

```text
find → "File कहाँ है?"

grep → "File के अंदर क्या लिखा है?"
```

---

# 🛠️ Commands Practiced

| Command | Purpose |
|---|---|
| `mkdir` | Create directory |
| `cd` | Change directory |
| `touch` | Create empty file |
| `ls` | List files/directories |
| `cat` | Read file content |
| `echo` | Write/display text |
| `grep` | Search text |
| `grep -i` | Case-insensitive search |
| `grep -n` | Search with line numbers |
| `find` | Search filesystem |
| `find -type f` | Find files |
| `find -type d` | Find directories |
| `>` | Redirect/overwrite output |

---

# 🚀 Engineering Takeaway

Linux systems can contain thousands of files and very large log files.

Manually reading every file is inefficient.

Tools like:

```text
find
grep
```

allow engineers to quickly locate files and extract relevant information.

These skills will become increasingly useful for:

- Server debugging
- Log analysis
- Linux administration
- Automation
- Infrastructure engineering
- Troubleshooting production systems

---

# ✅ Day 3 Completion

- [x] `grep` understood
- [x] `grep -i` practiced
- [x] `grep -n` practiced
- [x] `find` understood
- [x] `find -type f` practiced
- [x] `find -type d` practiced
- [x] `find + grep` practiced
- [x] Log-search challenge completed
- [x] Output redirection `>` understood
- [x] Practical mistakes and troubleshooting completed

**Day 3 Status: ✅ COMPLETE**

---

## 📌 Next

**Day 4 → Next Linux skill from Phase 0**

The focus will remain on one skill at a time with practical terminal exercises.
