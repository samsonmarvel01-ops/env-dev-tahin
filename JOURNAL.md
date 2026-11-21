# Journal des choix

## 2026-11-11 – Installation de Node.js

- **Décision :** installer Node.js avec le gestionnaire de paquet 'apt' en mode administrateur avec 'sudo'
- **Autres possibilités :** le paquet nodejs d'Ubuntu, le site nodejs.org.
- **Raison :** NodeSource donne la version LTS récente, et les commandes
  peuvent être écrites dans mon README pour être refaites à l'identique.

  ## 2026-11-11 - systeme pour le terminal

- **Décision :** installer Ubuntu dans le terminal en mode administrateur avec 'wsl'.
- **Autres possibilités :** le dual-boot (double démarage), machine virtuelle
- **Raison :** Pour redonner vie a un viel ordinateur ou pour quitter les écosystemes propriétaires

## 2026-11-13 - Hebergement du dépot : GitHub

- **Décision :** publier notre depot local sur un depot distant 'github'
- **Autres possibilités :** neant
- **Raison :**GitHub se distingue par sa capacité à héberger des ligne de code
  permettant aux developpeurs de partager et d'ameliorer le code ensemble

## Travailler avec des branches

**Décision :** Je crée une branche pour chaque nouvelle modification, puis je la fusionne dans main quand le travail est terminé et vérifié.

**Autres possibilités :**

- Tout modifier directement sur main, sans créer de branche.(mais c'est tres déconseillé)
- Copier le dossier du projet à chaque essai (env-dev-kone-v2, env-dev-kone-final...)

**Raison :** main est la « copie propre » du projet : elle doit toujours fonctionner. Une branche, c'est le brouillon : je peux essayer, me tromper et faire plusieurs commits sans risquer de casser ce qui marche.
