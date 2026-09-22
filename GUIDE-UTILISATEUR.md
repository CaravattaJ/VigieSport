# Guide d'utilisation — VigieSport BFC

Ce guide explique, étape par étape, comment ouvrir l'application et l'utiliser au quotidien. Il ne suppose aucune connaissance technique.

**Ce qu'il faut retenir avant de commencer :** cette application n'est pas installée sur votre ordinateur comme un vrai logiciel — c'est un simple fichier qui s'ouvre dans votre navigateur (Chrome, Edge...). Vos décisions ne sont pas automatiquement partagées avec vos collègues : c'est vous qui, à la fin de chaque session, devez enregistrer un fichier dans un dossier commun pour que l'équipe en profite. Ce point est expliqué en détail plus bas.

---

## 1. Ouvrir l'application (aucune installation)

Vous n'avez rien à installer, et vous n'avez pas besoin de droits administrateur.

- **Sous Windows** : double-cliquez sur le fichier `ouvrir-veille-sports.bat`, dans le dossier de l'application.
- **Si ce fichier n'existe pas ou ne fonctionne pas** : ouvrez votre navigateur (Chrome ou Edge de préférence), puis ouvrez directement le fichier `index.html` du même dossier (glissez-le dans une fenêtre du navigateur, ou faites clic droit → Ouvrir avec → votre navigateur).

L'application s'affiche. Vous êtes prêt à commencer.

> Si rien ne se charge (page blanche, message d'erreur réseau), parlez-en à votre service informatique : un pare-feu d'entreprise bloque parfois les échanges nécessaires. Les détails techniques à leur transmettre sont dans le fichier `README.md`.

---

## 2. La toute première fois que vous utilisez l'application

La première utilisation est particulière : il n'existe encore **aucune base commune** avec les décisions de l'équipe. C'est vous qui allez la créer. Suivez ces étapes dans l'ordre.

### Étape 1 — Lancez une recherche

Une date est déjà proposée dans le champ **« Chercher les structures créées depuis le »**, et le département **Côte-d'Or** est déjà coché. Vous pouvez les modifier si besoin (par exemple cocher d'autres départements de la région).

Cliquez sur le bouton orange **« Rechercher »**.

Patientez : l'application interroge plusieurs sources officielles. Cela peut prendre de quelques secondes à quelques minutes selon la période et le nombre de départements choisis.

### Étape 2 — Qualifiez les structures trouvées

Une liste de structures sportives récemment créées apparaît. Pour chacune, une **case « Décision »** vous permet de choisir ce que vous en pensez :

| Décision | Signification |
|---|---|
| **À qualifier** | Pas encore regardée (choix par défaut) |
| **À contrôler** | Mérite une visite ou une vérification |
| **Déjà connu** | Vous la connaissiez déjà |
| **Pas un lieu de pratique** | Ce n'est pas une vraie structure sportive (ex. juste un siège administratif) |
| **Hors périmètre** | Ne concerne pas votre service |

Pour chaque structure qui le mérite, cliquez sur son nom : cela ouvre une recherche Google dans un nouvel onglet, pratique pour vérifier de quoi il s'agit avant de choisir une décision. Vous pouvez aussi écrire une petite note libre sous la décision (par exemple « RDV pris le 12/10 »).

*Astuce : vous n'êtes pas obligé de tout qualifier en une seule fois. Vous pouvez vous arrêter et reprendre plus tard, tant que vous suivez bien l'étape 3 ci-dessous avant de fermer l'application.*

### Étape 3 — Enregistrez votre travail (étape la plus importante)

C'est l'étape à ne jamais oublier, surtout la première fois.

1. Cliquez sur le bouton **« Enregistrer »**, en haut de la page.
2. Un fichier nommé `veille-sports-partage.json` est téléchargé par votre navigateur (en général dans votre dossier **Téléchargements**).
3. **Déplacez ce fichier** dans le dossier `sauvegarde`, situé juste à côté du fichier `index.html` de l'application.

C'est ce fichier, dans ce dossier précis, qui devient **la base commune de l'équipe**. Si ce dossier `sauvegarde` se trouve sur un espace réseau partagé (un dossier accessible à tous vos collègues), alors tout le monde pourra désormais repartir de votre travail.

> **Pourquoi faut-il le déplacer soi-même ?** C'est une règle de sécurité de tous les navigateurs : aucun site ni aucune application ne peut choisir où un fichier téléchargé atterrit sur votre ordinateur. Le geste manuel est donc obligatoire — mais il ne prend que quelques secondes.

Vous avez terminé votre première utilisation. La base commune existe maintenant.

---

## 3. Toutes les fois suivantes

À partir de la deuxième utilisation, la logique change : **vous ne repartez plus de zéro**, vous repartez du fichier que l'équipe a enregistré en dernier. Suivez ces étapes, dans cet ordre précis.

### Étape 1 — Chargez la base commune (à faire en tout premier, avant tout le reste)

1. Cliquez sur le bouton **« Charger »**, en haut de la page.
2. Sélectionnez le fichier `veille-sports-partage.json` qui se trouve dans le dossier `sauvegarde`.

Vous récupérez ainsi toutes les décisions déjà prises par vous-même et vos collègues lors des sessions précédentes.

> Ne sautez jamais cette étape : si vous lancez une recherche sans avoir chargé le fichier au préalable, vous risquez de re-qualifier des structures déjà traitées par un collègue, ou pire, d'écraser son travail en enregistrant par-dessus sans l'avoir récupéré.

### Étape 2 — Lancez une nouvelle recherche

Cliquez sur **« Rechercher »**. La date proposée par défaut correspond à votre dernière recherche : vous n'avez rien à changer sauf besoin particulier (par exemple une recherche plus large une fois par mois, voir l'aide dans l'application).

### Étape 3 — Qualifiez uniquement les nouvelles structures

Les structures déjà traitées gardent leur décision. Concentrez-vous sur les nouvelles.

*Astuce : utilisez le menu déroulant **« Toutes les décisions »** au-dessus du tableau pour n'afficher que les structures encore **« À qualifier »** — pratique pour ne pas se laisser distraire par ce qui est déjà traité.*

### Étape 4 — Enregistrez à nouveau, en écrasant l'ancien fichier

1. Cliquez sur **« Enregistrer »**.
2. Un nouveau fichier `veille-sports-partage.json` est téléchargé.
3. Placez-le dans le dossier `sauvegarde`, **à la place de l'ancien** (remplacez-le quand votre navigateur vous le demande).

Votre travail est maintenant disponible pour toute l'équipe, prêt à être chargé à la prochaine session — par vous ou par un collègue.

---

## 4. Comprendre le tableau de résultats

| Élément | À quoi ça sert |
|---|---|
| **Pastille de couleur (Confiance)** | Indique la fiabilité de la détection automatique : rouge/orange = très probablement sportif, jaune = probable, gris = à vérifier vous-même |
| **Nom de la structure** (cliquable) | Ouvre une recherche Google dans un nouvel onglet |
| **Icône 🏛** (à côté du nom, si présente) | Ouvre la fiche officielle de la structure (adresse, dirigeants...) sur l'Annuaire des Entreprises. N'apparaît que si la structure a un numéro SIRET ou SIREN |
| **Champ de recherche** (au-dessus du tableau) | Filtre la liste par nom, commune ou numéro SIRET |
| **Menu « Toutes les décisions »** | N'affiche que les structures d'un statut précis |
| **Case « Masquer les Faible »** | Cache les structures dont la confiance est faible, pour se concentrer sur l'essentiel |
| **Case à cocher (première colonne)** | Affiche uniquement les structures cochées sur la carte à droite |

---

## 5. La carte et le calcul d'itinéraire

Une carte reste visible en permanence à droite de l'écran, avec un point pour chaque structure localisée.

**Pour estimer un trajet entre plusieurs structures** (utile pour préparer une tournée de contrôle) :

1. Cochez au moins deux structures dans le tableau (première colonne), **dans l'ordre où vous comptez les visiter**.
2. Un encadré apparaît sous la carte avec la distance et la durée estimées du trajet routier.

*Attention : l'application calcule le trajet dans l'ordre exact où vous cochez les cases — elle ne cherche pas le trajet le plus court toute seule.*

---

## 6. Exporter un tableau Excel (CSV)

Le bouton **« Exporter en CSV »** télécharge un fichier tableur (compatible Excel) avec toutes les structures et leurs décisions — pratique pour un rapport ou une réunion. Ce fichier est indépendant du fichier `sauvegarde` : l'exporter ne remplace pas l'étape « Enregistrer ».

---

## 7. En cas de souci

| Problème | Solution |
|---|---|
| La page ne s'ouvre pas / reste blanche | Essayez de l'ouvrir avec un autre navigateur (Chrome ou Edge) |
| Message d'erreur réseau au lancement d'une recherche | Contactez votre service informatique (voir `README.md`) |
| Vous avez un doute sur vos dernières décisions | Rechargez le fichier du dossier `sauvegarde` : c'est la seule version fiable, partagée par toute l'équipe |
| Vous voulez repartir de zéro sur ce poste uniquement | Bouton **« Réinitialiser les données »**, tout en bas du bloc d'aide (n'efface que ce qui est affiché sur cet ordinateur, pas le fichier `sauvegarde`) |

---

## En résumé (mémo rapide)

- **Première fois** : Rechercher → Qualifier → **Enregistrer** → déposer le fichier dans `sauvegarde`.
- **Fois suivantes** : **Charger** le fichier de `sauvegarde` → Rechercher → Qualifier les nouveautés → **Enregistrer** → remplacer le fichier dans `sauvegarde`.
- Le dossier `sauvegarde` est la seule mémoire commune de l'équipe. Sans ce geste manuel, chaque poste travaille dans son coin.
