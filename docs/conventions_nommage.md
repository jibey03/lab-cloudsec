# Conventions de nommage

## Principe
Tous les noms de ressources suivent le même format :

    <type>-<charge>-<env>-<région>[-<instance>]

- **type** : abréviation de la liste Microsoft (rg, vnet, snet, nsg, vm, kv, st, log).
  Placé en premier pour pouvoir trier et filtrer par préfixe dans le portail et la CLI.
- **charge** : ce que contient la ressource (platform, workloads, sandbox, ...).
- **env** : lab, le seul environnement : tout est un lab jetable, donc pas de dev/prod.
- **région** : code court de la région (ex : frc).
- **instance** : numéro à 2 chiffres (ex : 01).

## Règles générales
- Minuscules uniquement, tirets comme séparateurs.
- Jamais de date, de version, d'IP ni de secret dans un nom : un nom Azure ne se
  renomme pas, on détruit et on recrée.
- Un nom doit se comprendre sans ouvrir la ressource.

## Contraintes Azure et exceptions
| Ressource | Contrainte | Conséquence pour le lab |
|---|---|---|
| Storage account | 3-24 car., minuscules et chiffres, pas de tiret, unique mondialement | <À COMPLÉTER : ta règle d'exception> |
| Key Vault | 3-24 car., unique mondialement |
| VM Windows | nom d'ordinateur 15 car. max | <À COMPLÉTER : ta règle> |

## Région
<À COMPLÉTER : région choisie, région de secours, et 2 raisons (coût, latence, services disponibles).>

## Exemples
| Ressource | Nom |
|---|---|
| Resource group | <À COMPLÉTER> |
| Réseau virtuel | <À COMPLÉTER> |
| Storage account | <À COMPLÉTER : vérifie 24 car. max, minuscules, sans tiret> |
| Key Vault | <À COMPLÉTER> |
