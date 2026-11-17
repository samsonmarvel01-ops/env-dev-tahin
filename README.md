# env-dev-tahin (B1 DEV, IFRAN) - Mon environnement de developpement

environnement de developpement de samuel TAHIN - B1 DEV, IFRAN.

## Mon ordinateur

| Élément    | Valeur         |
| ---------- | -------------- |
| Système    | Windows 10 pro |
| Processeur | Intel Core i7  |
| Mémoire    | 16 Go          |
| Éditeur    | VS Code        |

## Mon Ubuntu

| Élément     | Valeur             |
| ----------- | ------------------ |
| Version     | Ubuntu 26.04.1 LTS |
| Lancé avec  | WSL                |
| Processeurs | 4                  |
| Mémoire     | 7,7 Go             |
| Utilisateur | hpsamuel           |

## Logiciels installés dans Ubuntu

| Logiciel | Version | Commande d'installation                             |
| -------- | ------- | --------------------------------------------------- |
| Git      | 2.53.0  | déjà présent dans Ubuntu                            |
| tree     | 2.3.1   | `sudo apt install -y tree`                          |
| htop     | 3.4.1   | `sudo apt install -y htop`                          |
| nano     | 8-7-1   | `sudo apt install -y nano`                          |
| Node.js  | 22.22.1 | dépôt NodeSource, puis `sudo apt install -y nodejs` |
| npm      | 11.20.0 | installé avec Node.js                               |

## Installation

### 1. Installer Ubuntu et VS Code

- **Windows :** dans le Terminal (administrateur), taper `wsl --install`,
  redémarrer, puis choisir un nom d'utilisateur et un mot de passe Ubuntu.
- **Mac :** installer Homebrew depuis [brew.sh](https://brew.sh), puis taper
  `brew install colima docker`, `colima start` et `colima ssh`.
- Installer VS Code depuis [code.visualstudio.com](https://code.visualstudio.com).

### 2. Installer les outils dans Ubuntu

1. Ouvrir Ubuntu et aller dans le dossier du projet : `cd ~/dev/env-dev-kone`
2. Lancer le script d'installation : `./scripts/installer.sh`

## Vérification

Lancer `./scripts/verifier.sh` dans Ubuntu.
Résultat attendu : une version pour Ubuntu, Git, Node.js, npm et tree.

## Contenu du dossier

| Fichier ou dossier     | Rôle                    |
| ---------------------- | ----------------------- |
| `README.md`            | Cette documentation     |
| `JOURNAL.md`           | Le journal de mes choix |
| `docs/aide-memoire.md` | aide a me souvenir      |
| `scripts/installer.sh` | installer outils        |
| `scripts/verifier.sh`  | verification de poste   |

## Historique

Ce dossier est suivi avec Git depuis le sous-module 2.
