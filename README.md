<p align="center"><img src="assets/banniere.svg" alt="Journal de dépannage — symptôme, tests, cause, solution" width="100%"></p>

# Journal de dépannage

Fiches d'intervention tirées de mon stage de technicien informatique chez LaboPhone Inc., atelier de réparation (octobre – novembre 2026), dans le cadre du DEP Soutien informatique (ESIDEM, Montréal).

Chaque fiche suit le même ordre : **symptôme → tests → cause → solution → ce que j'en retiens**. Les informations des clients ne sont pas publiées.

<p>
  <img src="https://img.shields.io/badge/fiches-7-informational?style=flat-square" alt="7 fiches">
  <img src="https://img.shields.io/badge/r%C3%A9par%C3%A9s-3-2E8B57?style=flat-square" alt="3 réparés">
  <img src="https://img.shields.io/badge/en%20cours-4-F28C28?style=flat-square" alt="4 en cours">
  <img src="https://img.shields.io/badge/outils-multim%C3%A8tre%20%C2%B7%20BIOS%20%C2%B7%20powercfg-555?style=flat-square" alt="Outils">
</p>

📅 **[Déroulement du stage, semaine par semaine](stage.md)** : l'atelier en photos, toutes mes interventions et les compétences mises en pratique.

| Fiche | Appareil | Problème | Résultat |
| --- | --- | --- | --- |
| [01](01-acer-nitro5-ne-demarre-pas.md) | Acer Nitro 5 AN515-55 | Ne démarre pas, ventilateurs muets | <img src="https://img.shields.io/badge/R%C3%A9par%C3%A9-2E8B57?style=flat-square" alt="Réparé"> |
| [02](02-dell-optiplex-3020-windows11.md) | Dell OptiPlex 3020 | Mot de passe BIOS inconnu, installation de Windows 11 bloquée | <img src="https://img.shields.io/badge/Remis%20en%20service-2E8B57?style=flat-square" alt="Remis en service"> |
| [03](03-asus-cpu-fan-error.md) | PC Asus, carte P8H61-M PRO | Message « CPU FAN ERROR » | <img src="https://img.shields.io/badge/En%20cours-F28C28?style=flat-square" alt="En cours"> |
| [04](04-portable-aucun-signe-de-vie.md) | Portable à deux SSD | Aucun voyant malgré 19 à 20 V au connecteur | <img src="https://img.shields.io/badge/En%20cours-F28C28?style=flat-square" alt="En cours"> |
| [05](05-surface-pro-7-batterie.md) | Microsoft Surface Pro 7 | Batterie non détectée, arrêt dès qu'on débranche | <img src="https://img.shields.io/badge/R%C3%A9par%C3%A9-2E8B57?style=flat-square" alt="Réparé"> |
| [06](06-hp-pavilion-p7-1042-sans-affichage.md) | HP Pavilion p7-1042 (tour) | S'allume sans affichage | <img src="https://img.shields.io/badge/En%20cours-F28C28?style=flat-square" alt="En cours"> |
| [07](07-hp-ventilateur-ne-tourne-pas.md) | Portable HP, carte DA0PAHMB8F0 | Voyants allumés, ventilateur immobile | <img src="https://img.shields.io/badge/En%20cours-F28C28?style=flat-square" alt="En cours"> |

## Ma méthode

```mermaid
flowchart LR
    A["🔎 Reproduire<br/>le symptôme"] --> B["📋 Recueillir<br/>les données<br/>BIOS · rapport · multimètre"]
    B --> C["🧪 Éliminer<br/>une cause à la fois<br/>du moins coûteux<br/>au plus coûteux"]
    C --> D{"Cause<br/>trouvée ?"}
    D -- "non" --> E["🔁 Croiser les tests<br/>pièce suspecte ailleurs<br/>pièce sûre ici"]
    E --> C
    D -- "oui" --> F["🔧 Réparer"]
    F --> G["📝 Documenter<br/>pour le superviseur<br/>et le client"]
    classDef ok fill:#E5F4E4,stroke:#2E8B57,color:#1B4D2E
    class F,G ok
```

Modèle vierge : [MODELE-FICHE.md](MODELE-FICHE.md)
