1- Introduction

L'utilisation de véhicules aériens sans pilote (UAV) en tant que plateforme de communication sans fil volantes a  suscité beaucoup d'attention \cite{8663615}. les UAVs, équipés de transmetteurs de communication qui sont des dispositifs électroniques a des fins d'envoi de signaux ou de données, sont de plus en plus utilisés pour la diffusion d'informations, le relais, la collecte de données, la surveillance, etc. \cite{zeng2016wireless}. Cela est principalement dû au déploiement flexible et à la grande mobilité des UAVs, ainsi qu'à leurs liaisons de communication en visibilité direct (en anglais: Line-of-sight) avec les terminaux au sol, par opposition aux communications terrestres conventionnelles ou aux communications de véhicules terrestres sans pilote (UGV) \cite{wang2017wirelessly}.Ces avantages ont conduit à l'adoption des UAVs autant que collecteurs de données sur des systèmes (IoT) composés de capteur\cite{ghorbel2019joint}, où un UAV visite chaque capteur IoT ou tête de cluster pour collecter des données avant de les livrer à une station de contrôle. En fonction de l'utilisation complète ou non de la mobilité de l'UAV, il existe principalement deux types de communications UAV-vers-le-sol (U2G)/Sol-vers-UAV (G2U) dans la littérature \cite{9054054}. Afin de garantir une couverture de communication aussi large que possible, plusieurs études se concentre principalement sur l'optimisation du placement et du déploiement de l'UAV statiques ou quasi statiques. L'autre axe de recherche vise à exploiter pleinement la grande mobilité des UAVs via la conception et l'optimisation de leur trajectoire \cite{8933037}, ce qui apporte un nouveau degré de liberté dans l'optimisation des performances des systèmes de communication sans fil.

L'utilisation de véhicules aériens sans pilote (UAV) en tant que plateforme de communication sans fil volantes a suscité beaucoup d'attention \cite{8663615}. Les UAVs, équipés de transmetteurs de communication qui sont des dispositifs électroniques destinés à l'envoi de signaux ou de données, sont de plus en plus utilisés pour la diffusion d'informations, le relais, la collecte de données, la surveillance, etc. \cite{zeng2016wireless}. Cela est principalement dû au déploiement flexible et à la grande mobilité des UAVs, ainsi qu'à leurs liaisons de communication en visibilité directe (en anglais : Line-of-sight) avec les terminaux au sol, par opposition aux communications terrestres conventionnelles ou aux communications de véhicules terrestres sans pilote (UGV) \cite{wang2017wirelessly}. Ces avantages ont conduit à l'adoption des UAVs en tant que collecteurs de données dans des systèmes IoT composés de capteurs \cite{ghorbel2019joint}, où un UAV visite chaque capteur IoT ou tête de cluster pour collecter des données avant de les livrer à une station de contrôle. En fonction de l'utilisation complète ou non de la mobilité de l'UAV, il existe principalement deux types de communications UAV-vers-le-sol (U2G)/Sol-vers-UAV (G2U) dans la littérature \cite{9054054}. Afin de garantir une couverture de communication aussi large que possible, plusieurs études se concentrent principalement sur l'optimisation du placement et du déploiement des UAV statiques ou quasi statiques. L'autre axe de recherche vise à exploiter pleinement la grande mobilité des UAVs via la conception et l'optimisation de leur trajectoire \cite{8933037}, ce qui apporte un nouveau degré de liberté dans l'optimisation des performances des systèmes de communication sans fil.



_______
==Plusieurs travaux se concentrent sur l'optimisation de la trajectoire des UAVs pour maximiser l'efficacité de la collecte de données. Des contraintes telles que la consommation d'énergie du drone, les restrictions de communication et de vitesse, ainsi que la couverture de communication sont prises en compte. \cite{8486942} modélise la consommation d'énergie des UAVs et permet d'optimiser leur énergie lors des missions, tandis que \cite{6863654} propose une formule pour prédire la probabilité de liaison en visibilité directe entre l'UAV et le récepteur, ce qui aide à optimiser la zone de couverture du signal radio. Ces travaux visent à concevoir des stratégies de planification de trajectoire écoénergétiques et efficaces pour les UAVs, tenant compte des exigences spécifiques de communication et de performance.==






==La conception de la trajectoire est cruciale dans les réseaux de capteurs IoT activés par UAV. Afin de garantir une transmission et une réception fiables des données, le drone doit voler à proximité suffisante des capteurs IoT tout en respectant les limites de distance maximale et ce pour assurer une plus grande couverture des capteurs dans l'optique de maximiser les performances globales du système. L'intérêt pour la conception de trajectoires a considérablement augmenté au cours des dernières années. Dans \cite{9054054}, les auteurs conçoivent une trajectoire tridimensionnelle d'un UAV pour une collecte efficace des données en maximisant l'efficacité du drone sous un ensemble de contraintes, sans considérer les obstacles lors des déplacements en perspective 3D. \cite{8933037} étudient le rôle des UAVs dans la gestion des ressources du réseau de capteurs en maximisant l'énergie résiduelle minimale des capteurs après la transmission des données tout en minimisant les mouvements du drone. Enfin, \cite{8663615} étudient la minimisation du temps de mission et de l'énergie sur un drone déployé dans des environnements IoTs tout en maintenant des restrictions de communication. Notamment, leur solution ignore les instances impliquant un grand nombre de capteurs, un élément important que notre étude aborde expressément. Notre stratégie, qui se base sur une fonction pondérée des objectifs à minimiser, fournit une alternative plus évolutive pour faire face aux déploiements de systèmes de plus en plus massifs.==

Ce qui reste a faire dans le chapitre 02 selon  **claude** 
-> Annoncez la structure du chapitre ? est ce que c'est obligatoire ? **regarde ce que a fait meriem**
-> Revoir l’introduction du chapitre 02
-> Ajoutez une brève introduction au début de chaque section principale, expliquant les caractéristiques générales de ces approches.
-> Ajoutez une brève introduction au début de chaque section principale, expliquant les caractéristiques générales de ces approches. 
	-c) À la fin de chaque sous-section, ajoutez un paragraphe de synthèse qui compare les approches présentées, leurs avantages et leurs limites.
-> Améliorations supplémentaires : 
	-a) Au début du chapitre, ajoutez un paragraphe expliquant la structure que vous avez choisie et pourquoi. 
	-b) À la fin de chaque section principale, ajoutez une synthèse plus large qui compare les approches exactes/solveurs avec les méthodes heuristiques/apprentissage par renforcement. 
	-c) Dans la conclusion du chapitre, incluez une analyse critique globale de l'état de l'art, identifiant les lacunes dans la recherche actuelle et expliquant comment votre travail s'inscrit dans ce contexte.

\chapter{ÉTAT DE L'ART}

\section{Introduction} [Contexte général, importance de l'optimisation de la trajectoire des UAVs dans les réseaux IoT, objectifs du chapitre]

\section{Approches exactes et Solveurs} [Sous-sections sur les différentes approches exactes]

\section{Méthodes Heuristiques et Apprentissage par Renforcement} [Sous-sections sur les différentes méthodes heuristiques et d'apprentissage]

\section{Défis spécifiques dans les réseaux IoT denses} [Discussion sur les problèmes particuliers liés aux environnements denses en capteurs]

\section{Conclusion et perspectives} [Résumé des tendances, identification des lacunes, positionnement de votre travail]