
# Installation de Laravel sur macOS

Ce guide explique comment installer Laravel sur macOS en utilisant Homebrew, Composer, et les outils PHP nécessaires. Suivez les étapes ci-dessous pour configurer votre environnement de développement Laravel.

---

## Prérequis

Avant de commencer, assurez-vous que les éléments suivants sont installés sur votre machine :

- **Homebrew** : Gestionnaire de paquets pour macOS.
- **PHP** : Langage utilisé par Laravel.
- **Composer** : Gestionnaire de dépendances PHP.

Si vous n'avez pas encore Homebrew installé, exécutez la commande suivante dans votre terminal pour l'installer :

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

---

## Étape 1 : Installation de PHP

Laravel requiert PHP, et vous pouvez l'installer via Homebrew. Dans le terminal, exécutez la commande suivante :

```bash
brew install php
```

Une fois PHP installé, vérifiez son installation en tapant :

```bash
php -v
```

Vous devriez voir la version de PHP installée, confirmant que tout fonctionne correctement.

---

## Étape 2 : Installation de Composer

Composer est le gestionnaire de dépendances utilisé pour installer Laravel. Pour l'installer globalement sur votre machine, exécutez les commandes suivantes dans le terminal :

```bash
brew install composer
```

Une fois l'installation terminée, vérifiez que Composer est bien installé avec :

```bash
composer -v
```

---

## Étape 3 : Installation de Laravel via Composer

Maintenant que PHP et Composer sont installés, vous pouvez installer Laravel globalement. Utilisez la commande suivante dans le terminal :

```bash
composer global require laravel/installer
```

### Configuration du PATH pour Laravel

Pour que la commande `laravel` soit accessible globalement dans le terminal, vous devez ajouter le chemin de Composer au `PATH` de votre système. Ajoutez la ligne suivante à votre fichier `~/.zshrc` (ou `~/.bash_profile` si vous utilisez Bash) :

```bash
export PATH="$HOME/.composer/vendor/bin:$PATH"
```

Ensuite, rechargez le fichier avec la commande :

```bash
source ~/.zshrc
```

Vérifiez que Laravel est bien installé en tapant :

```bash
laravel
```

---

## Étape 4 : Création d'un projet Laravel

Maintenant que Laravel est installé, vous pouvez créer un nouveau projet Laravel avec la commande suivante :

```bash
laravel new nom_du_projet
```

Cette commande va créer un nouveau dossier contenant tous les fichiers nécessaires pour démarrer un projet Laravel.

---

## Étape 5 : Lancement du serveur local

Une fois que le projet est créé, accédez au dossier du projet :

```bash
cd nom_du_projet
```

Lancez le serveur de développement local de Laravel en utilisant la commande :

```bash
php artisan serve
```

Ouvrez votre navigateur et accédez à l'URL suivante pour voir votre application Laravel en action :

```bash
http://localhost:8000
```

---

## Problèmes Courants et Solutions

### Problème : Commande `laravel` introuvable
Si vous voyez une erreur indiquant que la commande `laravel` est introuvable, assurez-vous que le chemin vers Composer est bien ajouté au fichier `~/.zshrc` ou `~/.bash_profile`, comme mentionné dans l'étape 3.

### Problème : Permissions refusées
Si vous rencontrez des problèmes de permissions lors de l'installation de PHP ou Composer, essayez d'exécuter les commandes avec `sudo` pour les exécuter avec des privilèges d'administrateur.

---

## Ressources Supplémentaires

- Documentation Laravel : [https://laravel.com/docs](https://laravel.com/docs)
- Documentation Composer : [https://getcomposer.org/doc/](https://getcomposer.org/doc/)
- Homebrew : [https://brew.sh/](https://brew.sh/)

---

## Conclusion

Félicitations ! Vous avez maintenant Laravel installé et configuré sur votre machine macOS. Vous êtes prêt à commencer le développement de vos projets Laravel. Si vous rencontrez des problèmes ou avez des questions, n'hésitez pas à consulter la documentation ou à poser des questions dans la communauté Laravel.














































# Laravel Installation

This README provides a step-by-step guide to install Laravel on macOS using Homebrew, Composer, and PHP. Follow these instructions to set up your development environment for Laravel applications.


Simple step-by-step way for [Laravel installation on Mac OS](https://pop-corn-code.github.io/Laravel-setup/laravel_installation_macOS.md)
