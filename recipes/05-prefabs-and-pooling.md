# Prefab and pooling workflow

**Goal:** turn spawned objects into prefabs and pool them instead of Instantiate/Destroy every time.

## Prompt

```
Make a Bullet prefab in Assets/Prefabs: a small sphere with a Rigidbody (no gravity), a
trigger collider and a Bullet script that moves it forward and returns it to the pool after
3 seconds or on hit. Create a BulletPool script using UnityEngine.Pool.ObjectPool<Bullet>
with a default capacity of 20. Add a Gun script to the Player that fires from the pool on
left click with a fire rate field. Check for compile errors and save.
```

## Check

- Play and hold fire: the Hierarchy shows a fixed set of bullets being reused instead of new ones piling up.
- No errors in the Console.

## If it goes wrong

- **Bullets keep old velocity**: "Reset the Rigidbody's velocity and position when a bullet is taken from the pool."
- **Bullets never return**: "Make sure the return timer restarts each time the bullet is taken from the pool."