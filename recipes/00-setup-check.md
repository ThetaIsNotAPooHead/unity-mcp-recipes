# Setup and first check

**Goal:** confirm the AI is connected to the right Unity project before it changes anything.

## Prompt

```
Before changing anything: list the connected Unity editor instances, tell me the project
name, Unity version, the open scene, and whether scripts are compiling. Then read the
Console and tell me if there are any existing errors.
```

## Check

- The project name and scene match what you have open.
- If there are existing errors, fix those first (see [Fix compile errors](03-fix-compile-errors.md)). New scripts won't work while the project doesn't compile.

## If it goes wrong

- **No instances found**: the MCP bridge isn't running in the editor. Open its window in Unity and start or restart it, then ask again.
- **Several instances**: tell it which one by name, so it doesn't edit the wrong project.