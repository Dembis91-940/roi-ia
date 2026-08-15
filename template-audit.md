# Template d'audit ROI IA — PME de 10 à 200 salariés

> **Usage** : ce template est pré-rempli avec les questions d'entretien, la grille de notation et la grille de calcul.
> Une **version remplie** (entreprise fictive « Menuiserie Dubois ») est fournie en exemple à la fin de chaque partie.
> Durée cible de l'audit terrain : **2 h** (1 h d'entretiens + 1 h de chiffrage).

---

## 1. En-tête de l'audit

| Champ | Réponse |
|---|---|
| Entreprise | |
| Secteur d'activité | |
| Effectif | |
| Chiffre d'affaires annuel | |
| Interlocuteur(s) | |
| Date de l'audit | |
| Auditeur | |
| Nombre d'outils IA recensés | |
| Coût mensuel total des abonnements | |

**Version remplie (exemple fictif)**

| Champ | Réponse |
|---|---|
| Entreprise | Menuiserie Dubois |
| Secteur d'activité | Fabrication artisanale / pose |
| Effectif | 34 |
| Chiffre d'affaires annuel | 3 200 000 € |
| Interlocuteur(s) | A. Dubois (gérant), C. Petit (commerciale), R. Ndiaye (atelier) |
| Date de l'audit | 12/08/2026 |
| Auditeur | ROI·IA |
| Nombre d'outils IA recensés | 6 |
| Coût mensuel total des abonnements | 642 € |

---

## 2. Inventaire des outils IA

Pour chaque outil : une ligne. Si un outil est payé mais inutilisé depuis plus de 30 jours, le mentionner en colonne « Statut ».

| Outil | Service principal | Nb d'utilisateurs actifs | Coût mensuel | Usage principal | Statut |
|---|---|---|---|---|---|
| | | | | | ☐ actif ☐ dormant ☐ redondant |
| | | | | | ☐ actif ☐ dormant ☐ redondant |
| | | | | | ☐ actif ☐ dormant ☐ redondant |
| | | | | | ☐ actif ☐ dormant ☐ redondant |
| | | | | | ☐ actif ☐ dormant ☐ redondant |
| **Total** | | | **€** | | |

**Version remplie (exemple fictif)**

| Outil | Service principal | Nb d'utilisateurs actifs | Coût mensuel | Usage principal | Statut |
|---|---|---|---|---|---|
| Assistant de rédaction IA (n°1) | Commercial | 3 | 39 € | Réponses aux appels d'offres, e-mails | ☒ actif |
| Générateur d'images IA | Marketing | 1 | 28 € | Visuels de chantiers | ☐ actif ☒ dormant |
| CRM avec IA intégrée | Commercial | 4 | 180 € | Qualification de leads | ☒ actif |
| Outil de comptes rendus IA | Direction | 2 | 45 € | CR de réunions, PV de chantier | ☒ actif |
| Automatisation no-code | Administratif | 1 | 120 € | Relances devis, classement factures | ☐ actif ☒ sous-utilisé |
| Assistant de devis IA | Atelier / Devis | 3 | 230 € | Génération et vérification des devis | ☒ actif |
| **Total** | | | **642 €** | | |

---

## 3. Grille de calcul (la formule)

### 3.1 Paramètres de référence

| Paramètre | Valeur par défaut | Commentaire |
|---|---|---|
| Coût chargé moyen d'un salarié PME | **40 €/h** | ≈ salaire brut moyen + charges patronales (ajustable) |
| Taux de réallocation du temps gagné | **65 %** | tout le temps gagné n'est pas réinvesti dans du travail productif |
| Semaines par mois | 4,33 | 52 semaines / 12 mois |
| Gain qualité (erreurs évitées) | 0,1 % à 0,8 % du CA mensuel | selon la fréquence de mesure constatée |

### 3.2 Grille par outil ou par tâche

Pour chaque ligne, calculer :

- **Heures gagnées / mois** = heures gagnées / semaine × 4,33
- **Valeur du temps** = heures gagnées / mois × 40 €/h × 65 %
- **ROI** = (gain mensuel − coût mensuel) / coût mensuel × 100

| Tâche / outil | Service | Heures gagnées / semaine | Coût mensuel | Valeur du temps (€/mois) | Gain net (€/mois) | ROI |
|---|---|---|---|---|---|---|
| | | | | | | |
| | | | | | | |
| | | | | | | |
| | | | | | | |
| **Total** | | | **€** | **€** | **€** | |

### 3.3 Version remplie (exemple fictif — extrait)

| Tâche / outil | Service | Heures gagnées / semaine | Coût mensuel | Valeur du temps (€/mois) | Gain net (€/mois) | ROI |
|---|---|---|---|---|---|---|
| Devis générés et vérifiés (IA devis) | Atelier | 12 h | 230 € | 12 × 4,33 × 40 × 65 % = **1 351 €** | **+1 121 €** | **+487 %** |
| Réponses aux appels d'offres (rédaction IA) | Commercial | 6 h | 39 € | 6 × 4,33 × 40 × 65 % = **675 €** | **+636 €** | **+1 631 %** |
| Comptes rendus et PV (IA CR) | Direction | 3 h | 45 € | 3 × 4,33 × 40 × 65 % = **338 €** | **+293 €** | **+651 %** |
| Relances devis automatisées (no-code) | Administratif | 4 h | 120 € | 4 × 4,33 × 40 × 65 % = **450 €** | **+330 €** | **+275 %** |
| Qualification de leads (CRM IA) | Commercial | 2 h | 180 € | 2 × 4,33 × 40 × 65 % = **225 €** | **+45 €** | **+25 %** |
| Générateur d'images | Marketing | 0 h (dormant) | 28 € | 0 € | **−28 €** | **−100 %** |
| **Total** | | **27 h** | **642 €** | **3 039 €** | **+2 397 €** | **+373 %** |

> **Lecture** : la menuiserie gagne ≈ **2 400 €/mois** malgré elle. Le seul gisement immédiat : couper le générateur d'images dormant (28 €/mois) ou le réattribuer, et mesurer le taux de réallocation réel (65 % retenu par prudence).

---

## 4. Questionnaire d'entretien (10 questions)

Les questions 1 à 10 correspondent aux critères notés du calculateur en ligne. Chaque réponse vaut de 0 à 4 points (voir grille de notation en partie 5).

**Adoption**
1. Combien d'outils IA l'entreprise utilise-t-elle aujourd'hui ? (abonnements actifs)
2. Quelle part de l'équipe utilise l'IA au quotidien ? (personnes réelles, pas de licences)

**Investissement**
3. Quel budget mensuel les abonnements IA représentent-ils ? (licences + API, hors salaires)

**Impact**
4. Combien d'heures par semaine l'équipe gagne-t-elle grâce à l'IA ? (somme sur tous les services)
5. Combien de tâches répétitives sont automatisées ou semi-automatisées ?
6. Quelle est la valeur des erreurs évitées ou de la hausse de qualité constatée ? (question ouverte, à recouper avec le taux d'erreur historique)

**Structuration**
7. Comment l'IA est-elle intégrée aux processus ? (usage informel → workflows documentés → processus clés)
8. Existe-t-il un budget ou un responsable dédié à l'IA ?

**Mesure**
9. À quelle fréquence mesure-t-on les erreurs évitées / la hausse de qualité ?
10. À quelle fréquence mesure-t-on le ROI des outils IA ?

**Contexte (non noté, sert au chiffrage)**
11. Quel est le chiffre d'affaires annuel ? (benchmark + valeur qualité)
12. Quel est le coût chargé moyen d'un salarié de l'entreprise ? (ajuste le paramètre 40 €/h)

---

## 5. Grille de notation

Chaque question notée vaut **0 à 4 points**. Score de maturité = total / 36 × 100 (9 questions notées).

| # | Critère | 0 pt | 1 pt | 2 pts | 3 pts | 4 pts | Note |
|---|---|---|---|---|---|---|---|
| 1 | Outils IA actifs | aucun | 1-2 | 3-5 | 6-10 | > 10 | |
| 2 | Équipe utilisant l'IA au quotidien | personne | 1-3 pers. | 4-10 pers. | 11-50 pers. | > 50 pers. | |
| 3 | Budget mensuel IA | < 100 € | 100-500 € | 500-2 k€ | 2-5 k€ | > 5 k€ | |
| 4 | Heures gagnées / semaine | 0 h | < 5 h | 5-15 h | 15-40 h | > 40 h | |
| 5 | Tâches automatisées | aucune | 1-3 | 4-10 | 11-25 | > 25 | |
| 6 | Mesure des erreurs / qualité | jamais | rarement | parfois | régulièrement | systématiquement | |
| 7 | Intégration aux processus | ponctuel | outils isolés | workflows doc. | processus clés | pilier org. | |
| 8 | Budget / responsable dédié | aucun | budget informel | budget dédié | responsable identifié | responsable + budget | |
| 9 | Fréquence de mesure du ROI | jamais | occasionnel | trimestriel | mensuel | continu | |
| 10 | **Total (/36)** | | | | | | |
| 11 | **Score de maturité (/100)** | | | | | | |

**Version remplie (exemple fictif) — Menuiserie Dubois : 20/36 ≈ 56/100 (« Maturité en construction »)**

| Dimension | Note /100 | Lecture |
|---|---|---|
| Adoption (Q1, Q2) | 50 | 6 outils, 3 services ; l'image IA dort |
| Investissement (Q3) | 25 | 642 €/mois, sans pilotage |
| Impact (Q4, Q5) | 75 | 27 h/semaine gagnées, 8 tâches automatisées |
| Mesure (Q6, Q9) | 38 | la qualité n'est pas suivie, le ROI jamais |
| Structuration (Q7, Q8) | 63 | processus documentés au commercial uniquement, pas de pilote |

---

## 6. Synthèse et recommandations

| Priorité | Action | Effort | Gain mensuel estimé | ROI attendu | Délai |
|---|---|---|---|---|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |

**Version remplie (exemple fictif)**

| Priorité | Action | Effort | Gain mensuel estimé | ROI attendu | Délai |
|---|---|---|---|---|---|
| 1 | Couper ou réattribuer le générateur d'images dormant | 15 min | +28 € | ∞ (coût nul) | J+2 |
| 2 | Mettre en place un suivi mensuel du temps gagné (tableau 3 indicateurs) | 1 h/mois | +250 € (via réallocation) | +42 % | J+7 |
| 3 | Étendre l'IA de devis au service pose (2 personnes) | 4 h | +350 € | +152 % | J+15 |
| 4 | Nommer un pilote IA (10 % du temps de la commerciale) | 0 € | +150 € | — | J+21 |

---

## 7. Annexe — tableau de suivi à 30 jours

| KPI | Valeur au jour J | Valeur à J+30 | Écart |
|---|---|---|---|
| Coût mensuel des abonnements | | | |
| Heures gagnées / semaine | | | |
| Tâches automatisées | | | |
| Erreurs évitées (nombre / valeur €) | | | |
| Gain net mensuel | | | |
