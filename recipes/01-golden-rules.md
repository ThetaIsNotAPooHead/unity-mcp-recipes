# Golden rules

Paste this at the start of a session, or put it in your project's `CLAUDE.md`.

```
Rules for working in this Unity project:
1. After creating or editing any script, read the Console and wait for compilation to finish
   before using the new type. Fix compile errors before doing anything else.
2. Save the scene after each finished step.
3. Don't delete or rename existing assets, scenes or GameObjects unless I ask.
4. Put new scripts in Assets/Scripts/<Feature>/ and new prefabs in Assets/Prefabs/.
5. Every new scene needs a Camera and a Directional Light.
6. Prefer [SerializeField] private fields and cache GetComponent calls in Awake.
7. Tell me what you changed at the end of each step.
```

## Why

- **Compile first**: a script that doesn't compile means its component can't be added. The AI keeps retrying and makes a mess.
- **Save often**: if something goes wrong you can reopen the last good scene.
- **No surprise deletes**: the AI can and will "clean up" things you needed.
- Use version control (Git with a Unity `.gitignore`) so you can roll back anything.