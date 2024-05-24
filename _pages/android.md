---
permalink: /android/
title: "Développement d'applications Android natives"
---

Je vous propose de vous accompagner dans le développement de vos applications Android natives en Kotlin.

Cela fait maintenant 10 ans que je développe des applications mobiles. En 10 ans, j'ai eu le temps de travailler :
- dans **différents domaines d'application** : IoT, mobilité, cinéma, spectacle, réseaux sociaux, stockage de fichiers, lecteurs multimédia, sécurité ..., 
- pour des applications aussi bien **métier**, que destinées au **grand public** (> 100k et > 1M utilisateurs pour certaines), 
- avec **différents composants** : WiFi, BLE - Bluetooth Low Energy, Géolocalisation, Caméra, cartographie ..., 
- avec **différentes architectures logicielles** : MVC, MVP, MVI, MVVM, Clean
- et j'ai vu évoluer les environnements/langages (plus anciennement *Java*, *Views* en *XML*, *Dagger*... et plus modernes comme Kotlin, et les composants cités juste après).

Cette expérience me permet aujourd'hui d'avoir un certain recul sur mon travail, une vision d'ensemble et une boîte à outils adaptée aux différentes problématiques de l'environnement Android.

## Développement moderne

Aujourd'hui, je travaille essentiellement avec des composants modernes, dont voici les principaux :
- *Jetpack Compose* pour la partie vue
- *ViewModel*, *UseCases*, *Repositories* ...
- *Room* pour la gestion de bases de données locales
- *Retrofit* et *Ktor* pour les échanges sur le réseau
- *WorkManager* pour la planification de tâches
- *Koin* et *Hilt* pour l'injection de dépendances

## Qualité de code

Je porte une importance particulière à la qualité du code, sa lisibilité et sa maintenance. Pour cela, j'utilise des architectures *MVVM* / *Clean* avec une inversion des dépendances et une attention au principe de responsabilité unique des classes afin de rendre le code le plus facilement testable et maintenable.

Une importance est aussi donnée à la partie validation avec une bonne maîtrise de gestion des tests unitaires, d'intégration et des tests UI. Leur mise en place est grandement facilitée par la qualité de l'architecture et le respect des principes du "*clean code*" / "*software craftsmanship*".

## Mutualisation iOS / Android

Afin de mutualiser au maximum le travail réalisé sur la couche métier et d'améliorer la cohésion de l'équipe mobile (iOS + Android), je mets en place, lorsque cela est possible, une partie de code partagée et développée en [*Kotlin Multiplatform* (KMP / KMM)](/kmp). Cette partie regroupe le plus généralement la couche métier avec les différents cas d'utilisation métier réalisés par l'application, et la couche données.

J'expérimente en ce moment l'utilisation de ViewModel partagés, ainsi que l'utilisation de Compose Multiplatform afin de faciliter le développement de MVP / PoC.

## Expérience / projets

Voici les principaux projets de développement Android sur lesquels j'ai eu l'occasion de travailler ces dernières années :

- **Oodrive** (Depuis 2021) : développement de nouvelles fonctionnalités et maintenances d'applications servant au stockage de fichiers en ligne et à la synchronisation automatique de la galerie de fichiers multimédias. Composants utilisés : architecture *MVVM/Clean*, *WorkManager*, *Kotlin Coroutines*, *Kotlin Flows*, *Hilt*, *Room*, *Baseline profiles*, *MacroBenchmarks*.
- **KerMap** (2024) : conception et développement d'une application Open Source (prochainement publiée) grand public afin de faire découvrir le patrimoine historique local d'une commune. Composants utilisés : *MVVM/Clean* architecture, *Jetpack Compose*, *Room*, *Ktor*, *Koin*, *Kotlin Coroutines*, *Kotlin Flow*, *Baseline profiles*, *MacroBenchmarks*, migration en cours vers *KMP*
- **Famileo** (2022 - 2023) : développement de nouvelles fonctionnalités sur une application de réseau social grand public à large audience (1 M+ de téléchargements, note de 4,8/5 avec ~40k avis sur le Play Store). Composants utilisés : *MVVM*, *Jetpack Compose*, *Ktor*, *Koin*, *Kotlin Coroutines*, *KMP*.
- **Velco** (2017 - 2020) : Lead tech développement applications mobiles pour de l'IoT. Développement d'applications Android grand public pour une aide à la navigation à vélo via un guidon connecté en Bluetooth Low Energy. Composants utilisés : *Bluetooth Low Energy*, GPS, cartographie *OpenStreetMap* & navigation avec *MapBox*, développement de librairies *C++*, *KMP*. 
- **Exalux** (2015 - 2017) : développement d'applications Android et iOS pour le contrôle d'éclairages connecté en *Bluetooth* classique, en *Bluetooth Low Energy* et en *Wi-Fi* (*UDP*).

Vous trouverez davantage de projets sur [mon profil LinkedIn](https://www.linkedin.com/in/antoine-jaury/).