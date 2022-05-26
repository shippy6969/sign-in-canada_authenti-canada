---
layout: default
ref: maintenance
title: Entretien prévu à venir
lang: fr
---
# Entretien prévu à venir

## Vendredi 27 mai 2022 7h00 HAE

### Environnements concernés :

* Test d'acceptation client

### La description

L'équipe d'Authenti-Canada sera de mise à jour les clés cryptographiques
utilisées pour s'authentifier aux environnements de test GCKEY et CBS entre 7 h
et 8 h, heure de l'Est le vendredi 27 mai.

Afin de maintenir l'intégration entre le Authenti-Canada Environnement test
 d'acceptation du client (CATE) et les deux services d'identification SSC, 2
Keys et SecureKey aura besoin de configurer ces nouvelles clés
simultanément.Celles-ci Les changements sont étroitement coordonnés entre TBS,
SSC et les deux fournisseurs afin Pour minimiser les temps d'arrêt, mais les
clients peuvent rencontrer brièvement des erreurs un changement est en cours.

La portée de ce changement est limitée au L'environnement de test d'acceptation client.
L'environnement de production ne sera pas affecté.

## Vendredi 27 mai 2022 21h00 HAE

### Environnements concernés :

* Test d'acceptation client

### La description

L'équipe d'Authenti-Canada déploiera une nouvelle version de la plate-forme du Authenti-Canada
[Version 1.2.98](https://github.com/sign-in-canada/Acceptance-Platform/releases/tag/v1.2.98)
à l'environnement de test d'acceptation du client.L'installation est prévue pour 21h
et devrait entraîner une panne d'environ 35 minutes.

## Dimanche 29 mai 2022 à 4 h 00 HAE

### Environnements concernés :

* Production

### La description

Les derniers correctifs de sécurité Linux seront appliqués à l'environnement de production
À partir de 4h du matin.Cela entraînera une panne d'environ 12 minutes.