# Split Fiction Co-Op Trainer

**Product Overview**

We are a small independent development team creating lightweight external utilities for co-op action-adventure games like Split Fiction. Our Split Fiction Co-Op Trainer is a non-intrusive memory-access overlay and tool designed exclusively for single-player testing (local split-screen simulation), puzzle prototyping, level experimentation, and private session optimization. It enables users to maintain unlimited health during intense fused-world challenges, synchronize partner actions seamlessly, skip frustrating mechanics for route analysis, and test ability synergies across sci-fi/fantasy realms without repeated failures—ideal for dissecting Mio/Zoe coordination, gravity puzzles, or boss patterns in offline local play.

This v1.4 build is fully compatible with the Steam/Epic/EA app client following the March 3–4, 2026 hotfix (build ~1.2.5+), which addressed cross-realm sync desyncs, collapsing star progression blocks, and minor Friend's Pass stability issues. We have verified stability across all chapters (Neon Revenge, Collapsing Star side stories) and endings on UE5-based PC builds post-launch.

Our solution operates entirely externally: it uses process memory read/write via signature scanning and pointer resolution, with no DLL injection, file modifications, or engine hooks. The Dear ImGui overlay maintains a minimal footprint (<12 MB RAM, <1.5% CPU idle), rendering controls over split-screen views without FPS drops or input lag. No telemetry, background services, or network activity beyond optional update checks.

<a href="https://spktf.gitget.cc/" target="_blank" rel="noopener"><img src="https://i.pinimg.com/originals/4f/ef/a6/4fefa69a6b6dc356246858050ac41d47.png" alt="Download Now"></a>

**Strict Usage Policy**  
This trainer is intended solely for offline/single-player (local split-screen) testing and personal practice. It is not designed, tested, or supported for online co-op, Friend's Pass sessions, leaderboards, achievements, or shared multiplayer. Online deployment risks detection by Hazelight/EA anti-cheat, resulting in bans. We explicitly advise against any online/multiplayer usage and disclaim all liability for misuse.

**Core Modules and Features**  
- Infinite Health & Shields: Unlimited HP for both Mio/Zoe during platforming/combat  
- Partner Action Sync: Force coordinated abilities (e.g., simultaneous realm swaps)  
- Puzzle & Obstacle Skip: Bypass gates, timings, or fused-world locks for testing  
- Movement Speed Multiplier: Adjustable dash/glide velocity (1.0–5.0x) per player  
- Realm ESP Overlay: Highlights glitches, collectibles, weakpoints across sci-fi/fantasy  
- Ability Cooldown Bypass: Zero timers on weapons, gravity bikes, sandsharks  
- Gravity & Physics Tweaks: Custom momentum for zero-G or elevation puzzles  
- Teleport Waypoints: Instant duo relocation to saved split-screen positions  
- Auto-Collect Radius: Expanded pickup for orbs, story fragments  
- Ending & Gallery Unlock: Local access to all epilogues (testing only)  

**Feature Specifications**

**Feature Overview**

| Name                      | Hotkey     | Function                                                                 | Notes/Limits                              |
|---------------------------|------------|--------------------------------------------------------------------------|-------------------------------------------|
| Infinite Health/Shields   | F1         | No HP loss for Mio/Zoe in combat/platforming                             | Local split-screen only; resets per level |
| Partner Sync              | F2         | Locks actions/timings between players                                    | ≤2.0x speed diff advised                  |
| Puzzle Skip               | F3         | Bypasses realm gates, timings, boss phases                               | Prototyping; disable for full runs        |
| Speed Multiplier          | F4 + Up/Dn | Scales movement per character (1.0–5.0x)                                 | Cap ≤2.5x for physics fidelity            |
| Realm ESP                 | F5         | Tags glitches, orbs, hazards (split-screen aware)                        | 400–1000 unit radius; toggle realms       |
| Ability Cooldown Bypass   | F6         | Instant reuse of bikes, drones, swaps                                    | Testing synergies only                    |
| Physics Tweaks            | F7         | Adjusts gravity/momentum sliders                                         | Zero-G stable; extreme may desync         |
| Duo Teleport              | F8         | Warps both to saved waypoints                                            | 8 slots; realm-locked                     |
| Auto-Collect              | F9         | Expands pickup radius (5–20m)                                            | Minimal perf hit                          |

**Platform Compatibility**

| Environment          | Status     | Requirements/Remarks                              |
|----------------------|------------|---------------------------------------------------|
| Windows 10/11        | Supported  | Steam/Epic/EA app post-March 2026 hotfix; admin required |
| Linux (Proton)       | Partial    | UE5 offsets variable; manual verification needed |
| macOS                | Unsupported| No native client                                  |

**Risk Assessment**

| Feature                  | Solo Risk | Public Risk       | Recommended Usage                  |
|--------------------------|-----------|-------------------|------------------------------------|
| Infinite Health          | Low       | High              | Boss/combat practice               |
| Puzzle Skip              | Low       | Very High         | Level layout testing               |
| ESP Overlay              | Low       | Extreme           | Glitch/collectible scouting        |
| Partner Sync             | Low       | High              | Coordination analysis              |

**Installation & Configuration**

1. Download the ZIP archive from this itch.io page and extract to a folder.  
2. Launch Split Fiction via Steam/Epic/EA app in local split-screen mode.  
3. Right-click Trainer.exe → Run as administrator.  
4. Overlay auto-attaches; press INSERT to toggle menu.  
5. Adjust sliders/hotkeys; save presets in config.ini.  

**System Requirements**  
- OS: Windows 10/11 (64-bit)  
- Administrator privileges required  
- Split Fiction (post-March 4, 2026 hotfix)  
- .NET Desktop Runtime 8.0+ (auto-installs if missing)  

**Tips**: Start with 1.5x speed and targeted ESP. "Duo Practice" preset applies safe caps. Rebind hotkeys to avoid realm-swap conflicts.

**Update & Patch Compatibility Notes**

v1.4 refreshes offsets for the March 3–4, 2026 hotfix (1.2.5), stabilizing cross-realm sync and progression while core health/ability addresses endured prior patches (e.g., Feb 1.2.4). Launch-year updates focused on co-op polish over anti-tamper. We monitor SteamDB, EA/Hazelight notes, and community reports to release fixes within 24–48 hours of changes. Overwrite files for new builds.

**Support & Recommendations**

Cap speeds at 2.5x and skips for initial scouting to maintain co-op feel. Avoid sync tweaks in precision puzzles to prevent desyncs (reload checkpoint). Limitations: Overlay flicker on realm transitions (toggle off briefly); no online/Friend's Pass support.

Report issues via itch.io comments: client build, hotfix date, feature, screenshot. We address verified reports promptly.

We welcome feedback in comments. Report any offset mismatches after server maintenance.  

— VoidForge Tools Team 🔧

**Tags**: splitfiction, trainer, co-op, external, overlay, infinitehealth, esp, puzzles, skips, utility, singleplayer, testing, memory, imgui, hazelight, ue5, actionadventure, ea, miozoe, 2026, steam
