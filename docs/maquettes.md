# Maquettes

Les maquettes sont conçues en mobile-first, puis adaptées pour l'ordinateur. Ce document décrit la composition de chaque écran et les choix d'accessibilité.

## Liste des salles

- En-tête : logo de la médiathèque, lien « Mes réservations », lien de connexion.
- Une carte par salle : nom, photo avec texte alternatif, capacité, équipements, bouton « Voir la salle ».
- Mobile : cartes empilées sur une colonne. Ordinateur : grille de deux colonnes.

## Fiche d'une salle

- Nom, photo, capacité, équipements, règles d'utilisation.
- Bouton « Réserver cette salle ».

## Recherche de disponibilité

- Champs : date, heure de début, durée, capacité minimale. Chaque champ a un libellé visible.
- Résultats : liste des salles disponibles, avec un message explicite si aucune salle ne convient.

## Réservation

- Récapitulatif (salle, date, créneau), case de consentement au traitement des données, bouton « Confirmer ».
- Message de confirmation annoncé aux lecteurs d'écran.

## Mes réservations

- Liste des réservations à venir, avec un bouton « Annuler » et une demande de confirmation.

## Connexion

- E-mail et mot de passe, avec libellés visibles et attributs `autocomplete`.
- Message d'erreur générique, qui ne précise pas si c'est l'e-mail ou le mot de passe qui est faux.

## Accessibilité

- Contraste du texte d'au moins 4,5:1.
- Un statut n'est jamais indiqué par la seule couleur.
- Focus visible sur tous les éléments interactifs.
- Cibles tactiles d'au moins 44 pixels de côté.
