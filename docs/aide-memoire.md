# Aide-mémoire du terminal Linux

## Se déplacer

| Commande | Ce qu'elle fait                           | Exemple    |
| -------- | ----------------------------------------- | ---------- |
| `pwd`    | Affiche le dossier où je suis             | `pwd`      |
| `ls`     | Affiche le contenu du dossier             | `ls`       |
| `ls -l`  | Le contenu en détail : taille, date…      | `ls -l`    |
| `ls -a`  | Le contenu, y compris les fichiers cachés | `ls -a`    |
| `cd`     | Change de dossier                         | `cd ~/dev` |
| `cd ..`  | Remonte d'un niveau                       | `cd ..`    |
| `clear`  | Efface l'écran                            | `clear`    |

## Fichiers et dossiers

| Commande   | Ce qu'elle fait                              | Exemple                         |
| ---------- | -------------------------------------------- | ------------------------------- |
| `mkdir`    | Crée un dossier                              | `mkdir photos`                  |
| `mkdir -p` | Crée plusieurs niveaux de dossiers d'un coup | `mkdir -p projet/assets/images` |
| `touch`    | Crée un fichier vide                         | `touch vide.txt`                |
| `cp`       | Copie un fichier                             | `cp a.txt b.txt`                |
| `cp -r`    | Copie un dossier et tout son contenu         | `cp -r projet sauvegarde`       |
| `mv`       | Déplace ou renomme un fichier                | `mv notes.txt idees.txt`        |
| `rm`       | Supprime un fichier                          | `rm notes.txt`                  |
| `rm -r`    | Supprime un dossier et tout son contenu      | `rm -r photos`                  |

## Lire et chercher

| Commande    | Ce qu'elle fait                                              | Exemple                       |
| ----------- | ------------------------------------------------------------ | ----------------------------- |
| `cat`       | Affiche tout le fichier                                      | `cat notes.txt`               |
| `less`      | Affiche le fichier page par page (`q` pour quitter)          | `less notes.txt`              |
| `head -n 5` | Affiche les 5 premières lignes                               | `head -n 5 notes.txt`         |
| `tail -n 5` | Affiche les 5 dernières lignes                               | `tail -n 5 notes.txt`         |
| `wc -l`     | Compte les lignes                                            | `wc -l notes.txt`             |
| `grep`      | Affiche les lignes qui contiennent un mot                    | `grep ERROR app.log`          |
| `find`      | Retrouve un fichier par son nom                              | `find . -name "*.js"`         |
| `>` / `>>`  | Écrit le résultat dans un fichier (écrase / ajoute à la fin) | `ls > liste.txt`              |
| `\|`        | Donne le résultat d'une commande à la commande suivante      | `grep ERROR app.log \| wc -l` |

## Processus, droits et paquets

| Commande           | Ce qu'elle fait                                          | Exemple                    |
| ------------------ | -------------------------------------------------------- | -------------------------- |
| `ps aux`           | Liste tous les processus d'Ubuntu                        | `ps aux`                   |
| `kill`             | Demande à un processus de s'arrêter                      | `kill 1234`                |
| `chmod +x`         | Ajoute le droit d'exécution : le fichier peut être lancé | `chmod +x script.sh`       |
| `sudo apt update`  | Met à jour la liste des paquets disponibles              | `sudo apt update`          |
| `sudo apt install` | Installe un paquet                                       | `sudo apt install -y tree` |
| `which`            | L'endroit où se trouve un programme                      | `which ls`                 |

## Branches

| Commande     | Ce qu'elle fait                                   | Exemple                           |
| ------------ | ------------------------------------------------- | --------------------------------- |
| `git branch` | Liste les branches de mon projet                  | `git branch`                      |
| `git switch` | Crée une nouvelle branche et se positionne dessus | `git switch -c ajout-section`     |
| `git merge`  | Fusionne une branche dans la branche courante     | `git merge branches-aide-memoire` |

## Astuce de Cheick

| Commande | Ce qu'elle fait                                            | Exemple  |
| -------- | -----------------------------------------                  | -------- |
|git status| Affiche l’état des fichiers : nouveaux, modifiés, préparés |git status|