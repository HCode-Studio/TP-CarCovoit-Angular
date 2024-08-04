# TP-CarCovoit-Angular

## Intégration Front-End Angular

### Contexte
La semaine dernière, vous avez développé une API Laravel pour une plateforme de covoiturage. Cette semaine, vous allez vous concentrer sur l'intégration du front-end de cette application en utilisant Angular.

### Objectifs
1. Créer une interface utilisateur intuitive et réactive avec Angular.
2. Consommer l'API Laravel que vous avez développée la semaine dernière.
3. Permettre aux utilisateurs de s'inscrire, se connecter, créer des annonces de covoiturage, rechercher des trajets et réserver des trajets.

### Livrables
Au terme de ce TP, vous devrez fournir un projet Angular fonctionnel permettant d’interagir avec l’API Laravel.

### Étapes

1. **Initialiser le Projet Angular**
   - Créez un nouveau projet Angular.
   - Configurez le routage et les modules nécessaires pour votre application.

2. **Interface d'Inscription et de Connexion**
   - Créez des composants pour les formulaires d'inscription et de connexion.
   - Utilisez Reactive Forms pour les formulaires.
   - Connectez-vous à l'API pour gérer les utilisateurs via `/api/register` et `/api/login`.

3. **Création et Gestion des Annonces**
   - Créez un composant pour l’ajout d’une nouvelle annonce de covoiturage via `/api/trips`.
   - Affichez la liste des annonces via `/api/trips`.
   - Mettez en place la possibilité de supprimer et modifier une annonce via `/api/trips/{trip}`.

4. **Recherche de Trajets**
   - Créez un composant de recherche.
   - Affichez les résultats de la recherche sous forme de liste ou de cartes en utilisant les paramètres de `start`, `end`, et `date` dans la route GET de `/api/trips`.

5. **Réservation et Gestion des Réservations**
   - Créez un composant pour réserver un trajet via `/api/booking`.
   - Gérez l'annulation des réservations via `/api/booking/{trip_id}`.

6. **Gestion des Utilisateurs**
   - Implémentez un système de rôle pour les utilisateurs (admin, utilisateur standard).
   - Gérer les informations utilisateur via `/api/users/{user}`.

7. **Améliorations UI/UX**
   - Ajoutez des validations aux formulaires.
   - Mettez en place des notifications pour les actions réussies ou les erreurs.

#### Technologies Utilisées
- **Framework Front-End:** Angular
- **API:** Laravel (développée la semaine dernière)

#### Exemples de Routes API

- **Authentification:** 
  - `POST /api/register` - Inscription d’un utilisateur
  - `POST /api/login` - Connexion d’un utilisateur
  - `POST /api/logout` - Déconnexion d’un utilisateur

- **Annonces:**
  - `GET /api/trips` - Récupération de la liste des annonces de covoiturage
  - `POST /api/trips` - Création d’une annonce de covoiturage
  - `GET /api/trips/{trip}` - Récupération des détails d'un trajet
  - `PUT /api/trips/{trip}` - Mise à jour d’une annonce de covoiturage
  - `DELETE /api/trips/{trip}` - Suppression d’une annonce de covoiturage

- **Réservations:**
  - `POST /api/booking` - Réservation d’un trajet
  - `DELETE /api/booking/{trip_id}` - Annulation d'une réservation 

- **Utilisateurs:**
  - `GET /api/users/{user}` - Récupération des détails d'un utilisateur
  - `PUT /api/users/{user}` - Mise à jour des informations d'un utilisateur
  - `DELETE /api/users/{user}` - Suppression d'un utilisateur

#### Critères d'Évaluation
- Structure du projet Angular.
- Intégration correcte avec l'API Laravel.
- Fonctionnalité et réactivité de l'application.
- Qualité de l'interface utilisateur.
- Respect des bonnes pratiques en matière de développement Angular.

#### Prérequis
- Avoir l’API Laravel fonctionnelle localement ou sur un serveur.
- Connaissances de base en Angular.

ard).
   - Gérer les informations utilisateur via `/api/users/{user}`.

#### Charte Graphique
- Palette de couleurs : [Coolors.co](https://coolors.co/000000-0d9488-abc2bf-f8b25b-fff3a6-fefce8-ffffff)

Exemple d'intégration des couleurs :
- **Couleurs principales :** 
  - `#000000` (Noir)
  - `#0D9488` (Cyan Foncé)
- **Couleurs secondaires :**
  - `#ABC2BF` (Gris Clair)
  - `#F8B25B` (Orange Clair)
- **Couleurs complémentaires :** 
  - `#FFF3A6` (Jaune Clair)
  - `#FEFCE8` (Beige)
  - `#FFFFFF` (Blanc)

Exemple d'intégration avec ces couleurs :
![Homepage example](https://github.com/user-attachments/assets/a48e10b3-ccfc-4c93-96de-1cc033f16795)
