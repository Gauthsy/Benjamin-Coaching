# Ben Fit Paris — déploiement

État de cette livraison : **prête à mettre à jour** sur le dépôt GitHub et le projet Vercel existants. Ne pas créer un nouveau projet Vercel.

## Avant le push

- Vérifier rapidement la home en mobile et desktop.
- Tester le formulaire de contact avec une adresse réelle.
- Vérifier les liens Instagram et les quatre Reels.
- Ne pas ajouter de fichier d’asset non utilisé au dépôt.

## Déploiement

Le site est statique : déployer le contenu de ce dossier à la racine du dépôt GitHub déjà connecté à Vercel.

État Git vérifié dans cette livraison :

- branche locale : `main` ;
- remote `origin` : `https://github.com/Gauthsy/Benjamin-Coaching.git` ;
- `main` suit `origin/main`.

Avant le push, dans le **projet Vercel existant**, vérifier une dernière fois dans Settings → Git que ce dépôt est toujours connecté et que `main` est bien la branche de production. Il n'est pas nécessaire d'importer le dépôt ou de créer un nouveau projet Vercel.

Workflow recommandé :

1. `git status`
2. `git add .`
3. `git commit -m "Update Ben Fit Paris"`
4. `git push`
5. Ouvrir le projet Vercel existant et vérifier le nouveau déploiement de production déclenché par le push sur la branche de production.

Le dossier `.git` et l’historique existant sont conservés dans cette livraison.

## Domaine

Le domaine canonique est `https://benfitparis.fr/`.

Dans Vercel, conserver :

- `benfitparis.fr` comme domaine principal ;
- `www.benfitparis.fr` redirigé en permanence vers `benfitparis.fr` ;
- l’ancienne URL Vercel redirigée vers le domaine final si elle reste publiquement accessible.

## Contrôles après déploiement

- `https://benfitparis.fr/`
- `https://benfitparis.fr/robots.txt`
- `https://benfitparis.fr/sitemap.xml`
- favicon dans un nouvel onglet et après ajout à l’écran d’accueil mobile ;
- formulaire Formspree ;
- liens Instagram ;
- affichage Open Graph lors du partage du domaine ;
- Google Search Console : vérifier que le sitemap reste accepté et demander une nouvelle exploration si nécessaire.

## Sécurité / technique déjà configurées

- HTTPS/HSTS via Vercel + headers projet ;
- Content Security Policy ;
- `X-Content-Type-Options: nosniff` ;
- protection contre l’intégration en iframe ;
- politique de référent et permissions navigateur ;
- `robots.txt`, sitemap, canonical, Open Graph, Twitter Card et JSON-LD ;
- Vercel Web Analytics ;
- formulaire Formspree avec champ anti-spam.

## Informations légales à confirmer avec le client

Le site contient déjà les informations professionnelles disponibles. Si le client souhaite compléter les mentions légales, confirmer avant publication publique de nouvelles données :

- identité légale complète de l’éditeur ;
- coordonnées professionnelles publiques éventuelles ;
- adresse ou informations de domiciliation à publier, si nécessaire ;
- lien Google Business Profile, s’il existe et doit être mis en avant.
