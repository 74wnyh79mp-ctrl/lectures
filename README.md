# Le Relevé

Les faits du jour, recoupés par plusieurs journaux. Pas un journal : pas d'éditos ni d'opinions, juste une dose d'infos factuelles, sans le bruit.

Chaque matin, un programme lit les flux RSS de plusieurs journaux, envoie les titres à Claude, qui regroupe les articles par événement et rédige l'essentiel, puis publie une édition finie en deux rubriques : **France** et **International**.

## Comment ça marche

| Fichier | Rôle |
| --- | --- |
| `sources.json` | La liste des flux RSS, rangés par rubrique. |
| `build_edition.py` | Lit les flux, appelle Claude, écrit `docs/edition.json`. |
| `docs/index.html` | La page que tu ouvres sur ton téléphone. |
| `docs/archive/` | Une copie de chaque édition. |
| `.github/workflows/edition.yml` | L'automatisation : tous les jours vers 6 h 30 (heure de Paris, en hiver). |

## Mise en route (à faire une seule fois)

1. **Clé API** : sur la console Anthropic, crée une clé API et fixe une limite de dépenses mensuelle.
2. **Secret** : dans le dépôt, *Settings → Secrets and variables → Actions → New repository secret*. Nom : `ANTHROPIC_API_KEY`, valeur : ta clé. Ne la colle jamais ailleurs.
3. **Publication** : *Settings → Pages → Source* : choisis **GitHub Actions**.
4. **Premier lancement** : onglet *Actions → Édition du jour → Run workflow*.

L'adresse du site apparaît ensuite dans *Settings → Pages*.

## Modifier les sources

Ouvre `sources.json` et ajoute ou retire des lignes du type :

```json
{ "source": "Nom du journal", "url": "https://adresse-du-flux.xml" }
```

Un flux qui ne répond pas est simplement ignoré. La liste « Sources consultées », en bas de chaque rubrique, indique combien d'articles chaque flux a fournis.

## Limites connues

- Les résumés sont rédigés par une IA à partir des titres et chapeaux des flux. Ils peuvent contenir des erreurs : les liens vers les articles sont là pour vérifier.
- Usage personnel. Avant toute ouverture au public, vérifier les conditions de réutilisation des contenus de presse (droits voisins).
