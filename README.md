# MP1: Infinite Matrix

This is my first Unreal Engine project for class. The assignment was to follow a basic tutorial (Kodeco tunnel game) and then expand it into an actual playable Matrix-themed game with new features. It’s not supposed to be a AAA game, just something fun that works and shows off what I learned.

---

## What the game is
You’re basically flying down an endless Matrix tunnel.  
- Dodge walls and enemies  
- Pick up health packs  
- Shoot projectiles at enemies  
- Try to survive as long as possible while the game keeps getting faster  

---

## Features I added

### Health system
- Shows as a bar on the UI  
- You lose health when you hit walls or enemies  
- You don’t instantly die from one hit, but game ends when health hits 0  
- Health resets when you restart  

### Score system
- Increases when you pass through a tunnel hole successfully  
- Shows on the UI  
- Resets to 0 when you restart  

### Health packs
- Spawn randomly in tunnels (but not more than 1 per tunnel)  
- Collect to get health back (can’t go over max health)  
- Disappear if you miss them  

### Projectiles
- Left mouse click shoots a projectile forward  
- Projectiles go faster than the player  
- Destroyed on impact or after a short lifetime  

### Enemies
- Spawn in the tunnel  
- Collide with them = you lose health  
- Shoot them = they get destroyed + you get score  
- Also disappear if you pass them  

### Speed increase
- Player speed ramps up over time  
- Makes the game harder the longer you play  
- Resets when you restart  

### Creative mods
- Walls change color depending on your health (visual feedback)  
- Gave enemies and health packs their own meshes/textures so they look different  

---

## Controls
- **Mouse movement** → move player  
- **Left click** → shoot projectile  

---

## How to play
1. Clone this repo  
2. Open in **Unreal Engine 5 (or above)**  
3. Hit **Play** and survive as long as you can  

---

## Extra notes
- Whole thing was built with Blueprints  
- Collision handled with `OnComponentBeginOverlap` so hits only count once  
- Health/score are displayed using Widget Blueprints  
- Spawning for health packs/enemies is semi-random but fair  

---

## Credits
- Tutorial base: Kodeco “Simple Tunnel Game”  
- Everything else (health, score, enemies, projectiles, etc.) I added myself for the assignment  
