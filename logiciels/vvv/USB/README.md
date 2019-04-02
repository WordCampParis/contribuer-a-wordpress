# Générer une clé USB contenant un VVV prêt à l’emploi

Le dépôt [CD USB Generator](https://github.com/Varying-Vagrant-Vagrants/CD-USB-Generator) vous permet d’économiser les téléchargements chronophages de VVV, Vagrant et Virtual Box lors des journées de contribution.

Après l’avoir cloné, il suffit de jouer la commande `./run.sh` pour qu'à partir de votre configuration VVV deux répertoires soit créés : `vvv` et `build`. Le premier est un répertoire temporaire que le script utilise pour télécharger tout le nécessaire à la constitution du deuxième.

Lorsque le script a terminé son exécution il s'agit de copier le contenu du répertoire `build` à la racine de votre clé USB.

Pour une prise en main simplifiée des utilisateurs français, vous pouvez remplacer le fichier `instructions.html` de la clé USB par [cette version traduite](./instructions.html).