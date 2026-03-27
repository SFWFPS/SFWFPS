# ***SFWFPS Changelog***

**Repository:** https://github.com/sfwfps/SFWFPS
**Project:** Single-file HTML5 raycasting game — a wholesome “Plushie Edition” of DOOM. Fully playable at https://sfwfps.com.

**March 26, 2026**
- BUG: Identified a landscape bug on iOS. Investigating.
- Integrated Beta Steam Deck compatibility (D-pad and standard button mapping only for now).
- Fixed a critical game freeze bug that triggered when defeating the second enemy on the first level.
- Improved the raycaster math using bitwise operations and added a hard step limit to the raycaster to prevent infinite loops.
- Implemented global DOM caching to significantly reduce game lag and prevent further freezing issues.
- Game hosting migrated to https://sfwfps.com.
- The Toy Box System: Implemented a multi-weapon arsenal (Magic Wand, Warm Milk, Heavy Pillow, Lullaby Box) featuring distinct fire rates, damage stats, spread patterns, particle effects, and custom animations.
- Dodge Mechanic: Added a skill-based dash move that grants invincibility frames (i-frames). Perfectly timing a dodge against the Boss's instant-kill attack awards a massive combo-scaled score bonus.
- Dynamic Drops: Built an intelligent loot system that drops ammo boxes and includes a "pity drop" mechanic that boosts health item spawns when the player's HP is critically low.
- Untouched Bonus: Introduced a passive scoring system that trickles points to the player after avoiding damage for 5 seconds, scaling up the longer they remain unhit.
- High Score Board: Built a fully functional "Top 10 Sleepers" menu using localStorage, complete with an arcade-style initials prompt when players break a record, plus a UI fix for landscape scrolling.
- Anti-Clumping AI: Upgraded enemy pathfinding with a separation vector so plushies naturally fan out instead of merging into a single sprite when swarming.
- Performance Optimizations: Dramatically improved framerates by removing expensive CSS shadowBlur effects, implementing painted oval drop-shadows, and caching background gradients.
- Engine Bug Fixes: Fixed a fatal infinite loop in the raycaster near portals, reversed particle array loops to stop memory thrashing, and expanded the Z-buffer FOV culling to stop the Boss from flickering out of existence.
- Stat Tracking: Expanded the victory screen to display total boops, highest combo, plushies saved, and the player's most used weapon.

**March 25, 2026**
- Migrated code to a new org and renamed/redesigned the cover art.
- Boss UI: Implemented a dedicated, stylized health bar overlay for the final Boss encounter.
- Difficulty Selection: Added the "Sleepiness Level" start menu to allow players to choose Easy, Normal, or Hard multipliers.
- Mobile Quality of Life: Pushed major scaling updates, including a custom iOS fullscreen fallback, a dedicated fullscreen toggle button, and landscape layout optimizations for smaller screens.
- Level Polish: Improved exit portal mechanics and animations.
- Asset Maintenance: Updated the dynamic player face HUD assets and refactored overall button CSS styling.

**March 24, 2026**
- Gameplay: Added Boss health bars, difficulty selection, second boss phase and "Fish Eye" effects.
- Fixes: Improved portal animations and patched Sugar Sanctuary.
- Mobile/UI: Implemented iOS fullscreen fallback, added Pause/Fullscreen buttons, and optimized the Landscape start menu.
- Visuals: Updated player face assets and refined button styles.

**March 23, 2026**
- Architecture: Major refactor of HTML/CSS for improved layout stability.
- Responsiveness: Enhanced mobile viewport settings and refined landscape orientation for better button access.
- Assets: Added initial portal assets and visibility controls.
- UI: Streamlined overlays and global UI styles in index.html.

**March 22, 2026**  
- Added virtual joystick & D-pad (major mobile/desktop control upgrade)  
- Audio enhancements and performance optimizations  
- Refined start menu, buttons, and overall UI styling  
- Added wall textures + updated maps/levels  
- Improved enemy behavior, level transitions, and progression  
- Added Face HUD and integrated plushie/boss assets  
- Added share button + extensive CSS refactoring  
- Enhanced SEO, social meta tags, and button polish  

**March 21, 2026**  
- Project launch with core engine  
- Created and expanded detailed README.md  

**Status:** 119 commits in 5 days. All logic lives in one `index.html` file.
