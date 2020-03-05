# Laravel Workshop 

by [Bacq Estelle](https://github.com/BacqEstelle), [Gilotaux Ludivic](https://github.com/Ludgil), [Markus Emile](https://github.com/emilemarkus).

#  Installation de Laravel

# 1. Installation sur Linux 

Au préalable, nous vous conseillons l’installation d’un serveur LAMP  => [ici](https://doc.ubuntu-fr.org/lamp)

## 1.1 Installation de PHP

Dans un premier temps, il vous faut les pré-requis 

```
>sudo apt-get install software-properties-common python-software-properties
```

Ensuite, ajoutez « ondreJ PPA »

```
>sudo apt-get-repository -y ppa:ondrej/php
>sudo apt-get update
```
Mettez a jour vos sources en executant :

```
>sudo apt-get install php -y
```

Et enfin les différentes libraries 

```
>sudo apt-get install php7.4 php7.4-cli php7.4-common
```

Laravel réclame une minimum d’extension php pour fonctionner, en voici la liste : 
* OpenSSL 
* PDO
* Mbstring
* Tokenizer
* XML
* Ctype
* Json
* BCMath

Voici la méthode d’installation pour ses fonctions : 

```
>sudo apt-get install php-curl php-gd php-json  php-mbstring php-intl php-mysql php-xml php7.4-zip
```

Ensuite viens les extensions spécifiques pour laravel :

```
>sudo apt-getinstall -y php7.4-bcmath  php7.4-ctype
```

On relance apache

```
>sudo systemctl restart apache2

ou

>sudo service apache2 restart
```
Un petit bonus, on ne sais jamais si vous en avez besoin l’installation d’un décompresseur zip

```
>sudo apt-get install zip -y
```
## 1.2 Installation de Composer


Laravel utilise les dépendances de php. Alors un petit tour par l’installation de composer est obligatoire.

Installation de curl

```
>sudo apt-get install curl -y
```

Téléchargement de composer

```
>cd  ~
>sudo curl -s https://getcomposer.org/installer | php
```

Maintenant nous allons le rendre disponible globalement

```
>sudo mv composer.phar /usr/local/bin/composer
```

Pour vérifier si composer est bien installer utiliser la commande : 

```
composer
```

Vous devriez voir une liste de commande apparaitre

Maintenant nous allons Installé Laravel Installer via la commande :

```
composer global require laravel/installer
```

Une fois terminer nous allons pouvoir créer notre premier projet :) 

# 2. Installation sur Windows

## 2.1 Installation de PHP

Au préalable, nous vous conseillons l’installation de xampp
 => [ici](https://blog.lws-hosting.com/creation-de-sites-web/utiliser-xampp-pour-creer-son-serveur-web)

## 2.2 Installation de Composer 

Composer est un gestionnaire de package PHP.
Pour l’installer sous windows, rendez-vous sur le site officiel et téléchargez le programme d’installation.
=> [Composer.](https://getcomposer.org/download/)

Au début de l’installation, il vous sera demandé de préciser ou se trouve php.exe.

Rechercher dans votre système ou se trouve le dossier d’installation de xampp/wamp. 

Exemple :
 ```
C:\xampp\php
```
Si l’installation est réussie, relancez votre terminal et tapez y la commande : 

```
composer
```

Si tout est ok, un bon nombre de commande devrait apparaître dans votre terminal. Bonne nouvelle !!! Passons à la suite.


Maintenant nous allons Installé Laravel Installer via la commande :

```
composer global require laravel/installer
```

Une fois terminer nous allons pouvoir créer notre premier projet :)


# 3. Installation sur MAC

Avant toute chose, il vous faut un HomeBrew qui est un gestionnaire de package pour macos.
Pour l’installer, rien de plus simple, rendez-vous sur votre terminal 

```
>/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

Cette étape peut prendre pas mal de temps...

## 3.1 Installation PHP

Installation de php avec homebrew

```
>brew install homebrew/php/php71
```

## 3.2 Installation de composer

Composer est un gestionnaire de dépendance PHP, il permet de télécharger des bibliothèques.

Composer permet également de créer des projets Laravel
Pour installer composer :

```
>brew install homebrew/php/composer
```

Si l’installation est réussie, relancez votre terminal et tapez y la commande :

```
composer
```

Si tout est ok, un bon nombre de commande devrait apparaître dans votre terminal. Bonne nouvelle !!! Passons à la suite.

Maintenant nous allons Installé Laravel Installer via la commande :

```
composer global require laravel/installer
```




# Let's Go 

Voici le lien pour suivre les étapes du Workshop 


[Laravel Workshop](https://ludgil.github.io/Laravel-Workshop/blog/index)