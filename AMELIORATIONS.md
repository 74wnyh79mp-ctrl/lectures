# Améliorations à faire

Liste tenue au fil de l'eau, à traiter en une seule séance après une semaine d'utilisation.

## Faites (24 novembre 2026)

- Nouveau nom : Le Relevé. Interface volontairement neutre pour tester le produit (le design sera retravaillé plus tard), mode jour et mode nuit.
- Chaque événement s'ouvre sur une page à part, avec tous les détails.
- Journaux de chaque événement repliés derrière une flèche ; contexte « Pour comprendre » dépliable.
- Navigation entre les éditions par date.
- Tribunes, éditos et chroniques écartés ; édition plus courte les jours calmes.

## Demandées (historique)

- **Ergonomie : alléger les fiches.** Replier par défaut la liste des journaux (« Double lecture ») de chaque événement, avec une petite flèche pour la déplier quand on veut. Sans ça, la page est trop chargée.
- **Lecture à deux niveaux : pouvoir toucher un événement pour en savoir plus.** Une fiche détaillée avec le contexte global (origines de l'affaire, enjeux, chronologie). À trancher : contexte rédigé à l'avance chaque matin pour tous les événements (coût fixe, un peu plus élevé), ou seulement pour les deux ou trois plus importants. Pas d'explication « à la demande » au clic : ça exposerait la clé API sur un site public.
- **Naviguer entre les jours.** En haut de la page, la date de l'édition affichée, avec des flèches ou un sélecteur pour revoir les éditions précédentes. Les éditions sont déjà archivées dans `docs/archive/` ; il manque un index de ces archives et le sélecteur dans la page. Aucun coût supplémentaire.

## Validé pour la prochaine mise à jour : nouvelle ligne éditoriale

**« Les faits qui comptent, et qui aident à comprendre le monde. »**

Un événement entre dans l'édition s'il passe au moins un de ces tests :
1. Il aura encore de l'importance dans un mois (loi votée, décision de justice qui fait date, tournant dans un conflit).
2. Il concerne beaucoup de gens, en France ou dans le monde (économie, emploi, santé publique, climat, énergie).
3. Il fait avancer un grand sujet en cours (Ukraine, budget, présidentielle 2027, relations États-Unis – Chine…).

Écartés même s'ils sont très repris : faits divers sans conséquence nationale, petites phrases et polémiques sans décision, « réactions » sans fait nouveau, sport et célébrités sauf événement exceptionnel. Classement par portée réelle, pas par nombre d'articles.

**Plus de nombre fixe d'événements.** Remplacer la limite de 6 par rubrique par un seuil d'importance : on garde tout ce qui passe les tests, rien d'autre. Garder seulement un plafond de sécurité large (environ 10 par rubrique) pour qu'une journée chargée ne fasse pas exploser le coût.

**Rendre le tri visible.** Pour chaque événement, une ligne « Pourquoi c'est important », pour pouvoir vérifier le choix et le contester.

Pistes pour mieux juger l'importance, à évaluer :
- donner plus de poids aux articles venant des flux « à la une » des journaux ;
- considérer qu'un sujet présent plusieurs jours de suite est un sujet de fond ;
- noter pendant la semaine de test les événements jugés « pas importants », pour ajuster les consignes.

## Idées en attente (à discuter en fin de semaine)

- **Articles de la veille dans l'édition du jour.** Aujourd'hui, l'appli prend tous les articles des 24 dernières heures : une édition de 6 h 30 reprend donc les articles publiés la veille depuis 6 h 30, et les articles sans date sont gardés. Pistes : ne prendre que ce qui est paru depuis l'édition précédente ; ou garder un sujet de la veille seulement s'il y a du nouveau.
- **Suivi des sujets d'un jour à l'autre (facultatif).** Repérer qu'un événement était déjà dans l'édition précédente et l'afficher comme « Suite » avec seulement ce qui a changé, au lieu de le répéter. À décider : utile ou superflu ?

## Positionnement à formaliser

- **Ce que l'appli est :** une dose d'infos factuelles, à jour, sans le bruit ni l'angoisse d'une chaîne d'info en continu. Les faits, et la façon dont chaque journal les a rapportés.
- **Ce qu'elle n'est pas :** un journal. Pas d'éditos, pas d'opinions, pas de dossiers de fond.
- **Conséquences à appliquer :** écarter des flux les tribunes, éditoriaux et chroniques ; garder le contexte détaillé strictement factuel ; décider du rythme (une édition par jour, ou plusieurs mises à jour courtes).

## À vérifier pendant la semaine de test

- Les résumés sont-ils justes ? Comparer chaque jour un ou deux résumés avec les articles d'origine.
- Les « regards » sont-ils vraiment différents, ou est-ce souvent la même dépêche d'agence ?
- Coût réel d'une édition (console Anthropic).
