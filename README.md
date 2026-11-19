# Journal de dépannage

Fiches d'intervention tirées de mon stage de technicien informatique chez LaboPhone Inc., atelier de réparation (octobre – novembre 2026), dans le cadre du DEP Soutien informatique (ESIDEM, Montréal).

Chaque fiche suit le même ordre : **symptôme → tests → cause → solution → ce que j'en retiens**. Les informations des clients ne sont pas publiées.

| Fiche | Appareil | Problème | Résultat |
| --- | --- | --- | --- |
| [01](01-acer-nitro5-ne-demarre-pas.md) | Acer Nitro 5 AN515-55 | Ne démarre pas, ventilateurs muets | Réparé |
| [02](02-dell-optiplex-3020-windows11.md) | Dell OptiPlex 3020 | Mot de passe BIOS inconnu, installation de Windows 11 bloquée | Remis en service |
| [03](03-asus-cpu-fan-error.md) | PC Asus, carte P8H61-M PRO | Message « CPU FAN ERROR » | En cours |
| [04](04-portable-aucun-signe-de-vie.md) | Portable à deux SSD | Aucun voyant malgré 19 à 20 V au connecteur | En cours |
| [05](05-surface-pro-7-batterie.md) | Microsoft Surface Pro 7 | Batterie non détectée, arrêt dès qu'on débranche | Réparé |

## Ma méthode

1. **Reproduire** le symptôme et noter l'état exact (voyants, messages, comportement sur batterie et sur secteur).
2. **Recueillir les données** avant de démonter : BIOS, rapport de batterie, mesures au multimètre.
3. **Éliminer une cause à la fois**, de la plus simple à la plus coûteuse : configuration minimale, CMOS, chargeur, pièces remplaçables, puis carte mère.
4. **Croiser les tests** : une pièce suspecte dans un autre appareil, ou une pièce sûre dans l'appareil en panne.
5. **Documenter** chaque test et son résultat, pour le superviseur et pour le client.

Modèle vierge : [MODELE-FICHE.md](MODELE-FICHE.md)
