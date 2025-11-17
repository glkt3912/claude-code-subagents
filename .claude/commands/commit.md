---
description: Generate conventional commit messages from staged changes
---

# Commit Message Generator

Analyze staged changes and generate conventional commit messages.

## Usage

```
/commit
```

## What I'll do

1. Analyze staged changes with `git diff --cached`
2. Identify file types, scope, and change patterns
3. Generate conventional commit message:
   ```
   <type>[scope]: <description>
   
   [optional body]
   
   [optional footer]
   ```

## Commit Types

- `feat`: New feature
- `fix`: Bug fix
- `docs`: Documentation
- `style`: Formatting changes
- `refactor`: Code restructuring
- `perf`: Performance improvements
- `test`: Test changes
- `build`: Build system changes
- `ci`: CI configuration
- `chore`: Maintenance

## Rules

- Imperative mood ("add" not "added")
- Subject under 50 characters
- No emojis or Claude attribution
- Professional, developer-written style