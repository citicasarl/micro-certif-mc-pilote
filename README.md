# Vérificateur Open Badges 3.0

Outil gratuit pour **lire et contrôler un badge numérique Open Badges 3.0** directement dans le navigateur.

**Utiliser l'outil en ligne : https://github.com/citicasarl/micro-certif-mc-pilote

Proposé par [Micro-Certif](https://www.micro-certif.com/), plateforme française d'émission de badges Open Badges 3.0.

## Ce que fait l'outil

- Lit un badge collé ou déposé : JSON, jeton JWT, image PNG ou SVG contenant les données du badge.
- Affiche le contenu en clair : badge, émetteur, bénéficiaire, dates de validité, critères, preuves.
- Contrôle la structure selon la spécification Open Badges 3.0 de 1EdTech : contextes, types, identifiant, émetteur, dates, bénéficiaire, réalisation certifiée, présence d'une signature.
- Indique si le badge est expiré ou pas encore valide.
- Permet de vérifier qu'une adresse e-mail correspond au bénéficiaire, y compris quand elle est enregistrée sous forme d'empreinte SHA-256.
- Reconnaît les badges Open Badges 2.0 et le signale.

Tout le traitement se fait dans le navigateur : le badge n'est envoyé nulle part.

## Limites

L'outil contrôle la structure du badge. Il ne vérifie pas la signature cryptographique et n'interroge pas le service de révocation de l'émetteur. Un badge bien formé n'est donc pas, à lui seul, une preuve d'authenticité.

## Installation

Un seul fichier, sans dépendance : `index.html`.

- **En local** : ouvrir `index.html` dans un navigateur.
- **GitHub Pages** : dans le dépôt, *Settings › Pages*, choisir la branche `main` et le dossier racine. L'outil est en ligne quelques minutes plus tard.
- **Sur votre site** : copier `index.html` sur n'importe quel hébergement en HTTPS.

## Licence

MIT. Voir le fichier `LICENSE`.

---

# Open Badges 3.0 Validator (English)

A free, browser-based tool to **read and check an Open Badges 3.0 credential**.

**Try it online: https://github.com/citicasarl/micro-certif-mc-pilote (interface in French)

Built by [Micro-Certif](https://www.micro-certif.com/), a French Open Badges 3.0 issuing platform.

## Features

- Accepts pasted or dropped credentials: JSON, JWT, or a baked PNG / SVG badge image.
- Shows the content in plain language: badge, issuer, recipient, validity dates, criteria, evidence.
- Checks the structure against the 1EdTech Open Badges 3.0 specification: contexts, types, id, issuer, dates, credential subject, achievement, presence of a proof.
- Flags expired and not-yet-valid badges.
- Checks whether an email address matches the recipient, including salted SHA-256 hashed identifiers.
- Detects Open Badges 2.0 assertions and says so.

Everything runs client-side: the badge never leaves the browser.

## Limitations

This tool checks structure only. It does not verify the cryptographic signature and does not query the issuer's revocation service.

## Setup

A single dependency-free file, `index.html`. Open it locally, or enable GitHub Pages on the `main` branch.

## License

MIT. See `LICENSE`.
