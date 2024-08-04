# Intégration Front-End Angular CarCovoit' 

### Contexte
La semaine dernière, vous avez développé une API Laravel pour une plateforme de covoiturage. Cette semaine, vous allez vous concentrer sur l'intégration du front-end de cette application en utilisant Angular.

### Objectifs
1. Créer une interface utilisateur intuitive et réactive avec Angular.
2. Consommer l'API Laravel que vous avez développée la semaine dernière.
3. Permettre aux utilisateurs de s'inscrire, se connecter, créer des annonces de covoiturage, rechercher des trajets et réserver des trajets.

### Étapes

1. **Initialiser le Projet Angular**
   - Créez un nouveau projet Angular.
   - Configurez le routage et les modules nécessaires pour votre application.

2. **Interface d'Inscription et de Connexion**
   - Créez des composants pour les formulaires d'inscription et de connexion.
   - Créez un model User avec une interface IUser qui nous permettra de typer nos objets avec TypeScript.
   - Utilisez [Reactive Forms](https://angular.dev/guide/forms/reactive-forms) pour les formulaires.
   - Connectez-vous à l'API pour gérer les utilisateurs via `/api/register` et `/api/login`. en utilisant un service `auth.service.ts`
      - Tips: on enregistre le token JWT ainsi que les informations (non sensible) de l'utilisateur connecté dans le LocalStorage du navigateur
      - Le service possèdera minimum 2 méthodes *login* et *register*

3. **Création et Gestion des Annonces de Trajet**
   - Créez un composant pour l’ajout d’une nouvelle annonce de covoiturage via `/api/trips`.
   - Affichez la liste des annonces via `/api/trips`.
   - Mettez en place la possibilité de supprimer et modifier une annonce via `/api/trips/{trip}`.
   - Intégrer les routes api avec un service `trip.service.ts`

4. **Recherche de Trajets**
   - Créez un composant de recherche.
   - Affichez les résultats de la recherche sous forme de liste ou de cartes en utilisant les paramètres de `start`, `end`, et `date` dans la route GET de `/api/trips`.

5. **Réservation et Gestion des Réservations**
   - Créez un composant pour réserver un trajet via `/api/booking`.
   - Gérez l'annulation des réservations via `/api/booking/{trip_id}`.
   - Créer un service `booking.service.ts` pour gérer requêtes de réservations 

6. Bonus : **Gestion de Profil** 
   - Implémentez une page profil permettant que modifier ses informations utilisateurs.
   - Ajouter un historique de vos trajets sur la page
   - Gérer les informations utilisateur via `/api/users/{user}`.

### Technologies Utilisées
- **Framework Front-End:** Angular
- **API:** Laravel [ici](https://github.com/G404-DWWM/correction-car-covoit-api)


### Charte Graphique
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
