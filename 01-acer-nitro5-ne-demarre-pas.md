# Fiche 01 : Acer Nitro 5 qui ne démarre pas

<img src="https://img.shields.io/badge/R%C3%A9par%C3%A9-2E8B57?style=flat-square" alt="Réparé">

**Date :** octobre 2026 · **Appareil :** Acer Nitro 5 AN515-55-75J1 (2021) · **Résultat :** Réparé

## Symptôme

Chargeur branché, voyant rouge. Au bouton d'alimentation, le voyant s'allume un instant puis s'éteint. Les ventilateurs ne tournent pas.

## Tests effectués

1. Boîtier ouvert, inspection visuelle du refroidissement (hypothèse de surchauffe) : rien de concluant
2. Batterie et SSD retirés : même comportement
3. Configuration minimale, une seule barrette de RAM : même comportement
4. Pile CMOS débranchée, chargeur seul : les ventilateurs et le rétroéclairage du clavier répondent
5. Pile CMOS rebranchée : le portable finit par démarrer normalement

## Cause

Paramètres du BIOS corrompus. Le retrait de la pile CMOS a réinitialisé le BIOS.

## Solution

Réinitialisation du BIOS par débranchement de la pile CMOS, puis remontage complet et test de démarrage.

## Ce que j'en retiens

Tester en configuration minimale élimine vite la RAM et le stockage. Quand rien ne change, penser au BIOS avant de soupçonner la carte mère.

---

[← Retour au journal](README.md)
