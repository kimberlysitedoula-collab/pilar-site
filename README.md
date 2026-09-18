# Pílar — site web

Site vitrine de Pílar, centre féministe et inclusif (fertilité, grossesse, parentalité).

## Pages (toutes reliées par le menu)

- `index.html` — Accueil
- `whatispilar.html` — What is Pílar
- `offre.html` — Offerings
- `qui-sommes-nous.html` — About / Qui sommes-nous
- `contact.html` — Contact

Chaque page contient ses textes, images et vidéos intégrés dans le fichier. La navigation
entre les pages se fait via le menu (header) et le pied de page (footer).

## Mise en ligne (Cloudflare Pages)

**Option A — connexion Git (déploiement automatique)**
1. Pousser ce dépôt sur GitHub.
2. Cloudflare → *Workers & Pages* → *Create* → *Pages* → *Connect to Git*.
3. Sélectionner le dépôt. Aucune commande de build. *Build output directory* : `/` (racine).
4. *Save and Deploy*. À chaque `git push`, le site se met à jour tout seul.

**Option B — dépôt direct (glisser-déposer)**
1. Cloudflare → *Workers & Pages* → *Create* → *Pages* → *Upload assets*.
2. Glisser les 5 fichiers `.html` **ensemble**, puis *Deploy*.

> Important : déposer les cinq pages en même temps pour que les liens fonctionnent.
> Le fichier d'accueil doit s'appeler `index.html`.

## Domaine

Brancher `pilar.center` via l'onglet *Custom domains* du projet Cloudflare Pages.

## Mettre à jour

Modifier la page voulue, puis `git commit` + `git push` (Option A) ou re-déposer les fichiers (Option B).
