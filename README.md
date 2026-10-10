# Plateforme de covoiturage étudiante

Plateforme de covoiturage dédiée à la communauté étudiante de l'EFREI, pour faciliter les trajets vers le campus, les lieux de cours et les événements de l'école.

Projet de cours en équipe, module de programmation avancée côté client et serveur.
**Mon rôle : développement du back-end.**

## Le problème

Les étudiants se déplacent vers les mêmes lieux aux mêmes horaires, souvent seuls. L'objectif était de les mettre en relation pour réduire les coûts de transport et créer du lien dans la promotion.

## Ce que fait l'application

- **Création de compte et authentification**, avec hachage des mots de passe en base
- **Publication d'un trajet** par un conducteur : date, heure, lieu de départ, destination, nombre de places disponibles
- **Modification et suppression** de ses propres trajets
- **Liste de tous les trajets publiés**, consultable par l'ensemble des utilisateurs
- **Réservation d'une place** par un passager, avec mise à jour du nombre de places restantes

## Ma contribution

J'ai pris en charge la partie serveur :

- Conception et développement des API REST pour la gestion des utilisateurs, des trajets et des réservations
- Authentification sécurisée avec hachage des mots de passe par bcrypt
- Communication entre l'application monopage et le serveur
- Persistance des données en base SQL

## Stack

| Couche | Technologies |
|---|---|
| Serveur | Node.js, Express.js |
| Client | Vue.js |
| Données | SQL |
| Sécurité | bcrypt |

## Ce que ce projet m'a appris

La partie la plus délicate n'était pas de créer un trajet, c'était de maintenir le nombre de places cohérent : deux réservations simultanées sur la dernière place ne doivent pas toutes les deux réussir. C'est le genre de détail invisible dans le cahier des charges et évident dès le premier test à deux utilisateurs.
