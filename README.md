# 🚀 C++ Learning Journey

> A structured, hands-on roadmap to master C++ — from fundamentals to concurrency and performance.  
> All notes, code exercises, and projects are organized by phase.

---

## 📅 Learning Roadmap Overview

| Phase | Topic | Timeline | Est. Hours | Projects |
|-------|-------|----------|------------|----------|
| 1 | Solidify the Fundamentals | Apr – May Wk1 | 20 hrs | 2 |
| 2 | OOP + Memory Ownership | May | 35 hrs | 2 |
| 3 | STL + Modern C++ Essentials | Jun | 35 hrs | 2 |
| 4 | File I/O + CLI Tool | Jul | 30 hrs | 1 |
| 5 | Templates & Generic Programming | Aug – Sep | 40 hrs | 2 |
| 6 | Concurrency & Performance | Sep – Oct | 65 hrs | 2 |
| | **TOTAL** | **~7 months** | **~225 hrs** | **11** |

---

## 📦 Phase 1 — Solidify the Fundamentals
**Timeline:** Apr – May Wk1 &nbsp;|&nbsp; **Est. Hours:** 20

### 📖 Topics
- Compilation process — How preprocessor → compiler → linker works
- Translation units — Header vs `.cpp` files, include guards
- Pointers & references — Difference between `*` and `&`, pass by value/ptr/ref
- `const` correctness — `const` on variables, parameters, member functions
- Namespaces — Avoiding name collisions, using declarations

### 💻 Coding & Debug Tasks
- Set up compiler + build system (`g++` / CMake)
- Write Hello World split across multiple `.cpp`/`.h` files
- Trace memory addresses with pointer exercises
- Fix 10 linker error examples intentionally

### ⭐ Projects
- **Number Guessing Game** — Multi-file project
- **Student Records Manager** — Pointers + references

---

## 📦 Phase 2 — OOP + Memory Ownership
**Timeline:** May &nbsp;|&nbsp; **Est. Hours:** 35

### 📖 Topics
- Classes & constructors — `this` pointer, constructor/destructor lifecycle
- Inheritance & polymorphism — Virtual functions, vtable, `override` keyword
- Abstract classes — Pure virtual functions, interface design
- Stack vs heap — `new`/`delete`, when each is used
- RAII — Resource Acquisition Is Initialization pattern
- Smart pointers — `unique_ptr`, `shared_ptr`, `weak_ptr`
- Rule of 3/5 — Copy ctor, copy assign, destructor + move variants

### 💻 Coding & Debug Tasks
- Implement Base/Derived class hierarchy from scratch
- Observe destructor call order in inheritance
- Cause and fix a memory leak deliberately
- Refactor: Replace raw `new`/`delete` with `unique_ptr`

### ⭐ Projects
- **Shape Area Calculator** — Virtual polymorphism
- **Custom String Builder class** — Rule of 3

---

## 📦 Phase 3 — STL + Modern C++ Essentials
**Timeline:** Jun &nbsp;|&nbsp; **Est. Hours:** 35

### 📖 Topics
- STL containers — `vector`, `map`, `unordered_map`, `set` — internals & complexity
- Iterators — `begin`/`end`, range-based for, iterator categories
- STL algorithms — `sort`, `find_if`, `transform`, `accumulate`
- Lambda expressions — Capture by value/ref, generic lambdas
- Move semantics — `std::move`, rvalue references, move constructor
- `auto` & `decltype` — Type deduction, structured bindings

### 💻 Coding & Debug Tasks
- Benchmark `vector` vs `list` insertion (measure time)
- Implement map-based word frequency counter
- Rewrite loops using `std::transform` and lambdas
- Write move constructor for a custom class

### ⭐ Projects
- **Contact Book CLI** — Add/search/delete/sort
- **CSV Analyzer** — Filter, sort, aggregate

---

## 📦 Phase 4 — File I/O + CLI Tool
**Timeline:** Jul &nbsp;|&nbsp; **Est. Hours:** 30

### 📖 Topics
- `fstream` — Text and binary file read/write
- `std::filesystem` (C++17) — Directory traversal, path manipulation
- Command-line args — `argc`/`argv`, argument parsing
- Error handling — `try`/`catch`, `std::exception`, custom exceptions
- String processing — `stringstream`, regex basics, tokenization

### 💻 Coding Tasks
- Read and write binary files
- Traverse a directory recursively
- Parse `argv` into a command dispatch map
- Implement SHA256 file hash (use a library)

### ⭐ Projects
- **Multi-command CLI Tool** — Search / rename / copy / hash

---

## 📦 Phase 5 — Templates & Generic Programming
**Timeline:** Aug – Sep &nbsp;|&nbsp; **Est. Hours:** 40

### 📖 Topics
- Function templates — Template type deduction, explicit specialization
- Class templates — Templated containers, member functions
- Variadic templates — Parameter packs, fold expressions
- `constexpr` — Compile-time constants and functions
- Concepts (C++20) — Constraining templates, `requires` clauses
- SFINAE basics — `enable_if`, type traits

### 💻 Coding Tasks
- Write a templated `max()` and `swap()`
- Implement templated `Stack<T>` class
- Use concepts to constrain a sorting template

### ⭐ Projects
- **Generic Data Structure Library** — vector / stack / queue
- **Compile-time Unit Converter**

---

## 📦 Phase 6 — Concurrency & Performance
**Timeline:** Sep – Oct &nbsp;|&nbsp; **Est. Hours:** 65

### 📖 Topics
- `std::thread` — Creating, joining, detaching threads
- Mutex & `lock_guard` — Data race prevention, RAII locking
- `condition_variable` — Producer-consumer pattern
- `atomic` — Lock-free operations, memory ordering
- Thread pool — Task queue, worker thread design
- Cache locality — Data layout for performance, false sharing
- Memory alignment — `alignas`, `aligned_alloc`
- Profiling — `gprof`, `perf`, Valgrind basics

### 💻 Coding & Debug Tasks
- Cause and detect a data race
- Implement producer-consumer with `condition_variable`
- Build a simple thread pool from scratch
- Benchmark cache-friendly vs cache-unfriendly access
- Profile a program with Valgrind / perf

### ⭐ Projects
- **Parallel File Processing Tool**
- **Thread Pool Task Scheduler**

---

## 🗂️ Repo Structure

```
cpp_learning/
│
├── phase1_fundamentals/
├── phase2_oop_memory/
├── phase3_stl_modern/
├── phase4_file_io_cli/
├── phase5_templates/
├── phase6_concurrency/
│
└── README.md
```

---

## 🛠️ Environment Setup

- **Compiler:** `g++` (GCC 11+) or `clang++`
- **Build System:** CMake
- **Standard:** C++17 / C++20
- **Tools:** Valgrind, gprof, perf

Compile any file with:
```bash
g++ -std=c++17 -Wall filename.cpp -o output
./output
```

---

## 🎯 End Goal

By the end of this roadmap, I aim to:
- Write clean, modern, idiomatic C++ code
- Confidently manage memory without leaks
- Use the STL and generic programming effectively
- Build concurrent, high-performance applications

---

*Started: April 2025 — Happy Learning! 💪*
