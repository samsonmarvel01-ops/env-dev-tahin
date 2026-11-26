# Fiche réseau

## Mes adresses IP

| Machine                | Adresse IP     | Privée ou publique ? |
| ---------------------- | -------------- | -------------------- |
| Mon Ubuntu             | 172.28.239.16  | privée               |
| Mon ordinateur (Wi-Fi) | 172.16.50.77   | privée               |
| Ma connexion Internet  | 160.120.118.75 | publique             |

## Résultats du DNS

| Nom de domaine  | Adresse IP |
| --------------- | ---------- |
| `github.com`    | …          |
| `wikipedia.org` | …          |

## Les outils réseau

| Commande          | Ce qu'elle fait                    |
| ----------------- | ---------------------------------- |
| `hostname -I`     | Affiche l'adresse IP de mon Ubuntu |
| `ping -c 4 <nom>` | …                                  |
| `nslookup <nom>`  | …                                  |

## Le trajet d'une requête

Quand je tape `https://github.com` dans mon navigateur :

1. l'url
2. le dns
3. la connexion
4. la securité
5. la requete
6. la reponse

## Les codes de réponse HTTP

| Code | Nom                   | Ce qu'il veut dire | Exemple que j'ai vu |
| ---- | --------------------- | ------------------ | ------------------- |
| 200  | OK                    | valide             | …                   |
| 301  | Moved Permanently     | déminagé           | …                   |
| 404  | Not Found             | …                  | …                   |
| 500  | Internal Server Error | …                  | (pas vu)            |
