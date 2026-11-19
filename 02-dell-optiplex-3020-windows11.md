# Fiche 02 : Dell OptiPlex 3020, remise en service et Windows 11

<img src="https://img.shields.io/badge/Remis%20en%20service-2E8B57?style=flat-square" alt="Remis en service">

**Date :** octobre 2026 · **Appareil :** Dell OptiPlex 3020 (PC de bureau) · **Résultat :** Remis en service, devenu poste de travail de la boutique

## Symptôme

PC reçu sans mémoire ni disque. Une fois équipé, il redémarre en boucle. Ensuite, la clé USB d'installation est détectée au menu F12 mais un mot de passe BIOS inconnu bloque le démarrage.

## Tests effectués

1. Installation de la RAM et du disque : redémarrages en boucle, puis arrivée au bureau Windows
2. Démarrage depuis une clé USB amorçable vers un SSD seul : bloqué par le mot de passe BIOS
3. Recherche du cavalier PSWD sur la carte mère (connecteur à 3 broches)

## Cause

Mot de passe BIOS laissé par l'ancien propriétaire. Ensuite, matériel non compatible TPM 2.0, exigé par l'installateur de Windows 11.

## Solution

1. Mot de passe effacé avec le cavalier PSWD
2. Vérification TPM contournée dans l'Éditeur du Registre de l'installateur (Maj+F10, regedit)
3. Windows 11 installé sur le SSD et configuré avec un compte local

## Ce que j'en retiens

Sur un vieux poste d'entreprise, vérifier d'abord le mot de passe BIOS et la compatibilité TPM avant de préparer l'installation. Le contournement TPM est acceptable pour un poste interne, pas pour un parc géré où la sécurité compte.

---

[← Retour au journal](README.md)
