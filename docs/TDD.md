# WARPPOINT — Technical Design Document

## Prototype Architecture
The vertical slice is organized around modular systems so additional weapons, enemies, missions and environments can be added without rewriting the foundation.

## Systems
- Player Controller
- Third-Person Camera
- Health/Stamina
- Weapon System
- Damage System
- Enemy AI
- Loot/Resource System
- Mission/Objective System
- Extraction System
- HUD/UI
- Mobile Input
- Save/Progression foundation

## Gameplay State
Boot → Spawn → Explore → Combat → Extraction → Mission Complete

## Enemy AI State Machine
Idle/Patrol → Detect → Chase → Attack → Recover → Dead

## Weapon Pipeline
Input → Aim/Fire → Projectile/Hit Detection → Damage → Impact Feedback → Ammo Update

## Mobile Input
Virtual movement stick, camera/look area and contextual action buttons. All core gameplay actions must have a touch equivalent.

## Performance Target
Design for a stable 30 FPS or better on supported mobile hardware while maintaining scalable visual quality.

## Repository Strategy
Design documentation, prototypes, source and assets are kept modular so engine-specific implementation can evolve without changing the game design contract.
