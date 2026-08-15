# ROI·IA — Audit & Calculateur de ROI IA pour PME

Site vitrine + outil de diagnostic pour un solopreneur français. Le produit aide les PME de **10 à 200 salariés** à savoir si leurs outils IA rapportent ou coûtent, en euros par mois.

## Offres

| Offre | Prix | Contenu |
|---|---|---|
| **Audit rapide** | **0 €** | Quiz de 10 questions → score de maturité sur 100, estimation €/mois gagnés ou perdus, 3 recommandations personnalisées. 100 % dans le navigateur, sans inscription. |
| **Rapport PDF complet** | **49 €** | Tout l'audit gratuit + analyse service par service, grille de calcul personnalisée (coût €/h réel), benchmark PME, 10 recommandations priorisées par ROI. Livré sous 48 h ouvrées. |
| **Pack direction** | **99 €** | Rapport complet inclus + plan d'action 30 jours semaine par semaine + 1 session d'accompagnement de 45 min (visio) + suivi des KPIs à J+30. |

Le paiement se fait par **lien sécurisé** (carte ou virement) envoyé par e-mail après commande. Les commandes et les demandes de contact transitent par **EmailJS** (aucun serveur à héberger).

## Contenu du dossier

```
~/Documents/livrables/roi-ia/
├── index.html          # Page d'accueil : hero + mockup dashboard animé (compteurs,
│                       #   jauge SVG, barres, sparkline), méthode, 3 offres, FAQ,
│                       #   formulaire de contact EmailJS
├── calculateur.html    # L'outil : quiz 10 questions → score de maturité (jauge animée),
│                       #   impact financier estimé €/mois, notes par dimension,
│                       #   3 recommandations personnalisées, formulaire de commande
│                       #   EmailJS (49 € / 99 €), impression PDF du résultat
├── template-audit.md   # Template d'audit pré-rempli : en-tête, inventaire des outils,
│                       #   grille de calcul (formule + exemple chiffré), questionnaire,
│                       #   grille de notation 0-4, synthèse, suivi à 30 jours
├── roi-ia-1.md         # Article SEO : « Qu'est-ce que le ROI d'un outil IA ? »
├── roi-ia-2.md         # Article SEO : « Les 5 indicateurs pour mesurer l'IA »
├── roi-ia-3.md         # Article SEO : « Erreur n°1 : mesurer les postes remplacés
│                       #   au lieu de la capacité »
├── roi-ia-4.md         # Article SEO : « Calculer le ROI d'un chatbot »
├── roi-ia-5.md         # Article SEO : « IA et productivité : le capability yield »
└── README.md           # Ce fichier
```

## Configuration EmailJS

Les deux formulaires utilisent le même service et le même template :

- **Service ID** : `service_cy1ytdb`
- **Template ID** : `template_xpo58cv`
- **Public key** : `8Pui4ZEqxW2jRVF7h`
- **Variables envoyées** : `{ site, name, email, question }`

Le template e-mail doit définir les variables `site`, `name`, `email` et `question` (dans EmailJS Studio → Templates → votre template). `site` = nom de l'entreprise, `question` = texte libre ou intitulé de commande (ex. « Commande — Rapport PDF complet (49 €) »).

Pour changer le destinataire : EmailJS Studio → Templates → votre template → champ « To email ».

## Méthodologie du calculateur

**Score de maturité (0-100)** : 9 questions notées de 0 à 4 points, réparties en 4 dimensions — Adoption, Structuration, Mesure, Impact. Le CA (question 6) et l'investissement (question 2) servent au chiffrage financier, pas au score.

**Estimation financière mensuelle** :

- Coût = milieu de fourchette du budget mensuel déclaré.
- Valeur du temps = heures gagnées/semaine × 4,33 × **40 €/h** (coût chargé moyen PME) × **65 %** (taux de réallocation).
- Valeur qualité = 0,1 à 0,8 % du CA mensuel selon la fréquence de mesure des erreurs.
- **Gain ou perte net** = valeur totale − coût. ROI = net ÷ coût × 100.

**Recommandations** : moteur de règles — les dimensions les plus faibles déclenchent des recommandations ciblées, complétées par des règles globales (abonnements dormants, premier use case, industrialisation si score ≥ 75). Toujours 3 recommandations.

## Design

- Palette **émeraude / teal** sur fond très sombre `#0a1412` : vert menthe `#34d399`, turquoise `#2dd4bf`, émeraude `#10b981`.
- Architecture « tableau de bord fintech » : header minimal, mockup dashboard animé dans le hero (compteurs JS, jauge SVG, barres, sparkline), sections en grille fine, grille de fond CSS (aucun canvas, aucune particule).
- Typographie : Space Grotesk (titres), Inter (texte), JetBrains Mono (chiffres).
- Accessibilité : focus visibles, `prefers-reduced-motion` respecté, navigation clavier du quiz.

## Mise en ligne (aucun GitHub)

1. Hébergez le dossier sur n'importe quel hébergement statique (Netlify Drop, Vercel, OVH, Infomaniak…).
2. Les liens internes sont relatifs : `index.html`, `calculateur.html`, `roi-ia-*.md`.
3. Pour un rendu propre des articles, convertissez les `.md` en HTML (ex. `npx markdown-it-cli` ou pandoc) et mettez à jour les liens du footer dans `index.html`.
4. Pensez à un nom de domaine en `.fr` et à la page Mentions légales (obligatoire : identité, SIREN, hébergeur).

## Personnalisation rapide

- **Prix** : recherchez `49&nbsp;€` et `99&nbsp;€` dans `index.html` et `calculateur.html`.
- **Coût horaire** : constante `HOURLY_VALUE` (40) dans `calculateur.html`, en tête du bloc JS.
- **Taux de réallocation** : constante `REDEPLOY_RATE` (0.65).
- **Textes** : sections `QUESTIONS` (quiz) et `POOLS`/`GLOBALS` (recommandations) dans `calculateur.html`.

## Notes

- Le calculateur fonctionne à 100 % en JavaScript côté client ; les réponses sont conservées en `localStorage` (reprise possible après actualisation, bouton « Recommencer » pour effacer).
- Aucune donnée n'est envoyée pendant le quiz. Seuls les formulaires (contact et commande) appellent EmailJS.
- Les exemples chiffrés (dashboard du hero, template d'audit) sont des illustrations ; les hypothèses de calcul sont affichées dans l'interface.
