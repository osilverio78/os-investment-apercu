# Cabinet OS Investment — site

Site vitrine du Cabinet OS Investment (expertise comptable, commissariat aux comptes, fiscalité et conseil au dirigeant).

## Contenu
- `index.html` : le site complet (une page, FR/EN), généré depuis la maquette Claude Design.
- `netlify/functions/chat.mjs` : assistant de discussion (`/api/chat`), Claude Haiku, nourri uniquement du contenu du site, réponses cadrées (pas de conseil personnalisé, pas de placements, aucun montant d'honoraires), aucune conversation enregistrée. Fichier généré à partir du contenu du site : à régénérer après chaque modification du contenu.
- Sans la fonction (GitHub Pages, aperçu Claude), l'assistant répond avec sa base de réponses intégrée.

## Hébergement
- Netlify (avec l'assistant IA) : https://os-investment.fr (alias : www.os-investment.fr, os-inv.fr, www.os-inv.fr, os-investment-apercu.netlify.app).

## Variables d'environnement Netlify
| Nom | Rôle |
|---|---|
| `ANTHROPIC_API_KEY` | Clé API Anthropic de l'assistant (`/api/chat`) |
| `ALLOWED_HOSTS` | Optionnel : domaines autorisés supplémentaires, séparés par des virgules (ex. domaine définitif) |

Aucun secret ne doit être écrit dans le code.

## Référencement
Site ouvert à l'indexation depuis le 24/10/2026 : `robots.txt` autorise, `sitemap.xml` liste les pages, adresse canonique https://os-investment.fr/.

## Formulaire de contact
Netlify Forms, formulaire `contact` (formulaire statique caché dans `index.html` pour la détection, envoi en JavaScript vers `/`). Notification par e-mail réglée dans Netlify → Forms → Form notifications.
