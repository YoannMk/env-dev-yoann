# Fiche réseau

## Mes adresses IP

| Machine                | Adresse IP     | Privée ou publique ? |
| ---------------------- | -------------- | -------------------- |
| Mon Ubuntu             | 172.22.91.167  | privée               |
| Mon ordinateur (Wi-Fi) | 172.16.51.24   | privée               |
| Ma connexion Internet  | (non publiée)  | publique             |

## Résultats du DNS

| Nom de domaine  | Adresse IP    |
| --------------- | ------------- |
| `github.com`    | 140.82.121.3  |
| `wikipedia.org` | 185.15.59.224 |

## Les outils réseau

| Commande          | Ce qu'elle fait                          |
| ----------------- | ---------------------------------------- |
| `hostname -I`     | Affiche l'adresse IP de mon Ubuntu       |
| `ping -c 4 <nom>` | Envoie seulement 4 paquets puis s'arrête |
| `nslookup <nom>`  | Donne l'adresse IP d'un nom de domaine   |

## Le trajet d'une requête

Quand je tape `https://github.com` dans mon navigateur :

1. Je tape l'adresse `https://github.com` dans mon navigateur qui joue le rôle de client.
2. Le navigateur interroge le DNS pour connaître l'adresse IP de `github.com` (`140.82.121.3`).
3. Le navigateur se connecte au serveur de GitHub à l'adresse `140.82.121.3`.
4. Avec HTTPS, le serveur présente son certificat, le navigateur le vérifie puis chiffre la connexion.
5. Le navigateur envoie la requête `GET /` au serveur pour demander la page d'accueil.
6. Le serveur renvoie la réponse `200 OK` avec le code HTML de la page, et le navigateur l'affiche.

## Les codes de réponse HTTP

| Code | Nom                   | Ce qu'il veut dire                            | Exemple que j'ai vu                             |
| ---- | --------------------- | --------------------------------------------- | ----------------------------------------------- |
| 200  | OK                    | Succès : la page demandée est bien envoyée    | `https://github.com`                            |
| 301  | Moved Permanently     | Redirection : la page a changé d'adresse      | `http://github.com` vers `https://github.com/`  |
| 404  | Not Found             | Erreur client : la page demandée n'existe pas | `https://github.com/page-qui-nexiste-pas-ifran` |
| 500  | Internal Server Error | Erreur serveur : le serveur a eu un problème  | (pas vu)                                        |
