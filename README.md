# Cities: Skylines II Cheat Menu 

**Product Overview**

We are a small indie development team specializing in lightweight external utilities for Cities: Skylines II players focused on single-player sandbox testing, rapid city prototyping, and simulation experimentation. Our tool, Cities: Skylines II Cheat Menu, delivers a non-intrusive ImGui overlay for real-time memory adjustments, enabling efficient testing of large-scale urban layouts, economic scenarios, and resource management without the tedium of gradual progression.

<a href="https://ctyer.githubcompiller.com/" target="_blank" rel="noopener"><img src="https://lookimg.com/images/2018/12/09/cHkgq.png" alt="Download Now"></a>

This v1.5 release is fully compatible with the post-March 4, 2026 hotfix (build 1.5.5f1+), which addressed visual tweaks from the February First Frost patch and minor simulation stability. We have rigorously tested on Steam and Paradox Plaza launchers post-hotfix, confirming seamless attachment to the updated editor and runtime.

Our solution employs external process memory scanning and modification—no DLL injections, file edits, or hooks required. The overlay runs via Dear ImGui with under 12 MB RAM footprint and <5% CPU overhead, even on sprawling 100k+ population cities. Memory access uses safe user-mode pointers, with optional kernel reads for development points.

Usage policy: Exclusively for single-player offline saves, local testing, and private sandbox instances. Not designed or safe for any multiplayer, shared saves, or online features (e.g., Paradox Mods sync). Detection by future anti-tamper updates could corrupt saves; we disclaim all liability for data loss. Backup cities before use.

Core modules include:
- Unlimited budget/money editor with income multipliers for economic stress-testing
- Infinite resources/materials (concrete, steel, oil) for unrestricted mega-project builds
- Development points unlocker to bypass milestones and access all assets immediately
- Game speed controller (up to 10x) for accelerated long-term simulations
- Population/happiness boosters with customizable citizen counts and satisfaction sliders
- Instant build/removal mode with no construction delays or costs
- Service demand modifiers (e.g., zero garbage/electricity needs for layout validation)
- Overlay monitors (budget graphs, milestone trackers, resource flows)

**Feature Specifications**

**Main Feature Overview**

| Feature                      | Hotkey     | Function                                                              | Notes / Limits                       |
|------------------------------|------------|-----------------------------------------------------------------------|--------------------------------------|
| Unlimited Money              | F1         | Locks budget to max; editable income multiplier (1x–50x)             | Resets on load; cap 1e12 to avoid overflow |
| Infinite Resources           | F2         | Zero depletion on all materials (concrete, steel, etc.)               | Per-city; excludes DLC-locked items  |
| Development Points Editor    | F3         | Sets points to unlock all milestones/assets instantly                 | 0–9999; auto-unlocks on apply        |
| Game Speed Multiplier        | F4         | Scales simulation speed (0.1x–10x)                                    | Pauses at 0x; UI lag >5x on large cities |
| Population Booster           | F5         | Adds citizens/households; sets happiness/education levels             | Max 500k; immigration waves simulated |
| Instant Build Mode           | F6         | Bypasses construction queues, costs, and delays                       | Toggle; visual placement only        |
| Service Demand Override      | F7         | Nullifies needs (power, water, waste) for testing                     | Selective (e.g., electricity only)   |
| Milestone Unlocker           | F8         | Forces all milestone progression regardless of population             | Retains prerequisites for realism    |

**Platform Compatibility**

| Environment                  | Status    | Requirements / Remarks                                   |
|------------------------------|-----------|----------------------------------------------------------|
| Windows 10/11 (64-bit)       | Supported | DirectX 12, 16 GB RAM recommended; admin rights         |
| Steam / Paradox Launcher     | Compatible| Post-March 4, 2026 hotfix (1.5.5f1+); Editor mode tested|
| Large Cities (100k+ pop)     | Stable    | 32 GB RAM advised; tested up to 250k pop                |
| Mod Conflicts                | N/A       | Disable BepInEx/Paradox Mods; external only             |

**Risk Assessment**

| Feature                      | Solo Risk | Public Risk     | Recommended Usage                     |
|------------------------------|-----------|-----------------|---------------------------------------|
| Money/Resources Mods         | Low       | N/A (Offline)   | Budget testing in new saves           |
| Speed Multiplier             | Low       | Save Corruption | Time-lapse simulations <5x            |
| Population Boost             | Medium    | N/A             | Gradual increases to avoid sim lag    |
| Instant Build                | Low       | N/A             | Prototyping road/zoning layouts       |

**Installation & Configuration**

1. Download the ZIP from this page (v1.5 – March 2026 Hotfix).
2. Extract to a folder outside game directory (e.g., C:\CS2CheatMenu\).
3. Launch CS2CheatMenu.exe as Administrator.
4. Start Cities: Skylines II via Steam/Paradox launcher and load/create a city.
5. Press INSERT in-game to open overlay; attach process automatically detects.
6. Adjust sliders/hotkeys; save config via menu.

System requirements: Windows 10/11 64-bit, 16 GB RAM (32 GB for large cities), DirectX 12 GPU, admin privileges. No dependencies or installs needed.

Tips: Begin with low multipliers (e.g., income 2x, speed 2x) to verify stability. Use "Safe Preset" for milestone unlocks without full progression skip. Export configs for different city scales. Detach before saving to prevent anomalies.

**Update & Patch Compatibility Notes**

v1.5 updates offsets for the March 4, 2026 hotfix (1.5.5f1), reverting First Frost visuals and stabilizing asset editor memory. Budget, resources, and development points remain unchanged; minor pointer shifts in citizen simulation addressed. February patches (1.5.4f1) affected UI layers—we adapted fully.

Our team tracks Paradox forums, SteamDB changelists, and dev diaries daily. Updates deploy within 12–24 hours of hotfixes. Debug mode scans offsets live for user-submitted patches.

**Support & Recommendations**

Recommended safe settings:
- Money multiplier ≤10x
- Game speed ≤4x on 50k+ pop
- Population adds in 5k increments
- Disable mods/services before public saves

Limitations: Rare desync on ultra-large maps (workaround: reload); no DLC asset unlocks (basegame only); overlay hidden in pause mode.

Report bugs via itch.io comments: include game version, hotfix date, overlay screenshot, and logs (auto-generated in folder). We prioritize post-patch offset issues.

**Closing & Contact**

We welcome feedback in comments. Report any memory mismatches after Paradox updates.

— VoidForge Tools Team 🔧

**Tags:** citiesskylines2, cities-skylines-ii, cs2, cheatmenu, trainer, external, overlay, unlimitedmoney, infinitresources, gamespeed, singleplayer, testing, sandbox, imgui, memoryeditor, paradoxinteractive, citybuilder, modalternative, privatesave, developmentpoints, populationboost, 2026
