 
  Dans ce mémoire, nous examinons un réseau de capteurs IoT assisté par un UAV dans un contexte de collecte de données. L'objectif est de minimiser conjointement le temps de mission et l'énergie consommée par le drone, tout en respectant les contraintes liées à la vitesse du drone, à la puissance de transmission moyenne des capteurs, ainsi qu'à la couverture du réseau de capteurs IoT. Ce chapitre présente le modèle de système utilisé durant notre projet de recherche et expose le problème d'optimisation sous une formulation mathématique de la fonction objective. Selon \cite{8663615}, le problème d’optimisation de la trajectoire d'un drone pour la collecte de données dans un réseau de capteurs IoT appartient à la classe des problèmes $\mathcal{NP}$-difficiles, en raison de sa similarité avec une variante du problème du voyageur de commerce (TSP). La démonstration sera fournie dans le chapitre.

Selon \cite{8663615}, le problème d'optimisation de la trajectoire d'un drone pour la collecte de données dans un réseau de capteurs IoT appartient à la classe des problèmes $\mathcal{NP}$-difficiles, en raison de sa similarité avec une variante du problème du voyageur de commerce. La démonstration sera fournie dans le chapitre suivant.

\section{Modélisation du système}
Nous considérons un système IoT distant comprenant un ensemble de capteurs sans fil $\mathcal{S}=\{1, 2, \cdots, N\}$ avec une cardinalité $N$. La collecte de données est assurée par une station de base volante intégrée à un UAV. Les capteurs IoT répartis sur une zone donnée collectent en continu des données sensibles au temps. Ces données contiennent des informations utiles liées au service IoT (par exemple, la surveillance, l'agriculture). Les données générées seront collectées par un UAV à voilure tournante, comme illustré dans la \ref{fig:modelDuSyteme}. Une station d'accueil pour UAV est considérée comme la position initiale, cette dernière peut être assimilée à une station de recharge (en anglais \textit{docking station}) de la mission, et une station au sol représente la position finale de la mission où les données collectées seront transférées vers le bord/le cloud. On note $(x(t),y(t))$ pour représenter les projections dépendantes du temps des coordonnées planes de l'UAV.
\noindent Dans un souci d'efficacité énergétique, l'UAV ne restera pas en stationnement au-dessus de chaque capteur individuel si possible. Au lieu de cela, il se positionnera au-dessus d'un groupe de capteurs IoT grâce à des positions de clusters précalculées, ces derniers peuvent contenir un ou plusieurs capteurs selon la nécessité qui peut être liée à la qualité de la solution. L'ensemble des $K$ clusters est désigné par $\mathcal{C}=\{\mathcal{C}_1, \mathcal{C}_2, \cdots, \mathcal{C}_K\}$, et leurs centroïdes respectifs sont $\mathcal{M}=\{m_1, m_2, \cdots, m_K\}$. Chaque capteur IoT $s \in \mathcal{S}$ appartient à un cluster unique. Le coût maximal de l'UAV en termes de temps et de consommation d'énergie est fixé respectivement à $T$ et $E$. Le problème de l'UAV consiste à desservir autant de dispositifs IoT que possible en collectant des informations à partir des capteurs tout en tenant compte du budget maximal de la mission. Pour ce faire, on utilise un modèle binaire; entre autres, cela signifie que l'UAV opère soit en se déplaçant d'un point à un autre, soit en restant en stationnement pour collecter des données à partir des capteurs IoT au sol. Sans perte de généralité et pour faciliter l'analyse, l'UAV vole à une altitude fixe appropriée $h$ et à une vitesse moyenne de vol optimale $v$, cette dernière est déterminée analytiquement. Les deux paramètres sont donnés par \cite{8663615}.
____

[[PREUVE TSP]]
Preuve que notre problème est $\mathcal{NP}$-difficile

Avant de commence la preuve , nous considérons le problème suivant:
\textbf{Entrée :}
\begin{itemize}
    \item Une position de départ fixe \( s = (0, 0) \).
    \item Une position d'arrivée fixe \( t = (800, 800) \), différente de \( s \).
    \item Un ensemble de points \( M = \{v_1, v_2, \dots, v_n\} \) dispersés dans le plan.
\end{itemize}
Notre objectif est de trouver le chemin le plus court qui part de \( s \), visite exactement une fois chaque point de \( M \), et se termine en \( t \), et prouver que ce problème appartient a la classe des problèmes  $\mathcal{NP}$-difficile.
Nous allons diviser notre preuve en 4 étape principale, une première étape qui rappelle la variante de notre problème et ça ressemblance avec le problème du chemin hamiltonien  que l'on notera (PCH), l’étape 2 consiste a faire la réduction polynomiale du PCH a notre problème,l'avant dernière consiste a faire la correspondance des solutions enfin nous clôturons notre démonstration par un conclusion qui prouve que notre problème optimisation est de nature $\mathcal{NP}$-difficile

\subsection{Étape 1 : Rappel du Problème du Chemin Hamiltonien (PCH)}

Le \textbf{Problème du Chemin Hamiltonien (PCH)} est un problème qui a déjà été prouvée  étant de classe  $\mathcal{NP}$-complet d’après \cite{Karp1972}, ce dernier 

\textbf{Entrée :}

\begin{itemize}
    \item Un graphe non orienté \( G = (V, E) \).
    \item Deux sommets distincts \( s', t' \in V \).
\end{itemize}

\textbf{Question :}

Existe-t-il un chemin dans \( G \) de \( s' \) à \( t' \) qui visite chaque sommet de \( V \) exactement une fois ?

\textbf{Complexité :}

Le PCH est un problème \textbf{NP-complet}.



Pour montrer que notre problème est NP-difficile, nous effectuons une réduction polynomiale du PCH à notre problème en assignant des distances spécifiques, une pratique courante pour prouver qu'un problème est $\mathcal{NP}$-difficile.

Cependant cette transformation reste polynomiale car la construction des distances peut être effectuée en temps polynomial par rapport à la taille de \( G \).