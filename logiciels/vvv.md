# Installer et utiliser VVV

## VirtualBox

Installez la version du logiciel qui correspond à la configuration de votre machine depuis cette [URL](https://www.virtualbox.org/wiki/Downloads)

## Vagrant

Installez la version du logiciel qui correspond à la configuration de votre machine depuis cette [URL](https://www.vagrantup.com/downloads.html)

### Vagrant Host Updater

Installez l'extension Host Updater grâce à cette ligne de commande :

```bash
vagrant plugin install vagrant-hostsupdater
```

## Installer VVV

Clonez le dépôt master de VVV grâce à cette ligne de commande :

```bash
git clone -b master git://github.com/Varying-Vagrant-Vagrants/VVV.git ~/vagrant-local
```

Positionnez-vous dans le répertoire `vagrant-local` puis effectuez une copie du fichier `vvv-config.yml` pour le coller sous le nom de `vvv-custom.yml`. C'est depuis ce deuxième fichier que vous pourrez éventuellement adapter la configuration de VVV.

```bash
cd ~/vagrant-local
cp vvv-config.yml vvv-custom.yml
```

Lancez VVV pour créer la machine virtuelle.

```bash
vagrant up
```

Une fois la série de commande terminée, vérifiez votre installation en vous rendant sur `http://vvv.test` ou `https://vvv.test` `*`.

![Dashboard VVV](https://dl.dropboxusercontent.com/s/5w6x370wh1wc7w4/vvv.png)

NB: Si vous utilisez `https`, pensez à mettre à jour les options `site_url` et `home` de la table `wp_options` de vos sites grâce à l'utilitaire phpMyAdmin de VVV (Utilisateur = mot de passe = root).

PS:  pour vous accéder à l'administration de vos sites WordPress, l'administrateur utiliser ces éléments d'accès :

- identifiant  : `admin`
- mot de passe : `password`

`*` Si vous souhaitez utiliser `https` et éviter les messages d'erreur des navigateurs, vous pouvez installer le certificat autosigné de VVV dans vos certificats en suivant ce [guide (en)](https://varyingvagrantvagrants.org/docs/en-US/references/https/trusting-ca/) depuis la documentation du site du projet [VVV](https://varyingvagrantvagrants.org/).

### Basculer de SVN à Git pour le Trunk de WordPress.

```bash
vagrant ssh
cd /srv/www/wordpress-trunk/bin/
./develop_git
```
Pour sortir du "mode SSH", saisissez:  
```bash
exit
```
