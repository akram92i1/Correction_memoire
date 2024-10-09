Description de l'algorithme SCA de référence:

L'algorithme SCA est appliqué dans le modèle Fly-Hover-Communicate du papier de référence  pour optimiser la trajectoire d'un drone et calculer les meilleures positions de vol stationnaire qkq_kqk​ où le drone communique avec les nœuds au sol (Ground Nodes, GNs). L'objectif est de minimiser l'énergie totale consommée, y compris l'énergie de propulsion et l'énergie de communication. À cette fin, SCA permet de résoudre itérativement les sous-problèmes convexes afin de déterminer ces positions $q_k$​, ainsi que la durée de vol et de communication à chaque position. Cela permet d'optimiser simultanément la trajectoire du drone et l'allocation du temps de communication.

Plus précisément, l'algorithme transforme un problème complexe non convexe en plusieurs sous-problèmes convexes plus faciles à résoudre. À chaque itération, une approximation convexe du problème est résolue, et la solution est progressivement affinée jusqu'à convergence vers une solution localement optimale, conforme aux conditions KKT (Karush-Kuhn-Tucker).

Toutefois, il convient de noter que la méthodologie complète et les détails mathématiques de l'implémentation de cet algorithme SCA, ainsi que son application pour déterminer les positions optimales qkq_kqk​, sont présentés en détail dans l'article de référence de Zeng et al. (2018). Pour une compréhension approfondie des aspects techniques de l'algorithme, nous recommandons la consultation de la publication originale disponible
_____


L'algorithme \textit{Approximations Convexes Successives (SCA)} est appliqué dans le modèle (en anglais : Fly-Hover-Communicate) du papier de référence dans le but d'optimiser la trajectoire d'un drone et de calculer les meilleures positions de vol stationnaire $q_k$ où le drone communique avec les nœuds au sol (en anglais : Ground Nodes, GNs), qui renvoient aux capteurs. L'objectif est de minimiser l'énergie totale consommée par le drone, en optimisant l’énergie de communication en gérant les positions de vol stationnaire $q_k$, ainsi que l’énergie de propulsion grâce à une vitesse optimale nommée $V_{mr}$.

Dans cette optique, l'utilisation de l'algorithme SCA permet l'optimisation des positions $q_k$ grâce au processus itératif. Cependant, certaines contraintes sont non convexes, plus précisément la contrainte liée à la distance de communication, ainsi que la distance totale parcourue, notée $D^{tr}$ dans \cite{8663615}. Cela est dû à la racine de la distance euclidienne qui rend le problème quadratique, donc non convexe. L’introduction des variables de relâchement (en anglais : slack variables), comme la variable $\eta_{k}$, qui est liée au débit de communication, permet que toutes les contraintes soient respectées tout en rendant le problème résoluble par approximation convexe. Par la suite, les sous-problèmes convexes sont résolus. Cela permet d'optimiser simultanément la trajectoire du drone et l'allocation du temps de communication.

Plus précisément, à chaque itération de l'algorithme, une approximation convexe du problème est résolue à l'aide du solveur CVX, et la solution est progressivement affinée jusqu'à convergence vers une solution localement optimale qui respecte les conditions KKT (Karush-Kuhn-Tucker).

Cependant, il est nécessaire de noter que pour une compréhension approfondie des aspects techniques, la modélisation entière ainsi que les détails mathématiques de l’implémentation de l'approche SCA à l'aide du solveur CVX sont présentés en détail dans l'article de référence \cite{8663615}.





Cependant , certaines contraintes sont non convexe dans le papier plus exactement  la contrainte liée a la distance de communications , ainsi que la distance totale parcourue noté  $D^{tr}$ dans le papier et ce a cause de la racine de la distance euclidienne qui rend le problème quadratique donc non-convexe, l’introduction des variable de relâchement  (en anglais: slack variables) comme la variable $\eta_{k}$  qui est liée au débit de communication permet que toute les contraintes soit respectées tout en rendant le problème résoluble par approximation convexe.     


___
Afin de faciliter la résolution des contraintes non-convexes, telles que celles relatives à la distance de communication entre le drone et les capteurs, des **slack variables** sont introduites. Ces variables d'écart permettent de simplifier les expressions complexes et d'assurer que les contraintes de communication et d'énergie sont respectées tout en rendant le problème résoluble par approximation convexe.






