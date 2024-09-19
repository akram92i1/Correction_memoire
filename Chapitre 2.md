1- Introduction
_______
==Plusieurs travaux se concentrent sur l'optimisation de la trajectoire des UAVs pour maximiser l'efficacité de la collecte de données. Des contraintes telles que la consommation d'énergie du drone, les restrictions de communication et de vitesse, ainsi que la couverture de communication sont prises en compte. \cite{8486942} modélise la consommation d'énergie des UAVs et permet d'optimiser leur énergie lors des missions, tandis que \cite{6863654} propose une formule pour prédire la probabilité de liaison en visibilité directe entre l'UAV et le récepteur, ce qui aide à optimiser la zone de couverture du signal radio. Ces travaux visent à concevoir des stratégies de planification de trajectoire écoénergétiques et efficaces pour les UAVs, tenant compte des exigences spécifiques de communication et de performance.==



==La conception de la trajectoire est cruciale dans les réseaux de capteurs IoT activés par UAV. Afin de garantir une transmission et une réception fiables des données, le drone doit voler à proximité suffisante des capteurs IoT tout en respectant les limites de distance maximale et ce pour assurer une plus grande couverture des capteurs dans l'optique de maximiser les performances globales du système. L'intérêt pour la conception de trajectoires a considérablement augmenté au cours des dernières années. Dans \cite{9054054}, les auteurs conçoivent une trajectoire tridimensionnelle d'un UAV pour une collecte efficace des données en maximisant l'efficacité du drone sous un ensemble de contraintes, sans considérer les obstacles lors des déplacements en perspective 3D. \cite{8933037} étudient le rôle des UAVs dans la gestion des ressources du réseau de capteurs en maximisant l'énergie résiduelle minimale des capteurs après la transmission des données tout en minimisant les mouvements du drone. Enfin, \cite{8663615} étudient la minimisation du temps de mission et de l'énergie sur un drone déployé dans des environnements IoTs tout en maintenant des restrictions de communication. Notamment, leur solution ignore les instances impliquant un grand nombre de capteurs, un élément important que notre étude aborde expressément. Notre stratégie, qui se base sur une fonction pondérée des objectifs à minimiser, fournit une alternative plus évolutive pour faire face aux déploiements de systèmes de plus en plus massifs.==


Récemment, l'intérêt pour la conception de trajectoires a considérablement augmenté.



Notre projet de recherche se concentre sur la planification d'une trajectoire écoénergétique et consciente du temps de vol de l'UAV tout en tenant compte de restrictions de communication et de vitesse. Nous présentons une stratégie heuristique efficace pour optimiser le placement des capteurs planifiés. Notre recherche s'appuie sur le modèle de consommation de temps et d'énergie des UAVs provenant de \cite{8663615} et développe notre approche de planification de mission pour le drone.


Notre projet de recherche se concentre sur la planification d'une trajectoire écoénergétique et consciente du temps de vol de l'UAV tout en tenant compte de restrictions de communication et de vitesse. Dans ce travail, j'ai proposé une modélisation introduisant une approche novatrice pour l'optimisation de la trajectoire des drones. Cette modélisation constitue une base solide dans ce domaine et se révèle facilement scalable, permettant ainsi d'intégrer de nouvelles contraintes à optimiser dans des travaux futurs. Nous présentons une stratégie heuristique efficace pour optimiser le placement des capteurs planifiés. Notre recherche s'appuie sur le modèle de consommation de temps et d'énergie des UAVs provenant de \cite{8663615} et développe notre approche de planification de mission pour le drone.

______
