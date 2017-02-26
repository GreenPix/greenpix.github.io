# Mac

Vous trouverez ici des instructions pour préparer
votre environement de développement en étant sous Mac.

Tout d'abord vous aurez besoin d'installer **XCode**.
Il se trouve dans l'AppStore. Il vous faudra le lancer
au moins une fois avant de procéder.

## Installer `homebrew`

[Homebrew](https://brew.sh/) est un peu le gestionnaire de
paquets de **Mac OS**.

A la différence de ceux que l'on peut trouver sous **Linux**
comme `apt-get` ou `yaourt` c'est qu'il n'est pas supporté
officiellement par Apple mais est le fruit de la communauté
open-source.

Pour l'installer ouvrer un terminal et copier-coller la ligne
suivante:

```bash
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

Pour vérifier que l'installation s'est bien déroulé:

```
brew --help
```

Vous aurez aussi besoin d'une extension (['cask'](https://caskroom.github.io)):

```bash
brew tap caskroom/cask
```

## Installer Git

Une fois **Homebrew** d'installé, Git peut être installer
simplement via `brew` dans un Terminal:

```bash
brew install git
```

## Installer VirtualBox

Virtual Box permet de créer [des machines virtuelles](https://fr.wikipedia.org/wiki/Virtualisation).
Cela va nous permettre de mettre en place un environement de travail qui est le même
que les autres développeurs et réduits les erreurs spécifiques à certains environements
de travail.

Pour installer **VirtualBox**, dans un terminal:

```bash
brew cask install virtualbox
```

## Installer Vagrant

Vagrant va nous permettre en une seule ligne de commande de préparer l'environement
complet de développement. VirtualBox gére des VMs et nous permets de tous avoir la
même machine quel que soit le système d'exploitation de notre vrai PC.

Cependant, avoir l'OS identique, n'est généralement pas suffisant. Il faut aussi
avoir les mêmes programmes d'installé. Vagrant va se charger de faire tout ça.

Pour installer **Vagrant**, dans un terminal:

```bash
brew cask install vagrant
```