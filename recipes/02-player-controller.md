# Player controller from scratch

**Goal:** a playable third-person capsule that walks, sprints and jumps in a new scene.

## Prompt

```
Create a new scene called Playground with a Camera, a Directional Light and a 50x50 ground
plane. Add a Player: a capsule with a CharacterController and a new script
Assets/Scripts/Player/PlayerMovement.cs that does WASD movement relative to the camera,
Shift to sprint, Space to jump, with gravity. Use [SerializeField] fields for walk speed,
sprint speed, jump height and gravity. Make the camera follow behind the player in
LateUpdate with a separate CameraFollow script. Check the Console for compile errors after
writing the scripts, then save the scene.
```

## Check

- Press Play: the capsule moves, sprints, jumps and lands.
- The Console has no errors.
- Speeds show in the Inspector so you can tune them.

## If it goes wrong

- **Player falls through the floor**: "Make sure the ground has a collider and the player starts above it."
- **Moves the wrong way**: "Movement should use the camera's forward and right vectors flattened on Y."
- **Input errors about the Input System**: "Check whether the project uses the new Input System or the old Input Manager in Player Settings and write the input code to match."