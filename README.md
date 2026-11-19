# unity-mcp-recipes

Copy-paste prompts and workflows for building Unity games with an AI assistant (Claude Code, Cursor, etc.) connected to the Unity Editor over **MCP** (Model Context Protocol), for example with [MCP for Unity](https://github.com/CoplayDev/unity-mcp).

The AI can create GameObjects, write scripts, read the Console and run tests in your open editor. These recipes are the prompts and habits that actually make that work instead of wrecking your scene.

## Recipes

| Recipe | Use it for |
|---|---|
| [Setup and first check](recipes/00-setup-check.md) | Making sure the AI can see your editor before you start |
| [Golden rules](recipes/01-golden-rules.md) | The habits that stop broken scenes and compile loops |
| [Player controller from scratch](recipes/02-player-controller.md) | A playable character in one session |
| [Fix compile errors](recipes/03-fix-compile-errors.md) | Getting out of a red Console fast |
| [Build a level blockout](recipes/04-level-blockout.md) | Greyboxing a level with primitives or ProBuilder |
| [Prefab and pooling workflow](recipes/05-prefabs-and-pooling.md) | Turning things into prefabs and pooling spawns |

> **Status:** early. These recipes follow Unity best practices but haven't all been tested across Unity versions and MCP servers yet. If one works (or doesn't) for you, open an issue with your Unity version and MCP server.

## Contributing

Got a prompt that works great? Add it as a new file in `recipes/` following the same layout (goal, prompt, what to check). See [CONTRIBUTING.md](CONTRIBUTING.md).

## License

MIT