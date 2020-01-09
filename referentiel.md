# Data science responsable et de confiance - Référentiel (WIP)

## Risques

Quels sont les risques que l'on souhaite prévenir ? Nous pouvons essayer de les lister, en les structurant par "risques chapeaux" (RC) :

| # | Risques | Exemples réels |
|:---:|:---|:---|
| **RC1** | **l'exposition de données personnelles ou confidentielles** |  |
| RC1-01 | des datasets contenant des données personnelles ou confidentielles sont exposés | [ré-identification de datasets anonymisés](https://www.wired.com/2007/12/why-anonymous-data-sometimes-isnt/) |
| RC1-02 | l'exploitation malveillante d'un modèle prédictif expose des données personnelles ou confidentielles | [rétro-engineering des résultats d'un algorithme](https://www.abc.net.au/news/2019-03-01/abs-census-vulnerability/10857236) |
| **RC2** | **la prise de décisions inappropriées par des systèmes automatiques**, qui seraient préjudiciables à des personnes ou des organisations |  |
| RC2-01 | la prise de décisions infondées, injustes ou illégitimes du fait de biais discriminatoires dans les données d'entraînement | [cas Apple Card](https://twitter.com/dhh/status/1192540900393705474) ; [algorithme RH d'Amazon](https://www.lefigaro.fr/social/2018/10/11/20011-20181011ARTFIG00096-le-logiciel-de-recrutement-d-amazon-n-aimait-pas-les-femmes.php) |
| RC2-02 | la prise de décisions infondées, injustes ou illégitimes du fait de biais discriminatoires dans les données de test | Cas à identifier |
| RC2-03 | l'utilisation de modèles prédictifs dans des contextes où ils ne sont pas suffisamment performants, pas pertinents, voire dangereux (où leur performance réelle est insuffisante par rapport au déclaré ou à l'attendu) | [exemple de Google Flu Trends en santé](https://science.sciencemag.org/content/343/6176/1203) ; [biais induits par les corpus de texte utilisés pour entraîner un modèle de word embedding](https://arxiv.org/abs/1607.06520) ; [biais et performances limitées du modèle COMPAS de prédiction de la récidive](https://advances.sciencemag.org/content/4/1/eaao5580) |
| **RC3** | **ne pas rendre des comptes de manière responsable à ses parties prenantes** quant aux conséquences de l'usage de modèles prédictifs |  |
| RC3-01 | dans le cas d'un incident avec ou provoqué par un modèle prédictif, ne pas avoir de personne physique ou morale identifiée à qui demander des comptes | [cas de Steve Wozniak avec l'Apple Card](https://twitter.com/stevewoz/status/1193330241478901760) |
| RC3-02 | dans le cas d'un incident avec ou dû à un modèle prédictif : pour l'acteur qui met en oeuvre le modèle, ne pas savoir interpréter et expliquer la prédiction en cause | [les algorithmes de censure automatiques de Facebook ont été moins efficaces lors de l'attentat de Christchurch qu'avec les vidéos de l'EI, que détectent-ils exactement ?](https://techcrunch.com/2019/03/21/facebooks-ai-couldnt-spot-mass-murder/) |
| **RC4** | **avoir une empreinte environnementale irresponsable** |  |
| RC4-01 | ne pas connaître le coût énergétique ou environnemental de l'élaboration et de l'utilisation d'un modèle, ou qu'il soit disproportionné par rapport à l'usage cible du modèle | [AlphaGo en kW vs. 20W pour un humain](https://deepmind.com/blog/article/alphago-zero-starting-scratch) |

## Propositions de thèmes, d'un canevas du référentiel

Propositions de thèmes pour structurer les bonnes pratiques et mesures de prévention des risques :

| # | Thèmes | Descriptions |
|:---:|:---|:---|
| T1 | **Protéger les données personnelles ou confidentielles** | L'utilisation de données personnelles ou confidentielles fait porter le risque d'exposition de celles-ci, ce qui peut avoir des conséquences très préjudiciables pour les producteurs, gestionnaires, ou sujets de ces données. Elles doivent donc être protégées, les risques d'exposition doivent être minimisés. |
| T2 | **Prévenir les biais malencontreux** | L'utilisation de modèles prédictifs élaborés à partir de données historiques peut se révéler néfaste lorsque les données historiques décrivent des phénomènes non souhaitables. Il apparaît indispensable de s'interroger sur ce risque et d'étudier la nature des données utilisées et ce qu'elles représentent. |
| T3 | **Evaluer la performance de manière rigoureuse** | Le score de performance d'un modèle prédictif est déterminant pour son adoption dans des produits, systèmes ou processus. L'évaluation de la performance se doit donc d'être rigoureuse. Une spécification de l'équité recherchée entre populations doit également être définie. En effet, l'équité d'un modèle peut [être définie de plusieur manières qui sont incompatibles entre elles](https://papers.nips.cc/paper/6995-counterfactual-fairness), et l'interprétation de scores de performances doit donc se faire dans le cadre de l'une de ces définitions. |
| T4 | **Etablir et maintenir une généalogie des modèles** | Un modèle prédictif est un objet informatique complexe qui peut évoluer au fil des apprentissages. Tracer les étapes de son élaboration et de son évolution permet d'en constituer une forme de **généalogie**, pré-requis pour **reproduire ou auditer** un modèle. |
| T5 | **Garantir la chaîne de responsabilité des modèles** | Un modèle prédictif peut-être utilisé comme un système automatique, dont les règles de fonctionnement ne sont pas écrites _in extenso_ et ne se prêtent pas ou mal à être explicitées, débattues, ajustées. Des efforts sont nécessaires sur **l'interprétation et l'explication** des choix réalisés à l'aide de ces systèmes. Il apparaît également indispensable de garantir une chaîne de responsabilité claire, de personnes physiques ou morales, pour chaque modèle. |
| T6 | **Minimiser les externalités de l'activité data science** | Les ressources informatiques peuvent être gourmandes en énergie et avoir une empreinte environnementale significative si elles ne sont pas optimisées. Prendre conscience de ce phénomène est indispensable, chercher à mesurer, voire optimiser l'utilisation des ressources est nécessaire. |

## Proposition de mesures

- **T1 - Protéger les données personnelles ou confidentielles**
  - Un processus et une organisation de veille juridique concernant la gestion des données personnelles et la mise en place d'algorithme sont mis en place et documentés.
  - Les concepteurs de modèles sont formés en continue aux différents types d'attaques des modèles.
  - Une cartographie des risques d'attaques à travers les modèles est mise en place comprenant des mesures de prévention.

- **T2 - Prévenir les biais malencontreux**
  -

- **T3 - Evaluer la performance de manière rigoureuse**
  - Les conditions de validité d'un modèle sont explicitées et documentées.
  - L'utilisation d'un modèle se restraint à une utilisation dans un périmètres contraints de conditions dans lequel celui-ci a été validé.
  - La vérification de la validation d'un modèle est réalisée à intervalle de période régulier afin d'éviter la dégénérence du modèle.
  - Une mesure de "fairness" est mise en place et intégrée dans la mesure de performance du modèle.

- **T4 - Etablir et maintenir une généalogie des modèles**
  - Les conditions d'entrainements d'un modèle à sa mise en place et son évolution à travers le temps sont documentées.

- **T5 - Garantir la chaîne de responsabilité des modèles**
  - La chaîne de responsabilités entre le fournisseur de données, le responsable de la conception du modèle et l'exploitant du modèle est décrite et validée par l'ensemble des parties prenantes.
  - Une cartographie des modèles existant et de la criticité des processus afférents est mise en place et maintenue.
  - Une politique de gestion des incidents liés à un modèle est mise en place, comprenant :
    - Le processus d'arrêt d'utilisation d'un modèle en cas de défaillance constatée;
    - Le mode de fonctionnement des processus impactés en cas de nécessité d'arrêt d'utilisation d'un modèle.

- **T6 - Minimiser les externalités de l'activité data science**
  - Une formation à l'éthique liée à l'utilisation de techniques algorithmiques sur des données, ainsi que les modèles prédictifs et les systèmes automatiques en résultant est dispensée à l'ensemble des parties prenantes de l'organisation liées à la conception et l'exploitation de modèles.
  - Un processus de mesure des externalités d'un modèle est mis en place. 
