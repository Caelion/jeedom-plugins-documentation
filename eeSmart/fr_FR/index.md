---
layout: default
title: Documentation eeSmart
lang: fr_FR
pluginId: eeSmart
---

<div id="title">
<a href="../../../{{site.baseurl}}/{{page.pluginId}}/{{page.lang}}">Plugin {{page.pluginId}}</a>
</div>

Présentation
===

Plugin développé en partenariat avec la société eeSmart qui distribue les produits D2L.
Leur produit est un module ERL à brancher sur le compteur Linky. Ce module envoi de manière régulière sur un serveur donné (pour le moment : d2l.sicame.io) les données du compteur Linky.

Ce plugin permet, via l’API qu’eeSmart met à disposition, de récupérer les données présentes sur le site d2l.sicame.io afin de les suivre dans Jeedom.

Note : le site d2l.sicame.io remplace dorénavant l'ancien site consospyapi.sicame.io

Note 2 : Manuel du module D2L : http://eesmart.fr/wp-content/uploads/eeSmart-D2L-Notice-dinstallation.pdf

Configuration
===
Une fois le plugin installé, vous devez :
- Aller dans la page "Configuration" du plugin et renseigner votre identifiant et votre mot de passe eeSmart
- Sauvegarder
- Cliquer sur le bouton "Connexion"
Si les informations saisies sont correctes, un message vous invitant à rafraîchir la page apparaît.

Vous pouvez ensuite ajouter un équipement dans le menu habituel.
Votre seule action sera alors de sélectionner le module correspondant à celui que vous voulez analyser.
Vous pouvez mettre vos différents modules si vous en avez plusieurs.

L'équipement alors créé se mettra en forme au premier rafraichissement (cron de 5 minutes) pour n'afficher que les index correspondants à ceux liés au contrat.

Fonctionnement
===
- Un cron quotidien est  présent pour rafraîchir la clé API
- Un cron à 5 minutes est utilisé pour mettre à jour les informations du compteur.

Info
===
La puissance affichée est déterminée par calcul sur la base d'un courant à 230 Volts :
Puissance théorique : Intensité * 230V (P=UI)

Changelog
===
[Lien vers le changelog]({{site.baseurl}}/{{page.pluginId}}/{{page.lang}}/changelog)
