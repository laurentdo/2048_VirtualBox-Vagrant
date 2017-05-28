# TP  : (2048_VirtualBox-Vagrant)

Le but est de déployer rapidement le jeu 2048 sur une VM VirtualBox, grace à Vagrant.

## Contributions

J'utilise https://github.com/ObjectifLibre/2048.git, pour la partie applicative

## Screenshot

<p align="center">
  <img src="https://cloud.githubusercontent.com/assets/1175750/8614312/280e5dc2-26f1-11e5-9f1f-5891c3ca8b26.png" alt="Screenshot"/>
</p>

## Installation
- Vagrant : https://www.virtualbox.org/wiki/Downloads
- VirtualBox : http://www.vagrantup.com/downloads.html

## Utilisation de l'environnement

Pour avoir le status des machines virtuelles, il faut taper la commande suivante :
```bash
vagrant status
```
Pour lancer une machine virtuelle :
```bash
vagrant up NOM_DE_VOTRE_MACHINE
```
Pour arrêter une machine virtuelle :
```bash
vagrant halt NOM_DE_VOTRE_MACHINE
```
Pour détruire votre machine virtuelle :
```bash
vagrant destroy NOM_DE_VOTRE_MACHINE
```
