# Cabinet OS Investment — site (aperçu)

Site vitrine du Cabinet OS Investment (expertise comptable, commissariat aux comptes, fiscalité et conseil au dirigeant).

## Contenu
- `index.html` : le site complet (une page, FR/EN), généré depuis la maquette Claude Design.
- `netlify/functions/chat.mjs` : assistant de discussion (`/api/chat`), Claude Haiku, nourri uniquement du contenu du site, réponses cadrées (pas de conseil personnalisé, pas de placements, aucun montant d'honoraires), aucune conversation enregistrée. Fichier généré à partir du contenu du site : à régénérer après chaque modification du contenu.
- Sans la fonction (GitHub Pages, aperçu Claude), l'assistant répond avec sa base de réponses intégrée.

## Hébergement
- GitHub Pages : https://osilverio78.github.io/os-investment-apercu/ (statique, sans IA).
- Netlify (avec l'assistant IA) : site relié à ce dépôt, adresse prévue `os-investment-apercu.netlify.app`.

## Variables d'environnement Netlify
| Nom | Rôle |
|---|---|
| `ANTHROPIC_API_KEY` | Clé API Anthropic de l'assistant (`/api/chat`) |
| `ALLOWED_HOSTS` | Optionnel : domaines autorisés supplémentaires, séparés par des virgules (ex. domaine définitif) |

Aucun secret ne doit être écrit dans le code. Site non référencé (`noindex`).
