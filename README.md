# Test Essentiel — Loksite

Repo client Loksite pour le compte de test **Test Essentiel** (plan Essentiel — utilisé pour valider le flux d'onboarding restaurant).

## Fichiers du repo

| Fichier | Rôle |
|---|---|
| `vitrine.html` | Site public — vitrine du restaurant, servi via GitHub Pages |
| `vitrine-preview.html` | Copie de travail utilisée par l'éditeur intégré (LKE) dans l'espace client avant publication. "Enregistrer" écrit ici, "Publier" copie ce fichier vers `vitrine.html` |
| `espace.html` | Espace client Loksite (connexion, tableau de bord, modification du site, messages, réservations, analytics…) |
| `politique-de-confidentialite.html` | Page de politique de confidentialité liée depuis la vitrine |

## Identité du client de test

| Champ | Valeur |
|---|---|
| Nom | Test Essentiel |
| Email | axelmerlot15@gmail.com |
| Ville | Lille |
| Téléphone | 07 49 17 54 70 |
| Type d'activité | Restaurant |
| Plan | Essentiel — 29€/mois |

## Déploiement

Ce repo est servi tel quel via **GitHub Pages** (branche `main`, racine `/`).

- Vitrine publique : `https://<utilisateur>.github.io/<repo>/vitrine.html`
- Espace client : `https://<utilisateur>.github.io/<repo>/espace.html`

## Backend

- **Supabase** : `qhnofvfgutsdgbfwhupg.supabase.co` — table `profiles`, colonne `github_repo` pointant vers ce repo
- **n8n** : workflow "Loksite — Assistant IA" pour la publication et les modifications via l'éditeur (selon le plan souscrit)

## Notes

Ce compte est un compte de **test** servant à valider le parcours d'onboarding complet (création Supabase → création repo GitHub → connexion espace client) pour le plan **Essentiel**, qui ne donne pas accès aux modifications par IA (réservé aux plans Standard et Premium).
