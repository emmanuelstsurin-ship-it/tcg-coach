---
name: diagnosis
description: Diagnostic profond du business pour trouver LE bottleneck qui bloque tout le reste. À utiliser quand le business stagne, quand l'utilisateur ne comprend pas pourquoi ça ne marche pas, quand un bottleneck vient d'être résolu, ou à chaque nouveau palier.
---

# Skill : Diagnosis

**Mission** : trouver le maillon le plus faible de la chaîne — le seul problème qui, s'il était réglé, débloquerait le plus de croissance. Avec des chiffres.

## Principe
Un business est une chaîne :

```
Trafic → Conversion → Livraison → Rétention → Recommandation
   ↑           ↑
 Offre (influence tout)       Entrepreneur (influence tout)
```

Le bottleneck est le maillon dont l'amélioration a le plus d'impact sur le CA. Améliorer autre chose est du gaspillage.

## Déroulé

### 1. Collecter les chiffres
Demande (une question à la fois, accepte les approximations) :
- CA des 3 derniers mois (tendance).
- Leads / prospects par mois, et d'où ils viennent.
- Nombre de conversations / calls de vente par mois.
- Nombre de nouveaux clients par mois.
- Prix / panier moyen.
- Combien de clients restent / rachètent. Durée de vie moyenne.
- Combien viennent par recommandation.
- Heures travaillées / semaine, capacité max de clients.

Mets à jour `Core/Business.md` avec chaque chiffre.

### 2. Calculer
- Taux de conversion = nouveaux clients ÷ leads.
- CA potentiel si chaque maillon était « normal ». Repères indicatifs :
  - Lead → call : 20-40 %
  - Call → client (offre high-ticket) : 20-35 %
  - Visite page → achat (e-commerce / produit) : 1-3 %
  - Churn mensuel (abonnement) : < 5-8 %
- Écart entre l'objectif (`Goal.md`) et la réalité : quel maillon, s'il était doublé, comblerait le plus l'écart ?

### 3. Tester les hypothèses dans cet ordre
1. **Modèle** : le marché a-t-il l'argent et la douleur ? (sinon → **find**)
2. **Entrepreneur** : sait-il quoi faire mais ne le fait pas ? (→ **mindset**)
3. **Trafic** : volume de leads trop faible pour l'objectif, même avec une conversion parfaite ? (→ **traffic**)
4. **Offre** : les gens viennent mais ne trouvent pas l'offre assez attractive / trop chère / floue ? (→ **offer**)
5. **Conversion** : l'offre est bonne mais le process de vente fuit ? (→ **funnel**)
6. **Livraison / rétention** : les clients partent, se plaignent, l'entrepreneur est saturé ? (→ **digestion**)
7. **Croissance** : tout fonctionne mais plafonne ? (→ **chase**)

Croise avec `Knowledge/Common_Problems.md`.

### 4. Annoncer
Format :
> **Ton bottleneck : [problème].**
> **Preuve** : [chiffres].
> **Pourquoi c'est lui et pas autre chose** : [raisonnement en 2 lignes].
> **Ce que ça vaut** : si on passe [métrique] de X à Y, ton CA passe de A à B.
> **Critère de résolution** : [chiffre cible].

### 5. Documenter
- Réécris `Core/Diagnosis.md` (bottleneck + autres problèmes classés par impact).
- Pour un diagnostic complet, crée un rapport `Output/AAAA-MM-JJ_diagnostic.md` (chiffres, analyse, bottleneck, plan).
- Enchaîne avec **organize** pour transformer le diagnostic en plan, ou directement avec le skill du bottleneck.
