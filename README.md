<p align="center"><img src="icon.png" width="96" height="96" alt="Paginel"></p>

# Paginel Text

**The word processor that complements Word and Google Docs, or replaces them.** Your `.docx` files stay `.docx` files;
your AI agents write in them too. Made in France — [paginel.com](https://paginel.com).

This repository publishes the **installers** of the Paginel Text desktop app (macOS, Windows, Linux) and news about
Paginel. The source code is not public.

## Download

**[Latest release](https://github.com/paginel/paginel-text/releases/latest)** — also on
[paginel.com/en/download](https://paginel.com/en/download/).

| System | File |
|---|---|
| macOS 12 or later, Mac with Apple silicon (M1 and later) | `Paginel_<version>_aarch64.dmg` |
| Windows 10 and 11, 64-bit (installs for you alone, no administrator rights) | `Paginel_<version>_x64-setup.exe` |
| Linux x86_64, recent distribution (built on Ubuntu 22.04) | `Paginel_<version>_amd64.AppImage` or `.deb` |

`SHA256SUMS.txt` lists the checksum of each file. Once installed, the app updates itself from paginel.com; every update
is signed and verified by the app.

## What it does

- Opens, edits and saves your `.docx` and Markdown files, where they are.
- Four views, in the order of the work: **Markdown**, **Web**, **Edit** and **PDF**.
- Works with no network: nothing essential is online.
- Exports to PDF, with the pages you see in the PDF view.
- Lets an AI model running on your computer (Ollama, through MCP) read, complete and comment a document; what it writes
  is signed with its name and can be undone.
- Also opens shared documents: **File › Sync with Paginel…** puts a copy online to write together, with a free Paginel
  account.

The app is free and opens right away, with no account.

## The first time you open it

During the beta, the app is signed by neither Apple nor Microsoft, so your system warns you once.

- **macOS**: open the disk image, drag *Paginel Text* to Applications, then in Terminal:
  ```sh
  xattr -cr "/Applications/Paginel Text.app"
  open "/Applications/Paginel Text.app"
  ```
  Or right-click the app › *Open* › *Open* (or *System Settings › Privacy & Security › Open Anyway*).
- **Windows**: SmartScreen shows “Windows protected your PC”: click *More info*, then *Run anyway*.
- **Linux**: AppImage: `chmod +x Paginel_*.AppImage` then run it. Package: `sudo apt install ./Paginel_*_amd64.deb`.

## Also

- **VS Code**: the [Paginel Text extension](https://marketplace.visualstudio.com/items?itemName=paginel.paginel-text).
- **Orca**: the Paginel Text plugin, from [our Orca catalog](https://github.com/paginel/orca-plugins).
- Contact: hello@paginel.com.

## License

Free to download and use; proprietary software, all rights reserved: see [LICENSE](LICENSE). The third-party components
the app includes keep their own licenses (*Help › Licenses…* in the app).

---

# Paginel Text (français)

**Le traitement de texte qui complète Word et Google Docs, ou les remplace.** Vos `.docx` restent des `.docx` ; vos
agents d'IA y écrivent aussi. Fait en France — [paginel.com](https://paginel.com).

Ce dépôt publie les **installateurs** de l'application de bureau Paginel Text (macOS, Windows, Linux) et les nouvelles de
Paginel. Le code source n'est pas public.

**Télécharger** : [la dernière version](https://github.com/paginel/paginel-text/releases/latest), aussi sur
[paginel.com/telecharger](https://paginel.com/telecharger/). Mac à puce Apple (macOS 12 ou plus récent) : `.dmg` ;
Windows 10 et 11, 64 bits : `_x64-setup.exe` ; Linux x86_64 : `.AppImage` ou `.deb`. `SHA256SUMS.txt` donne l'empreinte
de chaque fichier. Une fois installée, l'application se met à jour depuis paginel.com (mises à jour signées, vérifiées).

**Ce qu'elle fait** : ouvre, modifie et enregistre vos `.docx` et vos Markdown, là où ils sont ; quatre vues
(**Markdown**, **Web**, **Édition**, **PDF**) ; fonctionne sans réseau ; exporte en PDF ; un modèle d'IA de votre
ordinateur (Ollama, par MCP) peut lire, compléter et commenter un document ; **Fichier › Synchroniser avec Paginel…** met
une copie en ligne pour écrire à plusieurs, avec un compte Paginel gratuit. L'application est gratuite et s'ouvre
aussitôt, sans compte.

**À la première ouverture** (pendant la bêta, l'application n'est signée ni par Apple ni par Microsoft) :
- **macOS** : ouvrez l'image disque, glissez *Paginel Text* dans Applications, puis dans le Terminal :
  `xattr -cr "/Applications/Paginel Text.app"` et `open "/Applications/Paginel Text.app"` ; ou clic droit › *Ouvrir* ›
  *Ouvrir*.
- **Windows** : « Windows a protégé votre PC » : *Informations complémentaires*, puis *Exécuter quand même*.
- **Linux** : `chmod +x Paginel_*.AppImage` puis lancez-la ; ou `sudo apt install ./Paginel_*_amd64.deb`.

**Aussi** : l'[extension VS Code](https://marketplace.visualstudio.com/items?itemName=paginel.paginel-text), le plugin
Orca depuis [notre catalogue](https://github.com/paginel/orca-plugins). Contact : hello@paginel.com.

**Licence** : gratuite, logiciel propriétaire, tous droits réservés : voir [LICENSE](LICENSE).
