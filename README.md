# Carnet CRM

CRM (gestion de la relation client) pour petite entreprise, livré vierge : l'entreprise y entre ses propres informations.

Projet réalisé par Ilian SEGHIRI, BTS SIO option SISR (Ensitech).

![Aperçu du CRM](apercu.png)

## Fonctionnalités

- **Mise en route guidée** en 4 étapes à la première ouverture
- **Paramètres de l'entreprise** : nom, secteur, e-mail de contact
- **Contacts** : fiches clients et prospects, recherche et filtre par statut
- **Pipeline commercial** en kanban : glisser-déposer des opportunités entre les étapes (Nouveau, Contacté, Devis envoyé, Négociation, Gagné, Perdu)
- **Relances** : appels, e-mails et rendez-vous avec date d'échéance, alerte en cas de retard
- **Tableau de bord** : pipeline en cours, chiffre signé, taux de transformation, montant par étape
- **Sauvegarde et restauration** des données au format JSON

## Technique

- Une seule page : HTML, CSS et JavaScript, sans framework ni serveur
- Données enregistrées dans le navigateur (`localStorage`)
- Interface responsive (ordinateur et téléphone), mode clair et sombre
- Validation des saisies et protection contre les failles XSS (échappement des données affichées)

## Limites et évolutions prévues

Les données restent dans le navigateur de chaque utilisateur : deux postes ne partagent pas les mêmes contacts. Une version suivante pourrait ajouter un serveur (PHP + MySQL) avec des comptes utilisateurs et des rôles.
