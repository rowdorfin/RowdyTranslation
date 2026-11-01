<p align="center">
  <img src="images/banner.jpg" alt="Fan Translation Project by Rowdorf" width="480">
</p>

# RowdyTranslation v1.0 — Sword Art Online: Infinity Moment (PSP) in English and Português (BR)

**Fan Translation Project by Rowdorf**

<p align="center">
  <img src="images/title-screen.jpg" alt="Title screen" width="49%">
  <img src="images/battle2.jpg" alt="Battle" width="49%">
</p>
<p align="center">
  <img src="images/field.jpg" alt="Field messages" width="49%">
  <img src="images/main-menu.jpg" alt="Main menu and status" width="49%">
</p>
<p align="center">
  <img src="images/battle.jpg" alt="Battle" width="49%">
</p>

A fan translation of *Sword Art Online: Infinity Moment* (PSP, Japan, NPJH50701) into **English** and
**Brazilian Portuguese**. It is distributed **only as a patcher**: you need your own Japanese ISO. **This project
does not distribute the game or any game files.** Please buy the original game.

*Português (BR): veja a seção [Em português](#em-português).*

## Download
Get the package for your system from the [Releases](https://github.com/rowdorfin/RowdyTranslation/releases) page.
This repository and its releases are the **only** official distribution; any other copy may be modified.

| system | file |
|---|---|
| Windows 10/11 | `RowdyTranslationV1.0.zip` (window, nothing to install) |
| Linux (x64 / ARM64) | `RowdyTranslationV1.0-linux.tar.gz` (terminal) |
| macOS (Intel / Apple Silicon) | `RowdyTranslationV1.0-macos.zip` (terminal) |

Both languages are inside every package; you pick one when patching.

## Requirements
- Your original, unmodified Japanese ISO:

| field | expected value |
|---|---|
| game | Sword Art Online: Infinity Moment (PSP, Japan) |
| ID | NPJH-50701 (v1.00) |
| size | 1,200,226,304 bytes |
| SHA-256 | `c8797943ee17f0b2b8e8b8bffdfd1189c75a569c90c5eed62722901d95f95ac4` |

- About 1.4 GB free where the translated ISO is saved. Works offline.
- To play: a PSP with custom firmware (ARK-4, PRO or ME) or the PPSSPP emulator.

## How to use
**Windows**
1. Extract the `.zip` and run **RowdyTranslationV1.0.exe**.
2. Pick the language at the top: **English** or **Português (BR)**.
3. **Select ISO...** → your original Japanese ISO. **Choose destination...** → where to save.
4. Click **Install English translation** and wait a few minutes. The new ISO is verified by SHA-256; your original
   ISO is never modified. To have both languages, run it twice and save two ISOs.

**Linux / macOS** (terminal)
```
./RowdyTranslationV1.0-linux-x64
```
It asks for the language and the files (you can drag the ISO into the terminal). Or directly:
`./RowdyTranslationV1.0-linux-x64 --lang en original.iso SAO_IM_EN_v1.0.iso`. On a Mac the file is
`RowdyTranslationV1.0`; it is not notarized by Apple, so run `xattr -d com.apple.quarantine RowdyTranslationV1.0`
once (and `chmod +x RowdyTranslationV1.0` if it says "permission denied"). See the README inside each package.

## Verifying the download
The programs are **not digitally signed**, so Windows SmartScreen/Defender or macOS Gatekeeper may warn about them.
Compare the SHA-256 with `SHA256SUMS-release.txt` on the release page:
```
certutil -hashfile RowdyTranslationV1.0.exe SHA256
```

## Troubleshooting
| message | what to do |
|---|---|
| "not an ISO image" | Select the Japanese ISO (NPJH50701). CSO/ZIP/7z are not accepted: extract first. |
| "different SHA-256" / "size ... expected ..." | Your ISO is modified or a different dump/version (e.g. an already translated ISO). Use a clean dump. |
| "Not enough space" | Free about 1.4 GB or pick another drive. |
| "No permission to write" | Pick a folder of your own (Documents, Desktop), not `C:\Windows` or `Program Files`. |
| "patch data is corrupted" | Download the package again and check the hash. |
| Old/Japanese text or the other language in the game | If you used the game's **Data Install** before, delete the old install data (`PSP/SAVEDATA/NPJH50701INSTALL`) and install again. Saves can stay. |
| Anything else | Attach the log to an Issue: Windows `%LOCALAPPDATA%\RowdyTranslation\RowdyTranslation.log` (**Open log** button), Linux `~/.cache/RowdyTranslation/RowdyTranslation.log`. |

The translated game needs custom firmware or PPSSPP; it does not run on a PSP without CFW.

## What's new in v1.0
- New **Brazilian Portuguese** translation, alongside English.
- Movie subtitles drawn by the game itself (original videos untouched).
- Many in-game fixes from testing on PSP and PPSSPP: menus, buttons, shop/blacksmith labels, partner speech bubbles
  (no longer cut at 19 characters), boss result screen, system dialogs.
- Patchers for Windows, Linux and macOS; translated ISO is now ~1.3 GB (was ~2.2 GB).

Full list in the [CHANGELOG](CHANGELOG.md).

## Known issues (v1.0)
- Text drawn inside the videos (the character registration box, the boss room sign) stays Japanese.
- The title logo is kept as the original Japanese artwork.
- Some menu labels are abbreviated to fit fixed-size fields (e.g. "2HSwd", "Kat.", "1H Sword").
- The Linux ARM64 build has not been tested on real hardware.

## Help improve the translation!
If you play through the game, please report untranslated text, awkward translations, text overflow, or unexpected
behavior in [Issues](https://github.com/rowdorfin/RowdyTranslation/issues). Screenshots and the exact location
(floor, area, menu or event) are especially helpful. Every report helps make the next release better!

## Support Rowdorf
Enjoying this project? You can support my translation work and future fan projects through voluntary donations.

☕ [**Support Rowdorf on Ko-fi**](https://ko-fi.com/rowdorf)

Have an idea for a new project or a game you'd love to see translated? Leave a donation with a message, or share it
through [GitHub Issues](https://github.com/rowdorfin/RowdyTranslation/issues). Donations are completely optional.

## Em português
Tradução de fã de *Sword Art Online: Infinity Moment* (PSP) para **português do Brasil** (e inglês). Só o patcher é
distribuído: você precisa da sua própria ISO japonesa original (tabela acima). Nenhum arquivo do jogo é distribuído.

1. Baixe o pacote do seu sistema em [Releases](https://github.com/rowdorfin/RowdyTranslation/releases).
2. Windows: rode `RowdyTranslationV1.0.exe`, escolha **Português (BR)** no topo (a janela passa para português),
   selecione a ISO japonesa, escolha onde salvar (~1,4 GB livres) e clique em **Instalar tradução em português**.
   Linux/macOS: no terminal, `./RowdyTranslationV1.0-linux-x64 --lang pt original.iso SAO_IM_PT_v1.0.iso`
   (ou rode sem argumentos e responda às perguntas). No Mac o arquivo é `RowdyTranslationV1.0`; veja o README do zip.
3. A ISO original nunca é alterada; a nova é conferida por SHA-256. Para jogar: PSP com CFW ou PPSSPP.
4. Se o jogo mostrar texto antigo ou o outro idioma: apague `PSP/SAVEDATA/NPJH50701INSTALL` e instale de novo.

Tradução gratuita, **proibida a venda** do patcher, da tradução ou de ISO traduzida. Distribuição oficial só por
este repositório. Problemas: [Issues](https://github.com/rowdorfin/RowdyTranslation/issues).

## Credits
- Translation (English and Brazilian Portuguese), patch and patcher: **Rowdorf** (with AI assistance).
- References consulted: the official English localization of *SAO: Hollow Fragment* (terminology);
  **HoaiTrung97**'s earlier English fan translation; the hatsunumike.blogspot.com floor guides (area names).
- *Sword Art Online* © Reki Kawahara / KADOKAWA / SAO Project; game © BANDAI NAMCO Games. Non-profit fan project,
  not affiliated with the rights holders.

## License
**All rights reserved.** See [LICENSE](LICENSE). Redistribution, modification, extraction or reuse of the
translation, patch or patcher, in whole or in part, is prohibited without written permission. Selling the patcher,
the translation or a patched ISO is prohibited.
