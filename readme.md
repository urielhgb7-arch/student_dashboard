🎨 Rôle du fichier

Le fichier style.css définit l’apparence visuelle et la mise en page du site web associé à index.html. Il gère :

Les couleurs, polices et arrière-plans.

La disposition des sections (header, nav, section, footer).

Les effets interactifs (hover, active) sur les liens, images et options.

L’uniformité du design grâce à des règles globales (*, body).

🧩 Structure du fichier

Le fichier est organisé par blocs correspondant aux éléments HTML :

Global reset (*) : supprime marges/paddings par défaut et applique box-sizing: border-box.

Body : définit la police principale, la couleur de fond et les dimensions globales.

Header : couleur aquamarine, arrondi et ombre portée.

Nav : barre de navigation violette avec flexbox pour aligner les éléments.

Footer : fond noir, texte vert fluo, bordure verte.

Section : marges et centrage du contenu.

Span : blocs interactifs avec effet hover.

Listes (nav ul, section li) : suppression des puces, mise en page en flexbox, ajout de symboles personnalisés.

Liens (a) : styles par défaut, effets hover et active.

Options (.option, .ressources, .schedule) : tailles spécifiques et transitions sur hover.

Images (img) : centrées, arrondies, avec ombre et effet hover.

Figcaption : texte souligné, police monospace, couleur violette.

Titres (h2) : marges, couleur violette et soulignement.

🛠️ Comment modifier sans casser le design

Pour garder la cohérence visuelle :

Respecter les sélecteurs existants : ne pas supprimer les classes .option, .ressources, .schedule, car elles sont utilisées pour la mise en page.

Utiliser les mêmes unités : le fichier mélange vh, vw, %. Conserver ce système pour éviter des incohérences.

Maintenir les transitions : si vous changez les couleurs ou tailles, gardez les propriétés transition pour conserver les effets fluides.

Couleurs : privilégier des teintes cohérentes avec la palette actuelle (violet, aquamarine, vert fluo, bleu clair).

Flexbox : ne pas retirer display:flex des éléments clés (nav ul, img) pour éviter la rupture d’alignement.

Hover/Active states : si vous ajoutez de nouveaux éléments interactifs, définissez aussi leurs états :hover et :active.

✅ Bonnes pratiques

Ajouter vos nouvelles règles après celles existantes pour éviter les conflits.

Tester les modifications sur plusieurs tailles d’écran (responsive design).

Documenter vos changements directement dans le CSS avec des commentaires.

Ce fichier est la base du design : toute modification doit préserver la logique de structure et d’interaction pour garantir une expérience utilisateur fluide.