# Réservation de salles - Médiathèque de Valmont

Projet fictif à visée pédagogique. Il illustre l'organisation d'un projet avec GitHub : issues, jalons, branches, pull requests et GitHub Projects. Ce n'est pas une application réelle.

## Contexte

La médiathèque de Valmont met à disposition quatre salles (salle de travail, salle de réunion, auditorium, studio d'enregistrement). Les réservations se font aujourd'hui par téléphone et sont notées dans un agenda papier : doubles réservations, absence de visibilité pour les usagers, aucune statistique d'occupation.

## Objectif

Permettre aux usagers inscrits de consulter les salles, de vérifier leur disponibilité et de réserver un créneau en ligne, et donner aux agents un outil de gestion du catalogue et du planning.

## Acteurs

| Acteur | Rôle |
|---|---|
| Usager | Consulte les salles, réserve et annule ses créneaux |
| Agent de la médiathèque | Gère le catalogue des salles, bloque une salle pour maintenance |
| Responsable | Consulte le taux d'occupation des salles |

## Organisation du projet

- Méthode itérative : sprints de deux semaines, revue et planification à chaque fin de sprint.
- Suivi : [GitHub Projects](https://github.com/orgs/mnbd-software/projects/1) (vues Backlog, Sprint en cours, Roadmap, Toutes les tâches).
- Jalons : voir l'onglet Milestones du dépôt.
- Conventions de travail : [CONTRIBUTING.md](CONTRIBUTING.md).

## Documentation

- [Note de cadrage](docs/note-de-cadrage.md)
- [User stories du MVP](docs/user-stories.md)
- [Maquettes](docs/maquettes.md)
- [Enchaînement des écrans](docs/enchainement-ecrans.md)
- [Comptes rendus de réunion](docs/comptes-rendus/)

## Lancer le projet

Prérequis : Node.js 20 ou supérieur.

```bash
npm install
npm run lint
npx serve src
```

## Technologies

HTML, CSS (approche mobile-first), html-validate pour l'analyse statique.
