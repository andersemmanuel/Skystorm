<p align="center">
  <img src="C:\Users\ander\PhpstormProjects\php_cours\Skystorm\logo.png" alt="SkyStorm Logo" width="300">
</p>

# ⚡ SkyStorm

**SkyStorm** est une réplique allégée de **Twitter/X** développée avec **Laravel 12** dans un contexte pédagogique pour la préparation à l’épreuve **E6 du BTS SIO option SLAM**.

Le projet est construit en direct avec la classe afin d’illustrer **un cycle complet de développement web** :

- conception
- modélisation
- implémentation
- déploiement

---

# 🎯 Objectifs pédagogiques

- Comprendre l’architecture **MVC de Laravel**
- Manipuler l’**authentification avec Laravel UI (Bootstrap)**
- Concevoir un **MCD** et le traduire en **base de données relationnelle**
- Gérer les relations **1-N et N-N avec Eloquent**
- Implémenter des **fonctionnalités sociales**
- Structurer un projet **Git professionnel**

---

# 🛠 Stack technique

- **PHP 8.x**
- **Laravel 12**
- **Laravel UI (Bootstrap)**
- **MySQL / MariaDB**
- **Eloquent ORM**
- **Blade**

---

# 🚀 Fonctionnalités principales

- Inscription / connexion utilisateur
- Création de posts
- Modification et suppression de posts
- Système de **suivi entre utilisateurs**
- Système de **likes**
- **Fil d’actualité simplifié**

---

# 🗄 Modélisation des données

Le modèle de données repose principalement sur deux entités :

- **Users**
- **Posts**

avec des relations sociales entre utilisateurs.

### MCD (Mocodo)
FOLLOW, 0N Users, 0N Users
Users: id_user, name, email, password, created_at

LIKE, 0N Users, 0N Posts

POST, 0N Users, 11 Posts
Posts: id_post, content, created_at

---

# ⚙ Installation

```bash
git clone https://github.com/andersemmanuel/Skystorm.git
cd Skystorm
composer run-script setup

Configurer ensuite le fichier .env :
base de données
nom de l'application
URL

Puis exécuter :
php artisan migrate
php artisan serve

📁 Structure du projet
app/Models              # Modèles Eloquent
app/Http/Controllers    # Logique métier
resources/views         # Templates Blade
database/migrations     # Schéma de base de données
routes/web.php          # Routes principales
📚 Contexte pédagogique

Ce projet est réalisé dans le cadre de la formation BTS SIO SLAM afin de :

comprendre le fonctionnement d’un framework moderne

apprendre les bonnes pratiques Laravel

utiliser Git dans un contexte professionnel

📜 Licence

Projet pédagogique.
Utilisation libre dans un cadre scolaire ou de formation.
