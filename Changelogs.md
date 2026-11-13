# 0.3.0-Changelogs

### Gameplay & Progression
* Split stats into additive and multiplicative modifiers.
* Added absolute modifiers with a warning display.
* Split `EntityDataHandler` into modules.
* Added an experimental weapon and upgrade system with world pickups.
* Removed Level Up, XP, Powerup selection, and the Legendary system.

### Enemies & Combat
* Added death handling for players and enemies.
* Hitboxes now use `HitboxData` assets and scale with the hitbox size stat.
* Fixed hitbox offset not scaling with size.
* Fixed jump attack overwrite; hitboxes now disable on landing.
* Added transition from jump attack back to idle.
* Removed enemy friendly fire.

### Movement & Traversal
* Added grappling hook with rope visual, above/below variants, and target indicator.
* Added ledge grabbing with mantle recovery and ledge jumps.
* Added multiple jumps, long jump, and minimum jump height.
* Added sprinting.
* Dash and jumps now refresh on ledge grab and grapple.
* Removed friction and retuned movement.
* Player now phases through enemies.
* Respawn now resets velocity.
* Fixed jumps resetting on wall contact.

### World, Physics, & Mechanics
* Added new tiles, background, hidden areas, and scene objects.
* Added a respawn trigger at the bottom of the map.
* Camera now supports unbounded sides.
* Moved draw order from Z position to sorting layers.
* Moved spawn points to prevent clipping.

### Visuals & UI
* Added lighting layer and grapple lighting.
* Rope now renders pixelated.
* Improved warning popup readability.
* Standardized positive, negative, and neutral stat colors.

### Input & Controls
* Moved controls to Input Actions.
* Split `PlayerInput` into separate modules.

### Performance
* Added chunk loading.
* Added enemy pooling.
* Cached movement lookups to reduce overhead.
* Added slow motion debug mode and VSync.

---

# 0.2.0.1-Changelogs

### Input & Controls
* Fixed missing `GlobalInputManager` script causing input failures.

### Visuals & UI
* Added Tutorial Popup UI element.
* Added additional UI elements to the gameplay scene.

### Performance
* Added FPS limiter and performance display.

---

# 0.2.0-Changelogs

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
* Centralized tutorial and player input reading through `GlobalInputManager`.

### Visuals & UI
* Added UI elements for XP and Stats.
* Added Pixel Perfect Camera toggle test.
* Rescaled player model and sprites to uniform 16ppu from 64ppu.
* Imported new font.
* Added script to show keybinds.

### Documentation
* Added README with game overview and features list.
* Added documentation and comments for `PlayerDataHandler`.
* Updated `.gitignore`.

---

# 0.1.0-Changelogs

### Player
* Added Player Character.
* Added animations: Attack, Run, Jump, Dash, DashAttack, SpecialAttack.
* Added sword hitboxes and hurtboxes.

### Input & Controls
* Added input:
  * `A` / `D`: Left / Right
  * `LMB`: Attack (combo up to 3)
  * `Z` (`Y` on QWERTZ): Special Attack
  * `E`: Dash

### Gameplay & Progression
* Added Stat System with a `Stat` class.
* Added stats: `maxHealth`, `currentHealth`, `Damage`, `SpeedPercentage`, `LifeStealPercent`, `LifeStealFlat`, `LifeCount`, `InvincibilitySeconds`.

### Enemies & Combat
* Added Enemy layer.
* Added Enemy/Player damage.

### World, Physics, & Mechanics
* Added map with a rough walkable area.
* Added `InitializeTagAndLayer`, which sets the tag and layer of a GameObject's children.

### Visuals & UI
* Added Camera Follow with x-axis limits.
* Added `DisplayHealthRemaining`, which shows an entity's remaining HP as text.

### Documentation
* Added Roadmap to README.
