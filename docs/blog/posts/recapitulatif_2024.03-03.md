---
draft: false
authors:
  - partiexplorer
date: 2024-03-03
comments: true
tags:
    - Canada
    - Québec
---

# Récapitulatif - 2024-03-03

Récapitulatif des tâches accomplies par catégorie

## Camion

Pendant mon périple à la Baie-James, mon indicateur de carburant a cessé de fonctionner. À un moment donné, il est descendu en deux secondes et n'est jamais remonté. Pour éviter de tomber en panne, je me suis fié au nombre de kilomètres parcourus. J'ai commencé les travaux de réparation il y a quelques semaines et j'en étais arrivé à la conclusion que le problème était mon capteur de carburant, situé à l'intérieur du réservoir. J'ai reçu la pièce de rechange et ce matin, j'allais vérifier si elle fonctionnait avant de retirer le réservoir. Cependant, lors de mes tests, j'ai réalisé que ma compréhension du fonctionnement du capteur était erronée. Contrairement à ce que je pensais, le capteur était en bon état. Le problème était <!-- more -->en fait la mise à la terre du capteur. Je n'avais jamais connecté le boulon central du capteur à la masse, car connecter simplement les deux câbles semblait tout faire fonctionner. Je suppose que la boue et les vibrations ont dû rendre la mise à la terre avec la carrosserie du capteur moins efficace, voire inexistante. Lorsque j'ai connecté une nouvelle mise à la terre au boulon central, mon indicateur de carburant a affiché le bon niveau. Hourra ! Je n'ai pas besoin d'ouvrir le réservoir.

- Enfin un Fuel Gauge qui fonctionne... Houra !!
- Câblage des switchs qui indiquent l'état des portes avant
- Remplacement des stopper en caoutchouc pour remettre mon pneu de secours sur le capot
- Installation d'un Exhaust Gas Temperature (EGT) pour avoir un meilleur feedback de la mécanique.
- Déplacement des Front Position Light au dessous du rack au lieu du dessus.

## Électronique

### Pico-GPS

![Pico-GPS](/assets/images/blog/pico-gps-design1.jpg){ width=120 }
![Pico-GPS-Fritzing](/assets/images/blog/pico-gps-design1-fritzing.png){ width=120 }

Design de l'emplacement des composantes du Pico-GPS sur le BreadBoard. Les composantes électroniques sont :

* un microcontrôleur Raspberry Pi Pico W
* un module GPS
* un module BME280
* un écran LCD

Pour finaliser le design il ne manque que le module de carte microSD. Je me suis servi de ce design pour approfondir mes connaissances avec le logiciel [Fritzing](https://fritzing.org).

### Optocoupler

Validation de l'Optocoupler Board NPN (12v-->3.3v) avec prototype pico avec `led` pour afficher l'état du capteur `on/off`

![Optocoupler-Pico](/assets/images/blog/optocoupler-pico.jpg){ width=120 }

## Site web / Blog - Ajout de plugins
* `giscus` pour permettre l'ajout de commentaires et de likes
* `leaflet` et `leaflet-gpx` pour afficher les tracés et les points d'intérêt
* `leaflet-fullscreen` pour ajouter le mode plein écran et l'échelle

## Divers

* Commande de matériels électroniques. C'est toujours très long à faire à cause des "tant qu'à..."
* Journée administrative: papperasse, budget, etc
