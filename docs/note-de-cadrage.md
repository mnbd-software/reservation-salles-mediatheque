# Note de cadrage

**Projet** : Réservation de salles - Médiathèque de Valmont
**Version** : 1.0, validée en revue de sprint 0 le 02/10/2026

## 1. Contexte et problèmes

La médiathèque de Valmont prête quatre salles à ses usagers inscrits. Les réservations se font par téléphone et sont notées dans un agenda papier.

Problèmes constatés :

- doubles réservations, environ deux par mois ;
- les usagers ne peuvent pas connaître les disponibilités sans appeler ;
- les agents passent du temps au téléphone pendant les heures d'affluence ;
- la responsable ne dispose d'aucune statistique d'occupation.

## 2. Objectifs

1. Permettre la réservation en ligne, sans appel téléphonique.
2. Supprimer les doubles réservations.
3. Donner aux agents un outil de gestion du catalogue et du planning.
4. Mesurer le taux d'occupation des salles.

## 3. Périmètre

| Inclus | Exclu |
|---|---|
| Consultation des salles et de leurs disponibilités | Paiement en ligne (les salles sont gratuites pour les inscrits) |
| Réservation et annulation par l'usager | Gestion des inscriptions à la médiathèque (outil existant) |
| Gestion du catalogue par les agents | Prêt de matériel audiovisuel |
| Statistiques d'occupation | Application mobile native |

## 4. Acteurs

| Acteur | Droits |
|---|---|
| Usager | Consulter, réserver, annuler ses réservations |
| Agent | Droits de l'usager, plus gestion des salles et blocage pour maintenance |
| Responsable | Droits de l'agent, plus statistiques |

## 5. Contraintes

- Accessibilité : RGAA, niveau AA (service public).
- RGPD : seules les données nécessaires à la réservation sont conservées (nom, e-mail, créneau). Les réservations sont supprimées 12 mois après leur date.
- Délai : mise en production le 11/12/2026.
- Équipe : un développeur, une responsable côté client disponible en fin de sprint.

## 6. MVP

Le MVP correspond au jalon 2 : un usager connecté peut rechercher une salle disponible, la réserver et annuler sa réservation. Les doubles réservations sont impossibles.

## 7. Jalons

| Jalon | Date | Contenu |
|---|---|---|
| Jalon 1 - Cadrage validé | 02/10/2026 | Note de cadrage, user stories, maquettes |
| Jalon 2 - MVP réservation | 13/11/2026 | Parcours de réservation complet |
| Jalon 3 - Administration | 27/11/2026 | Gestion des salles, statistiques |
| Jalon 4 - Mise en production | 11/12/2026 | Recette, guide de déploiement |

## 8. Risques

| Risque | Probabilité | Impact | Mesure |
|---|---|---|---|
| Sous-estimation du module de réservation (règles de créneaux) | Moyenne | Fort | Découper en stories de 5 points maximum, traiter la règle anti-double réservation tôt |
| Indisponibilité de la responsable pour les validations | Moyenne | Moyen | Revues de sprint planifiées dès le cadrage, validation asynchrone possible |
| Exigences d'accessibilité découvertes tardivement | Faible | Fort | Audit d'accessibilité dès le premier formulaire |
