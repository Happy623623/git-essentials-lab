# Running the Library Demo

This guide shows how to run the small library application included in this repository.

## Prerequisites

- **JDK 17 or later.** Both `java` and the compiler `javac` must be available, because the runner compiles the Java code before running it.
- **Python 3.9 or later.** The runner script uses only Python's standard library.
- **Git**, if you still need to clone the repository.

No IDE, Maven, Gradle, or extra Java library is required.

## Run

Open a terminal in the repository's top-level folder and run:

```
python3 run.py demo
```

On Windows, if `python3` is not found, use the Python launcher instead:

```
py -3 run.py demo
```

## What the demo does

The demo runs a fixed scenario on a fixed date (2026-09-01) so the output is the same every time. It prints the borrowing limits for students and faculty, searches the catalog for a title, lets a member borrow a book and shows its due date, and then returns the book and shows the late fee and the number of active loans.

Example output:

```
Library loan demo (fixed date: 2026-09-01)
Student limit: 2
Faculty limit: 2
Search for 'git': []
Loan: Git Essentials
Borrowed by: Alex; due: 2026-09-15
Return fee: 0
Active loans after return: 0
```

Note that searching for `git` finds nothing because the baseline search is case-sensitive, while the book title is `Git Essentials`.