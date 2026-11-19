# Fix compile errors

**Goal:** a clean Console.

## Prompt

```
Read the Console and list every compile error with its file and line. Fix them one file at
a time, starting with the first error, because later errors are often caused by earlier
ones. After each fix, wait for compilation and read the Console again. Don't delete scripts
to make errors go away. Stop and ask me if a fix needs a package to be installed.
```

## Check

- The Console shows no red errors after compilation finishes.
- No scripts were deleted (check Git if you're not sure).

## If it goes wrong

- **Same error keeps coming back**: ask "Show me the full file around the error line and explain the cause before changing it again."
- **Missing namespace/type**: often a package isn't installed (TextMeshPro, Input System, Cinemachine). Install it through the Package Manager.