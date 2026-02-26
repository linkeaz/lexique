# Contribuer

Merci pour votre contribution.

## Où modifier les données
Le lexique est séparé par catégorie dans `data/`:
- `data/LEXIQUE_CYBER.JSON`
- `data/LEXIQUE_AI.JSON`
- `data/LEXIQUE_INFRA.JSON`
- `data/LEXIQUE_DEV.JSON`

## Convention de noms des fichiers
- Format actuel: `LEXIQUE_<CATEGORIE>.JSON`
- Catégories valides: `CYBER`, `AI`, `INFRA`, `DEV`

## Principes
- Français clair et précis.
- Orthographe et accents obligatoires.
- Ton neutre, défensif, non sensationnaliste.
- Pas de copier-coller de sources externes.

## Format d'une entrée
- `id` (slug anglais, unique)
- `term`
- `category` (`cyber`, `ai`, `infra`, `dev`)
- `shortDefinition` (1 phrase)
- `fullDefinition` (2 à 4 phrases)
- `aliases` (optionnel)
- `related` (optionnel)

## Limites recommandées
- `shortDefinition` : 40 à 140 caractères.
- `fullDefinition` : 120 à 500 caractères.
- `aliases` : max 8.
- `related` : max 6.

## Pull Request
- 1 PR = 1 objectif clair.
- Titre explicite.
- Inclure un bref "pourquoi".
- Vérifier la cohérence des champs `related`.
