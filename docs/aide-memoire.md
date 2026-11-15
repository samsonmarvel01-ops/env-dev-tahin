# Aide-mémoire du terminal Linux

## les premières commandes

| Commande | Ce qu'elle fait               | Exemple        |
| -------- | ----------------------------- | -------------- |
| `whoami` | affiche le nom d'utilisateur  | `whoami`       |
| `clear`  | efface l'ecran                | `clear`        |
| `ls`     | affiche le contenu du dossier | `ls docs`      |
| `echo`   | affiche un text               | `echo bonjour` |

## Se déplacer

| Commande | Ce qu'elle fait               | Exemple                |
| -------- | ----------------------------- | ---------------------- |
| `pwd`    | Affiche le dossier ou je suis | `pwd`                  |
| `cd`     | Change de dossier             | `cd ~/dev`             |
| `mv`     | deplace un fichier            | `mv note.txt archive/` |

## Fichiers et dossiers

| Commande | Ce qu'elle fait     | Exemple          |
| -------- | ------------------- | ---------------- |
| `cp`     | Copie un fichier    | `cp a.txt b.txt` |
| `mkdir`  | creer un dossier    | `mkdir photo`    |
| `rm`     | supprime un fichier | `rn note.txt`    |
| `touch`  | cree un fichier     | `touch life.txt` |

## Lire et chercher

| Commande | Ce qu'elle fait                  | Exemple                  |
| -------- | -------------------------------- | ------------------------ |
| `cat`    | affiche tout le fichier          | cat notes.txt            |
| `grep`   | recherche un mot dans un fichier | `grep ERROR app.log`     |
| `less`   | affiche le fichier page par page | `less unit.txt`          |
| `head`   | affiche les premiere ligne       | `head note.txt`          |
| `tail`   | affiche les derniere ligne       | `tail note.txt`          |
| `find`   | retrouve un fichier par son nom  | `lind . -name "facture"` |

## Branch

| Commande     | Ce qu'elle fait                                   | Exemple                       |
| ------------ | ------------------------------------------------- | ----------------------------- |
| `git branch` | liste les branche de mon depot                    | `git branch`                  |
| `git switch` | creer une nouvelle branch et se positionne dessus | `git switch -c ajout-section` |
| `git merge`  | fusionne une branch a la branch ou vous etes      | `git merge ajout-section`     |
