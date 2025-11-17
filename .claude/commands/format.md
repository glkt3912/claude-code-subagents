---
description: Format code across multiple languages including Markdown with markdownlint compliance
args: "[file_pattern]"
---

# Code Formatter

Format code files with proper styling and markdownlint compliance.

## Usage

```
/format [file_pattern]
```

## Examples

- `/format` - Format all files in current directory
- `/format *.md` - Format all Markdown files  
- `/format src/` - Format all files in src directory

## What I'll do

1. Detect file types and existing configurations (.prettierrc, .markdownlint.json, etc.)
2. Apply appropriate formatting rules:
   - JavaScript/TypeScript: Prettier + ESLint
   - Python: Black + isort
   - Markdown: markdownlint compliance
   - JSON/YAML: Structure formatting
3. Fix common issues:
   - Remove trailing spaces
   - Fix indentation
   - Add missing blank lines around headings/code blocks
   - Ensure single trailing newline
4. Provide summary of changes made

Target files: $ARGUMENTS