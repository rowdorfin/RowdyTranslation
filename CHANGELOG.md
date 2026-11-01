# Changelog

## v1.0 — 2026-11-01
- New Brazilian Portuguese translation; both languages ship in one patcher (language picker in the window,
  `--lang en|pt` in the terminal).
- Patchers for Windows (window), Linux x64/ARM64 and macOS Intel/Apple Silicon (terminal). Same checks everywhere:
  original ISO by size and SHA-256 (never modified), translated ISO verified by SHA-256.
- Movie subtitles are drawn by the game over the original videos (no video data in the patch); compatible with
  CWCheat codes.
- Translated ISO is ~1.3 GB (was ~2.2 GB); patches are ~1.7 MB per language.
- Partner speech bubbles no longer cut at 19 characters; long lines shortened to fit.
- Boot notice, system dialogs (install/save), button captions, tabs, FRIEND/OPTION/GUILDS labels, shop and
  blacksmith labels and the boss result screen translated in the images.
- Many text fixes from in-game testing on PSP and PPSSPP (quests, dialogue, menus, shop guide lines that
  overflowed).

## v0.9 beta — 2026-10-26 (first public release, pre-release)
- Complete English translation of the game text (dialogue, menus, items, quests, system messages); terminology
  aligned with the official English *SAO: Hollow Fragment*.
- English textures for area cards, floor titles, Teleport Gate and several menu labels.
- Title screen credit "Fan Translation Project by Rowdorf".
- Windows patcher (no installation, offline): checks the original ISO by size and SHA-256, never modifies it, and
  verifies the translated ISO by SHA-256 before finishing. English interface and log.
- Known issues: see the README.
