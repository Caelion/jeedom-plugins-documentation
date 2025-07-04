---
layout: default
title: Changelog Programmateur
lang: fr_FR
pluginId: Programmateur
---

<div id="title">
<a href="../../../{{site.baseurl}}/{{page.pluginId}}/{{page.lang}}">Plugin {{page.pluginId}}</a>
</div>

Changelog Stable
===
- Création du plugin
- Ajout de la documentation / changelog au format Jeedom
- 25/03/2020 : Refonte du système de cron du plugin
- 10/04/2020 : Modification d'informations en mode DEBUG
- 13/04/2020 : Relocalisation de la documentation du plugin
- 26/04/2020 : Correction d'une erreur sur les crons en cas d'existence de plusieurs programmateurs
- 03/05/2020 (Beta 24/04/2020) : /!\ Refonte du moteur de calcul du plugin : vous devrez refaire le paramétrage des équipements (les commandes ne changent pas donc les éventuels liens avec d'autres équipements restent opérationnels)
  - Ajout comptabilité avec les scénarios pour les actions 1 et 2
  - Ajout possibilité d'une durée négative
  - Ajout possibilité action non répétée
  - Ajout comptabilité avec une variable pour l'information sur les jours fériés
  - Modification du widget durée pour ajouter des boutons pour les modifications importantes (par tranche de 60min)
- 02/06/2020 : Correction d'un bug sur la désactivation / activation inopinée de l'information lundi (**ne corrige que les nouveaux équipements** : une correction manuelle sur les équipements déjà existants peut se faire en procédant ainsi : supprimer l'information lundi puis de sauvegarder 2 fois l'équipement pour la recréer correctement).
- 03/06/2020 : Correction de la liaison avec les widgets du plugin (**ne corrige que sur les nouveaux équipements** : une correction manuelle sur les équipements déjà existants peut se faire en procédant ainsi : sélectionner manuellement les widget du plugin pour les commandes Toggle/Day/Time/Delay). Avant cette correction, si vous allez dans Affichage de la commande, "Defaut" apparait alors que la commande utilise tout de même l'un des widgets du plugin (Toggle/Day/Time/Delay).
- 21/11/2020 :
  - Nouvelle présentation de la liste des objets
  - Ajout du tag "Compatibilité V4"
  - Ajout d'une fonction Marche forcée pour la durée spécifiée.
     - En cas de durée négative : durée en valeur positive et inversion des actions 1 et 2
     - Le programmateur n'a pas besoin d'être sur On pour que la marche forcée fonctionne. Par contre, l'équipement doit être actif.
- 22/12/2020 :
  - Refonte des widget Mobile : Toggle Jour / Heure / Durée
  - Refonte des widget Dashboard : Toggle Jour / Heure
  - Ajout d'une option d'exécution d'action de fin sur mise sur off du programmateur concerné
- 28/08/2021 :
  - Ajout d'un paramètre "tag" lorsque l'action est un scénario (merci @Henribi pour le développement)
- 31/05/2024 :
  - Modification widget :
    - Toggle > Core
    - Delay & Time : mise à jour suite évolution du core
  - Ajout vue tableau dans la page "mes programmateurs"
  - Suppression branche V3

Note : pour vos équipements actuels, vous pouvez appliquer le même correctif en faisant :

Edition du widget des commandes on et off en desktop et mobile : choisir core>binaryswitch et cocher "retour à la ligne après".
- 03/10/2024 :
  - Correction non static function (merci Henribi/Fabrice)
- 14/06/2025 :
  - Optimisation du code :
    - Factorisation des jours
    - Tests de l'existence des cmd
    - Tests de l'existence des scenarios
    - Tests de l'existence des eqLogic
  - Correction du Widget Time : gestion des minutes sur les heures < 10h lors du passage de 59 à 0 ou vice versa
  - Correction sur fonction dépréciée en 4.5 (jeedom.eqLogic.buildSelectCmd à la place de jeedom.eqLogic.builSelectCmd)

Changelog Beta
===
(passage en stable 7 jours après le dernier message sur le community ou sur le repo)

- 14/06/2025 :
  - 
