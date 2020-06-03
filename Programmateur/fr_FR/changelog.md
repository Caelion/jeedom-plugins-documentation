---
layout: default
title: Changelog Programmateur
lang: fr_FR
pluginId: Programmateur
---

<div id="title">
<a href="../../../{{site.baseurl}}/{{page.pluginId}}/{{page.lang}}">Plugin {{page.pluginId}}</a>
</div>

Changelog
===
- Création du plugin
- Ajout de la documentation / changelog au format Jeedom
- 25/03/2020 : Refonte du système de cron du plugin
- 10/04/2020 : Modification d'informations en mode DEBUG
- 13/04/2020 : Relocalisation de la documentation du plugin
- 26/04/2020 : Correction d'une erreur sur les crons en cas d'existence de plusieurs programmateurs
- 03/05/2020 (Beta 24/04/2020) : /!\ Refonte du moteur de calcul du plugin : vous devrez refaire le paramètre de l'équipement (les commandes ne changent pas donc les éventuelles liens avec d'autres équipements restent opérationnels)
  - Ajout comptabilité avec les scénarios pour les actions 1 et 2
  - Ajout possibilité d'une durée négative
  - Ajout possibilité action non répétée
  - Ajout comptabilité avec une variable pour l'information sur les jours fériés
  - Modification du widget durée pour ajouter des boutons pour les modifications importantes (par tranche de 60min)
- 02/06/2020 : Correction d'un bug sur la désactivation / activation inopinée de l'information lundi (ne corrige que les nouveaux équipements. Une correction manuelle peut être de supprimer l'information lundi puis de sauvegarder 2 fois l'équipement).
- 03/06/2020 : Correction de la liaison avec les widgets du plugin (ne corrige que sur les nouveaux équipements). Avant cette correction, si vous allez dans Affichage de la commande, "Defaut" apparait alors que la commande peut tout de même utiliser l'un des widgets du plugin (Toggle/Day/Time/Delay).

## BETA
- Néant
