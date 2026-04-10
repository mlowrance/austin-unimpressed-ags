# Project: Austin Unimpressed

## 1. Overview
A narrative-driven, satirical "boss rush" adventure built in Adventure Game Studio (AGS). The game follows Austin as he walks through life's mundane hurdles, remains perpetually unimpressed, and chases a retirement dream that is ultimately crushed by the housing market.

## 2. Technical Strategy
* **Engine:** AGS 3.6.1+ (High-Resolution 32-bit color).
* **Resolution:** 1280x720 (16:9 widescreen).
* **Control Scheme:** Keyboard-only (Space to start/interact, Right Arrow to move).
* **Deployment Target:** Windows (Native) and Web (WASM via GitHub Actions).

## 3. The "Unimpressed" Task List

| Status | Task | Type | Implementer |
| :--- | :--- | :--- | :--- |
| 🟢 | **1. Project Initialization** | Editor | Human |
| ⚪ | **2. Splash Screen:** "Press Space to Start" logic | Script | AI |
| ⚪ | **3. Austin Sprite:** Import high-res head/body | Editor | Human |
| ⚪ | **4. Character Setup:** Configure walk cycles/view | Editor | Pair |
| ⚪ | **5. Movement Engine:** Limit controls to Right Arrow | Script | AI |
| ⚪ | **6. UI:** Create the "Retirement Bar" GUI | Editor | Human |
| ⚪ | **7. Boss 1:** Huey Mango’s Chicken Strips encounter | Script | Pair |
| ⚪ | **8. Boss 2:** The "Mega PR" encounter | Script | Pair |
| ⚪ | **9. Boss 3:** [TBD] Final obstacle | Script | Pair |
| ⚪ | **10. The 4th Wall:** "Unimpressed" speech bubble | Script | AI |
| ⚪ | **11. The Ending:** Money pile + Awooga animation | Editor | Human |
| ⚪ | **12. The Twist:** Falling House & Game Over | Script | Pair |
| 🟢 | **13. CI/CD:** GitHub Action for Web Deployment | DevOps | AI |

## 4. Game Design Specifications

### Character: Austin
* **Visuals:** Standard 16-bit body proportions with an oversized head to emphasize facial expressions.
* **Attire:** Royal blue t-shirt, dark trousers.
* **Animations:** * Walk Right (Looping)
    * Idle/Turning to Camera (For boss encounters)
    * "Awooga" (Eyes out, mouth open - Ending only)

### Gameplay Mechanics
* **The Retirement Bar:** A GUI element at the top of the screen. Its width is tied to a Global Variable `RetirementProgress`.
* **Boss Battles:** Scripted trigger points where movement locks, Austin breaks the 4th wall, and says "Unimpressed."

## 5. Guidelines for AI Collaborators
* **Syntax:** Use AGS Script (C-style).
* **Modular Logic:** Keep room-specific triggers in `roomX.asc` and global game-state logic in `GlobalScript.asc`.
* **Asset References:** High-res source PNGs are located in the `/Assets` folder.