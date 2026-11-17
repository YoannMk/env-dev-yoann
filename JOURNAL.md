# Journal des choix

## 2026-11-03 – Système pour le terminal

- **Décision :** utiliser Ubuntu avec WSL sous Windows 11.
- **Autres possibilités :** utiliser uniquement Windows avec la souris.
- **Raison :** Ubuntu permet d'utiliser les mêmes commandes Linux que sur les serveurs.

## 2026-11-05 – Éditeur de code

- **Décision :** utiliser VS Code avec Ubuntu.
- **Autres possibilités :** utiliser uniquement `nano` dans le terminal.
- **Raison :** VS Code ouvre les dossiers d'Ubuntu avec `code .` et intègre un terminal en bas.

## 2026-11-10 – Installation de Node.js

- **Décision :** installer Node.js avec le dépôt NodeSource et apt.
- **Autres possibilités :** le paquet nodejs d'Ubuntu, le site nodejs.org.
- **Raison :** NodeSource donne la version LTS récente, et les commandes
  peuvent être écrites dans mon README pour être refaites à l'identique.

## 2026-11-11 – Scripts d'installation et de vérification

- **Décision :** écrire les scripts `scripts/installer.sh` et `scripts/verifier.sh`.
- **Autres possibilités :** noter seulement les commandes dans le README et les retaper à la main.
- **Raison :** avec un script, on n'oublie rien, on va plus vite et une autre personne peut refaire l'installation en une seule commande.

## 2026-11-13 – Hébergement du dépôt : GitHub

- **Décision :** publier notre dépôt local sur le site distant GitHub.
- **Autres possibilités :** garder le dépôt uniquement sur mon ordinateur.
- **Raison :** sauvegarder l'historique en ligne et partager le dossier pour qu'il soit évalué.
