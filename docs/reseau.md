# Fiche réseau

## Mes adresses IP

| Machine                | Adresse IP     | Privée ou publique ? |
| ---------------------- | -------------- | -------------------- |
| Mon Ubuntu             | 172.28.239.16  | privée               |
| Mon ordinateur (Wi-Fi) | 172.16.50.77   | privée               |
| Ma connexion Internet  | 160.120.118.75 | publique             |

## Résultats du DNS

| Nom de domaine  | Adresse IP    |
| --------------- | ------------- |
| `github.com`    | 140.82.121.4  |
| `wikipedia.org` | 185.15.59.224 |

## Les outils réseau

| Commande          | Ce qu'elle fait                                             |
| ----------------- | ----------------------------------------------------------- |
| `hostname -I`     | Affiche l'adresse IP de mon Ubuntu                          |
| `ping -c 4 <nom>` | Envoie 4 paquets à la machine et mesure le temps de réponse |
| `nslookup <nom>`  | Demande au serveur DNS l'adresse IP correspondant au nom    |

## Le trajet d'une requête

Quand je tape `https://github.com` dans mon navigateur :

1. l'url
2. le dns
3. la connexion
4. la securité
5. la requete
6. la reponse

## Les codes de réponse HTTP

| Code | Nom                   | Ce qu'il veut dire                          | Exemple que j'ai vu |
| ---- | --------------------- | ------------------------------------------- | ------------------- |
| 200  | OK                    | valide                                      | 200                 |
| 301  | Moved Permanently     | déminagé                                    | 301                 |
| 404  | Not Found             | la page n’existe pas                        | 404                 |
| 500  | Internal Server Error | le serveur a planté en préparant la réponse | 500                 |

## Les ports

| Port | Service                                  | Exemple d'URL      |
| ---- | ---------------------------------------- | ------------------ |
| 80   | http                                     | http://github.com  |
| 443  | https                                    | https://github.com |
| 8000 | développeurs lancent sur leur ordinateur | http.server 8000   |

## Diagnostiquer une erreur

Les 4 questions, dans l'ordre :

1. Le nom est-il trouvé ? → `nslookup <nom>`
2. La machine répond-elle ? Réseau ping -c 4 <nom>
3. Un serveur écoute-t-il le port ? Connexion curl -I <url>  : pas de Couldn't connect  ? Pour votre propre machine : ss -tln 
4. Que répond le serveur ?

### Exemple : une panne que j'ai réparée

- **Symptôme :** le dns ne trouve pas le nom du site
- **Étape :** etape 2
- **Cause :** le site n etais pas hebergé
- **Correction :** hebergement du site
- **Vérification :** 200 OK
