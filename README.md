# RoboRapture: Audio System Design
 
Design documentation for the core audio system of **RoboRapture**, a turned-based strategy video game built in Unity with C#.

I was the **Team Lead and Audio Programmer**, responsible for the audio architecture, memory optimization, debugging tools and version-control workflow for the team. A secondary responsibility in this project (I volunteered) was the musical composition of a full soundtrack and dynamic system design.
 
> **About this repository:** The game's source code and Unity project are under NDA and are not included. This repository contains my own design documentation, with game-specific content removed, and the scripts I was cleared to share.
 
## At a glance
 
| | |
| --- | --- |
| **Role** | Team Lead, Audio Programmer, Music Composer, Music System Architect |
| **Year** | 2025 |
| **Location** | Vancouver, Canada |
| **Engine, middleware and language** | Unity, Wwise, C# |
| **Tools** | Git, SourceTree, Google Sheets + Apps Script, Wwise, Visual Studio (C#), PyWwise |
| **Status** | Non-public release (School owns rights) -> Availabe only for current and past students or collaborators |
 
## What I built
 
- **Core audio system in C#.** Created the core scripts running the game's audio: WwiseMenuManager and WwiseTurnManager, both in C#
- **Music creation and implementation.** Composed the full soundtrack for the game, implemented through wwise behaviors interacting with the audio managers; achieved a dynamic music system that played differently depending on turns, bosses, menus, etc.
- **Memory optimization.** Handled optimization by asset handling: trimming silences in audio files; bouncing variations into a single file, using trimming to handle one asset instead of multiples; reduced sample rate on low-frequency asssets. Used hash maps and dynamic programming algorithms wihin the codes to reduce times.
- **Debugging tools.** Created and implemented a C# script that let developers use numpad to spawn enemies, bosses, change wwise states, etc. Created a type-check and naming convention-check for assets (in Python).
- **Production tracking.** A ticketing and team-tracking system in Google Sheets with Google Apps Script, used to track 1,000+ assets.
- **Version control.** I managed the Git workflow in Sourcetree, including merge conflicts and pull requests.

## Documentation
 
| Document | What it covers |
| --- | --- |
| [Architecture](architecture.md) | The layers of the audio system, how data flows between them, and why |
| [Memory and loading](memory-and-loading.md) | Loading strategy per sound type, what was measured, what changed |
| [Debugging tools](debugging-tools.md) | What each tool showed and how the team used it |
| [General Overview](RoboRapture-Presentation.pdf) | Initial presentation used to pitch audio vision to devs |
