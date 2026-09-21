# Conventions de travail

## Cycle d'une tâche

1. Toute tâche commence par une **issue** (user story, tâche technique, bug).
2. L'issue est priorisée, estimée et placée dans un sprint dans GitHub Projects.
3. On crée une **branche** depuis `main` : `feature/<numéro>-<description>`, `fix/<numéro>-<description>` ou `docs/<numéro>-<description>`.
4. On fait des **commits** courts et réguliers, en suivant la convention ci-dessous.
5. On ouvre une **pull request** qui contient `Closes #<numéro>` : l'issue sera fermée automatiquement à la fusion.
6. La pull request est relue, puis fusionnée dans `main`. La carte passe en « Terminé ».

## Messages de commit

Format : `<type>: <description à l'impératif, en minuscules>`, suivi si besoin de `(#numéro)`.

| Type | Usage |
|---|---|
| `feat` | Nouvelle fonctionnalité |
| `fix` | Correction de bug |
| `docs` | Documentation |
| `style` | Mise en forme, sans changement de comportement |
| `refactor` | Restructuration du code, sans changement de comportement |
| `test` | Ajout ou modification de tests |
| `chore` | Configuration, outillage |

Exemple : `feat: afficher la liste des salles (#6)`

## Priorisation : MoSCoW

| Priorité | Signification |
|---|---|
| Must | Indispensable au MVP |
| Should | Important, mais le MVP fonctionne sans |
| Could | Souhaitable si le temps le permet |
| Won't | Exclu de cette version (la décision reste tracée) |

## Estimation

Les tâches sont estimées en points de complexité, sur la suite 1, 2, 3, 5, 8. Une tâche estimée à plus de 8 points doit être découpée.

## Définition de prêt

Une issue peut entrer dans un sprint si :

- son objectif est compris (format user story pour un besoin utilisateur) ;
- ses critères d'acceptation sont écrits ;
- elle est estimée ;
- ses dépendances sont identifiées.

## Définition de terminé

Une issue est terminée si :

- les critères d'acceptation sont vérifiés ;
- le code passe le lint (`npm run lint`) ;
- l'écran est utilisable au clavier et lisible sur mobile ;
- la pull request a été relue et fusionnée ;
- la documentation est à jour si nécessaire.
