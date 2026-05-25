# RW-0.2.0-Changelogs

### Gameplay & Progression
* Added Level Up system using XP.
* Added pausing mechanic during level up.
* Added Powerup selection and integration.
* Added Legendary system and item foundation.
* Refactored Stat system and added definitions.
* Revised ability meter.

### Enemies & Combat
* Added Enemy AI.
* Added Enemy Spawner for horde mechanics.
* Added dynamic hitboxes linked to animations.
* Added hitbox debugging and adjustment helpers.
* Adjusted dash recovery time.
* Removed direct animator links for dashing.
* Optimized Enemy AI with caching and reduced lookups.

### World, Physics, & Mechanics
* Adjusted physics and movement logic.
* Adjusted ground collision checks.
* Added Tilemap implementation.
* Updated map structure.
* Adjusted parallax scrolling.
* Disabled normal maps.
* Centralized tutorial and player input reading through GlobalInputManager.

### Visuals & UI
* Added UI elements for XP and Stats.
* Added Pixel Perfect Camera toggle test.
* Rescaled player model and sprites to uniform 16ppu from 64ppu.
* Imported new font.
* Added script to show keybinds.

### Documentation
* Added README with game overview and features list.
* Added documentation and comments for PlayerDataHandler.
* Updated .gitignore.