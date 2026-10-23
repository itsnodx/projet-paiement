#  Projet Paiement - API Flask

Lien de la capsule vidéo : https://youtu.be/ks04bro5tDc?si=8TJjdGDWyw9mHQEy
##  Description
Ce projet est une **API web de paiement** réalisée avec **Flask**, **PostgreSQL**, **Redis** et **RQ**.  
Il permet de :

- Récupérer dynamiquement la liste des produits depuis une API externe
- Créer une commande pour un ou plusieurs produits
- Ajouter les informations client (adresse, email, province)
- Calculer automatiquement la **taxe selon la province** et les **frais de livraison**
- Afficher un formulaire de paiement avec carte de crédit
- **Traiter le paiement de manière asynchrone** grâce à Redis + RQ
- Mettre à jour le statut de la commande après un paiement réussi
- Afficher et **vérifier le statut d’une commande** (payée ou non)
- Interface HTML minimaliste avec design CSS
---
## Technologies utilisées

- **Python 3.11**
- **Flask**
- **PostgreSQL** (au lieu de SQLite dans la première partie)
- **Redis** (mise en cache)
- **RQ** (traitement asynchrone des paiements)
- **HTML + CSS** (interface utilisateur)
- **Docker & docker-compose** (conteneurisation)

##  Installation et Exécution
Python 3.11+
- Docker + Docker Compose
- Compte GitHub (optionnel pour clonage)

pip install -r requirements.txt

###  **Installation des dépendances**
Avant de commencer, assurez-vous d'avoir au minimum **Python 3.6+** installé sur votre machine.

Étapes

1. **Cloner le dépôt GitHub**
  bash
 git clone https://github.com/Mdaffe17/projet-paiement.git
 cd projet-paiement
2. **Lancer les services avec Docker**
 docker compose up --build

Cela lance :

Le backend Flask (web)

PostgreSQL (db)

Redis (redis)

Worker RQ (worker)
####  Accéder a l'application :

Page d’accueil : http://localhost:5000/

Commander un produit

Remplir les infos client

Payer la commande

Vérifier le statut de la commande


## Auteur
NodX — Projet universitaire

python app.py
