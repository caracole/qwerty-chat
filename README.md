# QWERTY Cipher

> **Système de chiffrement original basé sur le principe du préfixe aléatoire sur les lignes du clavier QWERTY**  
> *An original encryption system based on the random prefix principle on QWERTY keyboard rows*

[![Version](https://img.shields.io/badge/version-v2026.2-blue?style=flat-square&fontFamily=monospace)](https://caracole.github.io/qwerty-chat/)
[![License](https://img.shields.io/badge/license-GNU_GPL_v3-green?style=flat-square)](LICENSE)
[![DOI](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.19916172-orange?style=flat-square)](https://doi.org/10.5281/zenodo.19916172)

---

## 🌐 Application en ligne

**[https://caracole.github.io/qwerty-chat/](https://caracole.github.io/qwerty-chat/)**

Aucune installation requise. Fonctionne dans tout navigateur moderne, hors ligne, sur mobile et desktop.  
Installable comme application (PWA) sur Android et iOS via "Ajouter à l'écran d'accueil".

---

## 📖 Description

QWERTY Cipher est un système de chiffrement symétrique à deux couches :

**Couche 1 — Préfixe aléatoire QWERTY**  
Chaque lettre est codée par sa position dans sa ligne du clavier, précédée d'une lettre de référence choisie aléatoirement dans cette même ligne. Ce mécanisme produit un encodage non-déterministe : la même lettre donne un code différent à chaque chiffrement, rendant l'analyse fréquentielle impossible.

**Couche 2 — Chiffrement XOR**  
Le code QWERTY est ensuite chiffré par XOR avec une clé secrète partagée, transformant le résultat en hexadécimal opaque.

**Extension originale :**  
Une ligne 4 de voyelles accentuées (Á É Í Ó Ú Ü À È Ì Ò Ù Ï) permet de traiter les langues européennes sans normalisation préalable.

---

## 📁 Fichiers du projet

| Fichier | Description |
|---|---|
| `index.html` | Page À propos — présentation du projet (FR/ES/EN/RU) |
| `cifrador_qwerty.html` | Application principale — Chiffreur / Déchiffreur |
| `guide-utilisation.html` | Guide d'utilisation — Français |
| `guide-utilisation-es.html` | Guide d'utilisation — Español |
| `guide-utilisation-en.html` | Guide d'utilisation — English |
| `manifest.json` | Manifest PWA (installation mobile) |
| `icon.png` | Icône de l'application |
| `LICENSE` | Licence GNU GPL v3 |

---

## 📄 Document académique

L'invention est documentée dans un article académique disponible en trois langues :

| Langue | Format |
|---|---|
| Français | `qwerty_cipher_academic.docx` / `.pdf` |
| English | `qwerty_cipher_english.docx` |
| Español | `qwerty_cipher_espanol.docx` |

**Publication Zenodo (avec DOI permanent) :**  
[https://doi.org/10.5281/zenodo.19916172](https://doi.org/10.5281/zenodo.19916172)

---

## ✨ Fonctionnalités de l'application

- 🔐 Double chiffrement : QWERTY (couche 1) + XOR avec clé secrète (couche 2)
- 🌍 Interface multilingue : Français, Español, English, Русский
- 🎨 5 thèmes visuels : Obsidian, Ocean, Forest, Crimson, Paper
- 📱 PWA installable sur Android et iOS
- 📒 Carnet de contacts avec clés secrètes
- ⌨️ Clavier visuel interactif (référence visuelle)
- 🔑 Générateur de clé cryptographique forte (CSPRNG)
- 📤 Partage direct : WhatsApp, Telegram, Signal, Email
- 🔁 Mode icônes / texte pour les boutons
- 💾 Fonctionne 100% hors ligne, sans serveur

---

## 🔒 Analyse de sécurité (résumé)

| Propriété | César | Vigenère | QWERTY (couche 1) | QWERTY + XOR |
|---|---|---|---|---|
| Analyse fréquentielle | ✗ | ~ | ✓ | ✓ |
| Préfixe aléatoire | ✗ | ✗ | ✓ | ✓ |
| Résistance brute force | ✗ | ~ | ~ | ✓ |

> Pour un usage personnel, une clé de 16 caractères générée aléatoirement offre une résistance pratique satisfaisante.

---

## 🛠️ Travailler sur le projet avec Claude

Pour reprendre le développement dans une nouvelle session Claude :

1. Uploadez les fichiers HTML (`index.html`, `cifrador_qwerty.html`) dans la conversation
2. Décrivez ce que vous souhaitez modifier
3. Claude lit les fichiers et applique les modifications

**Historique des versions :**

| Version | Date | Changements principaux |
|---|---|---|
| v2026.1 | Avril 2026 | Version initiale — chiffreur/déchiffreur, multilingue, PWA, carnet de contacts |
| v2026.2 | Avril 2026 | 5 thèmes visuels, mode icônes, accordéons, boutons Coller/Copier, DOI Zenodo |

---

## 👤 Auteur

**Pierre-Henri Giraud**  
Ingénieur informatique  
📧 [ph.giraud@proton.me](mailto:ph.giraud@proton.me)

*Développé en collaboration avec [Claude](https://claude.ai) (Anthropic)*  
*L'invention du préfixe aléatoire sur les lignes QWERTY est originale et appartient exclusivement à Pierre-Henri Giraud.*

---

## 📜 Licence

Ce projet est distribué sous licence **GNU General Public License v3**.  
Voir le fichier [LICENSE](LICENSE) pour les détails.

© 2026 Pierre-Henri Giraud — Tous droits réservés sur l'invention originale.
