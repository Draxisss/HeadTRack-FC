# Éco'Light 🌞

*Projet pour automatiser l'éclairage solaire avec ESP32-C3.*

--

## Overview

**Éco'Light** est un projet qui automatise l’allumage et l’extinction des LED selon la luminosité ambiante.  
Pourquoi ce projet : pour économiser de l’énergie et expérimenter l’intégration électronique et mécanique.  
Comment l’utiliser : branchez le module, chargez le firmware via USB, et observez les LED s’allumer ou s’éteindre automatiquement.

---

## Full 3D Model

![Vue 3D complète](images/full_assembly.png)

> Montre l’assemblage complet, incluant l’électronique et le boîtier.

---

## PCB

![PCB](images/pcb.png)

> Capture de l’empreinte PCB et de tous les composants soudés.

---

## Wiring Diagram

![Schéma câblage](wiring/wiring_diagram.png)

> Schéma pour les câbles qui ne passent pas par la PCB.

---

## CAD Files

- Fichier natif : `/cad/ecolight.FCStd`  
- Export STEP complet : `/cad/ecolight.step`

> ⚠️ Le fichier STEP doit inclure toutes les pièces et l’électronique.

---

## PCB Files

Tous les fichiers PCB sont dans `/pcb/` :  

- `ecolight.kicad_pro`  
- `ecolight.kicad_sch`  
- `ecolight.kicad_pcb`  
- `gerbers.zip`

---

## Firmware

Le code source est dans `/firmware/` :  

- `main.cpp`  
- Bibliothèques nécessaires  
- Configurations et fichiers de calibration

---

## Bill of Materials

| Item | Quantity | Price | Link |
|------|----------|-------|------|
| ESP32-C3 | 1 | $5.20 | [Lien](https://...) |
| LED 5mm | 5 | $0.50 | [Lien](https://...) |
| Résistance 220Ω | 5 | $0.10 | [Lien](https://...) |
| LiPo 1000mAh | 1 | $8.00 | [Lien](https://...) |

> ⚠️ Pense à ajouter le fichier `BOM.csv` à la racine avec les mêmes éléments.

---

## Folder Structure

```text
/ (root)
│── README.md
│── BOM.csv
│── firmware/
│    └── main.cpp
│── pcb/
│    ├── ecolight.kicad_pro
│    ├── ecolight.kicad_sch
│    ├── ecolight.kicad_pcb
│    └── gerbers.zip
│── cad/
│    ├── ecolight.FCStd
│    └── ecolight.step
│── wiring/
│    └── wiring_diagram.png
│── images/
     ├── full_assembly.png
     └── pcb.png
