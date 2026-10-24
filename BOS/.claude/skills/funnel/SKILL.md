---
name: funnel
description: Diagnostiquer et réparer la conversion. À utiliser quand l'utilisateur a du trafic ou des leads mais pas assez de ventes, quand les calls de vente ne closent pas, quand la page de vente ou le site ne convertit pas, ou quand il n'y a pas de suivi des prospects.
---

# Skill : Funnel

**Mission** : trouver la plus grosse fuite entre « quelqu'un découvre l'offre » et « il paie », et la colmater.

## Déroulé

### 1. Cartographier le funnel
Écris chaque étape réelle avec son volume (mois dernier). Exemple :

```
Vues / visiteurs   2 000
  → Leads (DM, inscrits, formulaires)   80   (4 %)
  → Calls réservés   25   (31 %)
  → Calls honorés   18   (72 %)
  → Clients   3   (17 %)
```

S'il n'y a pas de chiffres : première action = les mesurer pendant 7 jours.

### 2. Trouver la fuite
Compare chaque taux aux repères (voir **diagnosis**) et au potentiel. La fuite = l'étape où l'écart est le plus grand **et** où une amélioration a le plus d'impact sur le nombre de clients.

### 3. Réparer selon l'étape

**Visiteur → Lead**
- Promesse claire et spécifique en haut (titre = résultat pour l'avatar).
- Un seul appel à l'action.
- Lead magnet qui résout un vrai petit problème.
- Preuves (témoignages, chiffres, captures).

**Lead → Call / achat**
- Réponse rapide (< 1 h idéalement).
- Séquence de suivi : J+1, J+3, J+7, J+14. Utile, pas insistant.
- Qualification : budget, urgence, décisionnaire.

**Call → Client** — structure de call :
1. Cadre (durée, objectif, « à la fin on voit si ça a du sens »).
2. Situation actuelle — chiffres.
3. Situation désirée — chiffres, pourquoi maintenant.
4. Obstacles — pourquoi pas encore atteint.
5. Coût de l'inaction.
6. Présentation de l'offre **reliée à ce qu'il a dit**.
7. Prix, silence, traitement des objections.
8. Close ou prochaine étape datée.

Règle : 70 % écoute, 30 % parole. Pas de coaching gratuit pendant le call.

**Objections** — liste les 5 objections les plus fréquentes et écris la réponse à chacune. Récurrentes → les traiter en amont (offre, contenu, page).
- « C'est trop cher » → valeur mal démontrée ou mauvaise cible.
- « Je dois réfléchir » → demander « à quoi précisément ? », souvent une objection cachée.
- « Je dois en parler à mon conjoint / associé » → l'inclure dans le call la prochaine fois.
- « C'est pas le moment » → coût de l'inaction.

**Page de vente** — structure : titre résultat → problème → mécanisme / solution → preuves → offre détaillée → bonus → garantie → prix → FAQ / objections → CTA (répété).

### 4. Livrables (dans `Output/`)
Selon la fuite : script de call, séquence de relance, réécriture de page, tableau de suivi du funnel, réponses aux objections.

### 5. Mesurer l'effet
Fixer le taux cible et re-mesurer après 2 semaines.

## Mise à jour des fichiers
- `Core/Business.md` : taux de conversion de chaque étape.
- `Core/Diagnosis.md` : fuite identifiée, critère de résolution.
- `Core/Actions.md` : correction + date de re-mesure.
