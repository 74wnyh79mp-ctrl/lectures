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

## Faites (25 novembre 2026)

- Nouvelle ligne éditoriale (ci-dessous), sans nombre fixe d'événements, avec « Pourquoi c'est important ».
- Rubriques thématiques Défense, Achats, Tech et IA, qui complètent le socle sans le répéter ; bouton « + » pour choisir ses rubriques.
- Suivi d'un jour à l'autre : les articles déjà utilisés sont écartés, un sujet qui avance devient une « Suite », un sujet sans nouveauté disparaît.

- Historique d'un sujet : depuis une « Suite », frise de toutes les étapes précédentes, tirée des éditions archivées (aucun coût d'IA). Idée née du retour de la mère de Raphael (« suivre un sujet qui m'intéresse »).

## Ligne éditoriale en vigueur

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

- **Suivi au-delà de la veille.** Aujourd'hui, la comparaison se fait seulement avec l'édition précédente : un sujet qui revient après plusieurs jours est traité comme nouveau.
- **Nom et devise** : ils disent ce que fait l'appli, pas ce qu'elle évite (retour d'Alexis : « ce n'est pas que les bonnes nouvelles ? »).
- **Mettre en avant les regards divergents** : pour chaque événement, une phrase « Ce qui diverge » et une étiquette « Regards divergents » sur les cartes où les journaux racontent le même fait très différemment ; montrer les angles dès la liste. Rester sur des angles différents, sans mise en scène de polémique.
- **Comptes utilisateurs** (plus tard) : profil, connexion, rubriques et filtre synchronisés entre appareils.
- **Filtre d'importance** : une note de 1 à 3 par événement, et un réglage sur le téléphone. Plutôt deux niveaux (« L'essentiel » / « Complet ») que trois. Les événements secondaires en brèves (titre, une phrase, un lien) pour limiter le coût (+20 à 40 % estimés). « L'essentiel » par défaut.
- **Rejeté : recherche libre avec les opinions des journaux** (retour de la mère de Raphael). Revient à refaire Google et contredit la ligne « pas d'opinions » ; le besoin réel (suivre un sujet) est couvert par les Suites et l'historique.
- **Personnalisation** : socle commun obligatoire + rubriques au choix (fait sur ce téléphone) ; rubriques sur mesure plus tard éventuellement.

## Positionnement à formaliser

- **Ce que l'appli est :** une dose d'infos factuelles, à jour, sans le bruit ni l'angoisse d'une chaîne d'info en continu. Les faits, et la façon dont chaque journal les a rapportés.
- **Ce qu'elle n'est pas :** un journal. Pas d'éditos, pas d'opinions, pas de dossiers de fond.
- **Conséquences à appliquer :** écarter des flux les tribunes, éditoriaux et chroniques ; garder le contexte détaillé strictement factuel ; décider du rythme (une édition par jour, ou plusieurs mises à jour courtes).

## À vérifier pendant la semaine de test

- Les résumés sont-ils justes ? Comparer chaque jour un ou deux résumés avec les articles d'origine.
- Les « regards » sont-ils vraiment différents, ou est-ce souvent la même dépêche d'agence ?
- Coût réel d'une édition (console Anthropic).
