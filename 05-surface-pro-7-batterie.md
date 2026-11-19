# Fiche 05 : Surface Pro 7, batterie non détectée

<img src="https://img.shields.io/badge/R%C3%A9par%C3%A9-2E8B57?style=flat-square" alt="Réparé">

**Date :** novembre 2026 · **Appareil :** Microsoft Surface Pro 7 (modèle 1866), Windows 11, UEFI 23.101.140 · **Résultat :** Réparé (remplacement de la carte mère)

## Symptôme

Branchée, Windows affiche la batterie à 100 % mais elle ne se charge pas. Débranchée, la Surface s'éteint immédiatement, et parfois même en restant branchée. La batterie avait déjà été remplacée avant l'intervention, sans effet.

## Tests effectués

1. Chargeur retiré : arrêt immédiat. Rebranchée, la jauge revient à 100 % : la valeur affichée ne reflète pas une batterie utilisable
2. Paramètres d'alimentation : économiseur d'énergie actif, sans lien avec la panne
3. Rapport de batterie `powercfg /batteryreport` : emplacement « SurfaceBattery » détecté mais aucune donnée (fabricant, chimie et capacités vides, numéro de série par défaut `0000007000`). L'historique montre une seule lecture de 100 % pour 4 160 mWh, environ un dixième de la capacité normale : la jauge est déréglée
4. Remplacement du connecteur de batterie, nouveau rapport : toujours vide
5. Mises à jour Windows et micrologiciel : aucun changement
6. Chargeur d'origine à la place du premier : même comportement
7. Batterie essayée dans un autre appareil : elle s'y charge normalement, elle est hors de cause
8. Inspection de la carte mère : ni corrosion, ni trace de liquide, ni composant brûlé ; pâte thermique sèche

## Cause

Deux batteries et deux connecteurs donnaient le même résultat, et la batterie fonctionnait dans un autre appareil : la panne venait de la carte mère, dans le circuit qui lit et charge la batterie.

## Solution

Remplacement de la carte mère par une carte de Surface Pro 7. Le rapport de batterie lit enfin la batterie : fabricant, chimie lithium-ion, capacité d'origine 43 200 mWh, 135 cycles, vrai numéro de série, et la jauge affiche une valeur réelle.

## Ce que j'en retiens

Le rapport de batterie Windows montre si le système communique vraiment avec la batterie, quelle que soit la jauge. Croiser les pièces (la batterie dans un autre appareil) évite de remplacer une pièce saine, et on va toujours du moins coûteux au plus coûteux avant de toucher à la carte mère.

---

[← Retour au journal](README.md)
