# Améliorations à faire

Liste tenue au fil de l'eau, à traiter en une seule séance après une semaine d'utilisation.

## Demandées

- **Ergonomie : alléger les fiches.** Replier par défaut la liste des journaux (« Double lecture ») de chaque événement, avec une petite flèche pour la déplier quand on veut. Sans ça, la page est trop chargée.
- **Lecture à deux niveaux : pouvoir toucher un événement pour en savoir plus.** Une fiche détaillée avec le contexte global (origines de l'affaire, enjeux, chronologie). À trancher : contexte rédigé à l'avance chaque matin pour tous les événements (coût fixe, un peu plus élevé), ou seulement pour les deux ou trois plus importants. Pas d'explication « à la demande » au clic : ça exposerait la clé API sur un site public.
- **Naviguer entre les jours.** En haut de la page, la date de l'édition affichée, avec des flèches ou un sélecteur pour revoir les éditions précédentes. Les éditions sont déjà archivées dans `docs/archive/` ; il manque un index de ces archives et le sélecteur dans la page. Aucun coût supplémentaire.

## Positionnement à formaliser

- **Ce que l'appli est :** une dose d'infos factuelles, à jour, sans le bruit ni l'angoisse d'une chaîne d'info en continu. Les faits, et la façon dont chaque journal les a rapportés.
- **Ce qu'elle n'est pas :** un journal. Pas d'éditos, pas d'opinions, pas de dossiers de fond.
- **Conséquences à appliquer :** écarter des flux les tribunes, éditoriaux et chroniques ; garder le contexte détaillé strictement factuel ; décider du rythme (une édition par jour, ou plusieurs mises à jour courtes).

## À vérifier pendant la semaine de test

- Les résumés sont-ils justes ? Comparer chaque jour un ou deux résumés avec les articles d'origine.
- Les « regards » sont-ils vraiment différents, ou est-ce souvent la même dépêche d'agence ?
- Coût réel d'une édition (console Anthropic).
