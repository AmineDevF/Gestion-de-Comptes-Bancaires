# 📘 Projet : Gestion de Comptes Bancaires

## 📝 Contexte
Vous allez développer une petite application PHP orientée objet (OOP) qui permet de gérer des comptes bancaires. Les utilisateurs (clients) pourront consulter leur solde, effectuer des dépôts, retraits, et transferts d’argent.

---

## 🚀 Fonctionnalités

### 👤 Partie Client

1. 🔑 **Connexion**
   - En tant que client, je veux me connecter pour accéder aux fonctionnalités de gestion de mon compte.

2. ✏️ **Modifier les informations personnelles**
   - En tant que client, je veux modifier mes informations personnelles en fournissant mon nom, email, et mot de passe.

3. 💰 **Consulter mon solde**
   - En tant que client, je veux voir le solde de mon compte courant et épargne pour suivre mes finances.

4. ➕ **Effectuer des dépôts**
   - En tant que client, je veux déposer de l’argent sur mon compte (minimum 0,01 €) afin d’augmenter mon solde.

5. ➖ **Effectuer des retraits**
   - En tant que client, je veux retirer de l’argent de mon compte, dans la limite de mon solde disponible.

6. 🔄 **Effectuer des transferts**
   - En tant que client, je veux transférer de l’argent d’un compte à un autre (ex. : courant → épargne) pour gérer mes finances.

7. 📜 **Consulter l’historique des transactions**
   - En tant que client, je veux consulter l’historique des dépôts, retraits, et transferts effectués.

8. 🔍 **Rechercher dans l’historique des transactions**
   - En tant que client, je veux rechercher des transactions spécifiques dans mon historique en utilisant une interface AJAX pour des résultats instantanés.

---

### 🏦 Partie Administrateur

1. 👥 **Gérer les comptes des clients**
   - En tant qu’administrateur, je veux pouvoir ajouter, modifier ou désactiver les comptes des clients.

2. 📊 **Afficher les rapports financiers**
   - En tant qu’administrateur, je veux générer un rapport global qui affiche :
     - Le total des dépôts effectués par tous les clients.
     - Le total des retraits effectués.
     - Le solde cumulé de tous les comptes.

3. 🔍 **Rechercher des clients**
   - En tant qu’administrateur, je veux rechercher rapidement des clients via une interface AJAX pour faciliter la gestion.

---

## 🛠️ Technologies
- **Langage** : PHP (OOP)
- **Base de données** : MySQL avec PDO

---

## 📋 Table de la Base de Données

### Table `users`
| Champ        | Type         | Description                        |
|--------------|--------------|------------------------------------|
| id           | INT          | Identifiant unique                |
| name         | VARCHAR(100) | Nom du client                     |
| email        | VARCHAR(100) | Email du client                   |
| password     | VARCHAR(255) | Mot de passe (haché)              |
| profile_pic  | VARCHAR(255) | Chemin de l'image de profil       |
| created_at   | TIMESTAMP    | Date de création du compte        |
| updated_at   | TIMESTAMP    | Dernière mise à jour des données  |

---

## 📂 Structure du Projet
```
project/
├── config/
│   └── database.php       # Configuration de la base de données
├── controllers/
│   ├── ClientController.php
│   └── AdminController.php
├── models/
│   ├── User.php           # Modèle utilisateur
│   ├── Account.php        # Modèle compte bancaire
│   └── Transaction.php    # Modèle transaction
├── views/
│   ├── login.php
│   ├── dashboard.php
│   └── admin.php
└── public/
    ├── index.php          # Point d'entrée principal
    └── assets/            # Fichiers CSS/JS/images
```

---

## 📅 Durée et Niveau
- **Durée estimée** : 4 jours
- **Niveau** : Moyennement complexe

---

## ✅ Critères d'Évaluation
1. Respect de la structure OOP (encapsulation, héritage, polymorphisme, abstraction).
2. Fonctionnalités implémentées conformément aux user stories.
3. Validation des formulaires et gestion des erreurs.
4. Bonne organisation du code et respect des conventions.
5. Documentation claire et lisible.

---

## 📌 Améliorations Futures
- Ajouter une fonctionnalité de téléchargement de relevés bancaires en PDF.
- Intégrer les notifications par email.

---


