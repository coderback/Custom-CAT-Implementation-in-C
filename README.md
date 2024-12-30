# Custom-CAT-Implementation-in-C
A custom implementation of the cat command in C with additional features and a focus on demonstrating buffer overflow vulnerability detection and prevention. Includes options for line numbering, blank line suppression, and line-ending formatting. Designed for educational purposes in order to understand file handling and security in C programming.

## Overview
This repository contains a custom implementation of the `cat` command in C, with additional features and a demonstration of buffer overflow vulnerability detection.

The program reads content from files or standard input and applies optional formatting based on command-line flags.

## Features
- Supports the following options:
  - `-b`: Number non-blank lines.
  - `-e`: Append a `$` symbol at the end of each line.
  - `-n`: Number all lines.
  - `-s`: Suppress consecutive blank lines.
- Demonstrates buffer overflow detection by using a `controlValue` check.
- Reads input using a deliberately vulnerable structure to highlight potential security issues.

## Usage
```bash
./cat_implementation [-b] [-e] [-n] [-s] [file ...]
