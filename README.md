<p align="center">
  <img src="assets/cotcor-banner.png" alt="Bannière CotCor" width="100%">
</p>

<h1 align="center">CotCor</h1>

<p align="center">
  <strong>L’addon complet pour Mage sur WoW 3.3.5a</strong><br>
  Développé pour le serveur Way of Elendil
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Version-5.9.0-f59e0b" alt="Version 5.9.0">
  <img src="https://img.shields.io/badge/WotLK-3.3.5a-7c3aed" alt="WotLK 3.3.5a">
  <img src="https://img.shields.io/badge/Interface-30300-2563eb" alt="Interface 30300">
  <img src="https://img.shields.io/badge/Langue-Français-dc2626" alt="Français">
</p>

---

## Présentation

**CotCor** est un addon développé pour les mages du serveur privé **Way of Elendil**, avec une attention particulière portée à la spécialisation Feu.

Il réunit dans une seule interface claire, légère et personnalisable plusieurs outils habituellement répartis entre différents addons et WeakAuras.

CotCor améliore la visibilité des informations importantes en combat, facilite la coordination entre les mages et permet à chacun d’adapter son interface à sa manière de jouer.

## Fonctionnalités principales

| Module | Description |
| --- | --- |
| **Focalisation de la magie** | Filtrage intelligent des cibles compatibles et suivi des Focalisations du raid. |
| **Chaleur continue / Pyro** | Affichage clair des procs et des critiques en réserve. |
| **Bombe vivante** | Suivi multicible de toutes les Bombes vivantes actives. |
| **Portails et téléportations** | Regroupement des sorts connus avec détection de la faction. |
| **Image miroir** | Visualisation de la durée d’activité et du temps de recharge. |

---

## Focalisation de la magie

CotCor détecte les joueurs du groupe ou du raid ainsi que leur spécialisation. Il les classe automatiquement en trois catégories : **casteurs, soigneurs et corps à corps**.

Seules les classes et spécialisations compatibles avec la Focalisation sont conservées dans la liste. Les autres joueurs n’y apparaissent pas, ce qui offre une meilleure visibilité et permet d’identifier rapidement les cibles les plus intéressantes.

L’addon aide ainsi les mages à mieux répartir et à optimiser leurs **Focalisations de la magie** au sein du raid.

Il permet également de suivre les Focalisations posées par les autres mages, leur cible et leur durée restante grâce à un affichage pouvant regrouper jusqu’à huit mages.

Des messages privés personnalisables facilitent la coordination lorsqu’une Focalisation est posée ou reçue. Un système anti-spam limite automatiquement les messages répétés.

Le suivi reste actif lorsque la cible est hors de portée ou dans une autre instance, puis se réinitialise automatiquement lorsque le joueur quitte son groupe.

---

## Chaleur continue et Pyro

CotCor affiche clairement l’activation de **Chaleur continue** ainsi que les critiques en réserve détectés grâce au journal de combat.

Plusieurs indicateurs visuels sont proposés :

- de grandes flammes pour signaler un proc de Chaleur continue ;
- de petites flammes pour représenter un critique en réserve ;
- des icônes carrées avec un décompte pour un affichage plus classique.

Trois modes permettent d’afficher les flammes, les icônes ou les deux simultanément. La taille des éléments visuels est personnalisable.

Le proc de Pyro et le critique en réserve fonctionnent indépendamment. La réserve peut également être conservée après la fin du combat.

---

## Bombe vivante

Le module **Bombe vivante** suit simultanément toutes les Bombes actives sur les différentes cibles.

Chaque cible dispose de sa propre barre avec son nom complet et le temps restant avant l’explosion. Jusqu’à **12 Bombes vivantes** peuvent être affichées en même temps.

La largeur, la hauteur, l’espacement et le nombre maximal de barres sont entièrement personnalisables.

---

## Portails et téléportations

CotCor regroupe les portails de groupe et les téléportations personnelles dans deux interfaces distinctes.

L’addon analyse automatiquement le grimoire et ne conserve que les sorts réellement connus par le personnage. Il détecte également la faction afin de proposer uniquement les destinations correspondantes, avec les noms des villes en français.

Les temps de recharge sont affichés directement sur les icônes. CotCor peut aussi annoncer l’ouverture d’un portail dans le raid et détecter ceux lancés par les autres mages.

Les éléments du module peuvent être positionnés librement dans l’interface.

---

## Image miroir

Le module **Image miroir** permet de distinguer immédiatement les deux états du sort :

- un affichage vert pendant les 30 secondes d’activité des images ;
- un affichage rouge et grisé pendant les 150 secondes de recharge.

Un décompte numérique indique précisément le temps restant dans chaque état.

---

## Interface et personnalisation

CotCor possède une interface centralisée organisée en sept catégories :

- Options ;
- Focus Magic ;
- Pyro ;
- Bombe vivante ;
- Portails ;
- Image miroir ;
- Profils.

Le menu est redimensionnable et son contenu s’adapte automatiquement à la largeur disponible. Les différents modules peuvent être déplacés et configurés séparément.

Le système de profils permet de sauvegarder plusieurs configurations, de les charger rapidement ou de revenir aux paramètres par défaut.

Tous les textes sont centralisés dans `Localization.fr.lua`. Ils peuvent être modifiés sans toucher au code principal et les personnalisations sont préservées lors des mises à jour.

---

## Performances

CotCor est optimisé pour conserver un impact minimal sur les performances, y compris en raid 25 :

- limitation intelligente des événements fréquents ;
- réutilisation des tables afin de réduire le garbage collector ;
- filtrage immédiat de la majorité des événements du journal de combat ;
- réduction des accès inutiles aux fonctions globales de WoW.

---

## Informations techniques

| Élément | Détail |
| --- | --- |
| **Version** | 5.9.0 |
| **Compatibilité** | WoW 3.3.5a |
| **Interface** | 30300 |
| **Serveur** | Way of Elendil |
| **Langue** | Français |
| **Encodage** | UTF-8 sans BOM |
| **Sauvegarde** | `CotCorDB`, par compte |
| **Communication** | Préfixe `COTC` en P2P |
| **Librairies** | LibGroupTalents, LibStub, CallbackHandler et ChatThrottleLib |

---

<p align="center">
  <img src="assets/cotcor-logo.png" alt="Logo CotCor" width="180">
</p>

<p align="center">
  <strong>Toutes les informations essentielles du mage réunies dans un seul addon.</strong>
</p>

<p align="center">
  Développé par <strong>Anrel / CotteCotte</strong>
</p>
