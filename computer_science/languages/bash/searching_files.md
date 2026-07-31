---
tags:
  - bash
  - grep
  - ysap
  - piping
  - search
  - terminal
date: 2026-07-31
---

---
status: #complete 
class backlink: [[ysap_bash_scripting]]

# Searching in Files (Ch 01, Sec 03)

**command:** `cat [file]` (print file content to screen)

**command:** `grep [pattern] [file]` (filter)
* `^` match beginning only
* `$` match end only
* `''` wrapping keeps BASH from interpreting

**command:** `echo [str] > [file]`
* pipes (overwrite) str into file
* `>>` appends instead of overwrite

**command:** `grep -A1 [pattern] [file]` (prints grep filter but 1 line after)
* `B` does N lines before
* `C` does N lines before and after (context)

**command:** `grep -i [pattern] [file]` (grep case insensitive)

**command:** `grep -o [pattern] [file]` (grep only prints what matches pattern not whole line)

* flags are position indifferent

Piping: `cmd 1 | cmd 2 [input]`
* output connects to input
ex: `cat dict | grep -i dave | grep i`

---
Directly Related Subjects

- 


