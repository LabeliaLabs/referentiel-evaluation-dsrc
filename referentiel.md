# Data science responsable et de confiance - Référentiel (WIP)

## Risques

Quels sont les risques que l'on souhaite prévenir ? Nous pouvons essayer de les lister, en les structurant par "risques chapeaux" (RC) :

| # | Risques | Exemples réels |
|:---:|:---|:---|
| **RC1** | **l'exposition de données personnelles ou confidentielles** |  |
| RC1-01 | des datasets contenant des données personnelles ou confidentielles sont exposés | [ré-identification de datasets anonymisés](https://www.wired.com/2007/12/why-anonymous-data-sometimes-isnt/) |
| RC1-02 | l'exploitation malveillante d'un modèle prédictif expose des données personnelles ou confidentielles | [rétro-engineering des résultats d'un algorithme](https://www.abc.net.au/news/2019-03-01/abs-census-vulnerability/10857236) |
| RC1-03 | un changement de réglementation expose des données personnelles ou confidentielles jusque là protégées | cloud Act - demandes du régulateur américain |
| RC1-04 | une attaque à travers le modèle expose des données personnelles ou confidentiells | algorithmes malveillants |
| **RC2** | **la prise de décisions inappropriées par des systèmes automatiques**, qui seraient préjudiciables à des personnes ou des organisations |  |
| RC2-01 | la prise de décisions infondées, injustes ou illégitimes du fait de biais discriminatoires dans les données d'entraînement | [cas Apple Card](https://twitter.com/dhh/status/1192540900393705474) ; [algorithme RH d'Amazon](https://www.lefigaro.fr/social/2018/10/11/20011-20181011ARTFIG00096-le-logiciel-de-recrutement-d-amazon-n-aimait-pas-les-femmes.php) |
| RC2-02 | la prise de décisions infondées, injustes ou illégitimes du fait de biais discriminatoires dans les données de test | cas à identifier |
| RC2-02 | la prise de décisions infondées, injustes ou illégitimes du fait de biais discriminatoires dans l'algorithme de conception du modèle | vecteur qui genre une profession dans les systèmes d’apprentissage (cas à creuser) |
| RC2-04 | l'utilisation de modèles prédictifs dans des contextes où ils ne sont pas suffisamment performants, pas pertinents, voire dangereux (où leur performance réelle est insuffisante par rapport au déclaré ou à l'attendu) | [exemple de Google Flu Trends en santé](https://science.sciencemag.org/content/343/6176/1203) ; [biais induits par les corpus de texte utilisés pour entraîner un modèle de word embedding](https://arxiv.org/abs/1607.06520) ; [biais et performances limitées du modèle COMPAS de prédiction de la récidive](https://advances.sciencemag.org/content/4/1/eaao5580) |
| RC2-05 | l'utilisation de modèles prédictifs dans des contextes pour lesquels ils n'étaient pas prévus et validés | cas à identifier |
| RC2-06 | la prise de décisions infondées, injustes ou illégitimes du fait d'une dégénérance dans le temps ou d'un drift du modèle | cas à identifier |
| **RC3** | **ne pas rendre des comptes de manière responsable à ses parties prenantes** quant aux conséquences de l'usage de modèles prédictifs |  |
| RC3-01 | dans le cas d'un incident avec ou provoqué par un modèle prédictif, ne pas avoir de personne physique ou morale identifiée à qui demander des comptes | [cas de Steve Wozniak avec l'Apple Card](https://twitter.com/stevewoz/status/1193330241478901760) |
| RC3-02 | dans le cas d'un incident avec ou dû à un modèle prédictif : pour l'acteur qui met en oeuvre le modèle, ne pas savoir interpréter et expliquer la prédiction en cause | [les algorithmes de censure automatiques de Facebook ont été moins efficaces lors de l'attentat de Christchurch qu'avec les vidéos de l'EI, que détectent-ils exactement ?](https://techcrunch.com/2019/03/21/facebooks-ai-couldnt-spot-mass-murder/) |
| RC3-03 | dans le cas d'un incident avec ou dû à un modèle prédictif : pour l'acteur qui met en oeuvre le modèle, ne plus être capable d'assurer un service critique | cas à identifier |
| **RC4** | **avoir une empreinte sociétale et environnementale irresponsable** |  |
| RC4-01 | ne pas connaître le coût énergétique ou environnemental de l'élaboration et de l'utilisation d'un modèle, ou qu'il soit disproportionné par rapport à l'usage cible du modèle | [AlphaGo en kW vs. 20W pour un humain](https://deepmind.com/blog/article/alphago-zero-starting-scratch) |
| RC4-02 | ne pas avoir anticiper les impacts sociaux de la mise en place d'un modèle | cas à identifier |
| RC4-03 | ne pas avoir anticiper une utilisation potentielle négative et dangereuse lors de la conception d'un modèle | mise en place de la reconnaissance faciale |

## Propositions de thèmes, d'un canevas du référentiel

Propositions de thèmes pour structurer les bonnes pratiques et mesures de prévention des risques :

| # | Thèmes | Descriptions |
|:---:|:---|:---|
| T1 | **Protéger les données personnelles ou confidentielles** | L'utilisation de données personnelles ou confidentielles fait porter le risque d'exposition de celles-ci, ce qui peut avoir des conséquences très préjudiciables pour les producteurs, gestionnaires, ou sujets de ces données. Elles doivent donc être protégées, les risques d'exposition doivent être minimisés. |
| T2 | **Prévenir les biais malencontreux** | L'utilisation de modèles prédictifs élaborés à partir de données historiques peut se révéler néfaste lorsque les données historiques décrivent des phénomènes non souhaitables. Il apparaît indispensable de s'interroger sur ce risque et d'étudier la nature des données utilisées et ce qu'elles représentent. |
| T3 | **Evaluer la performance de manière rigoureuse** | Le score de performance d'un modèle prédictif est déterminant pour son adoption dans des produits, systèmes ou processus. L'évaluation de la performance se doit donc d'être rigoureuse. Une spécification de l'équité recherchée entre populations doit également être définie. En effet, l'équité d'un modèle peut [être définie de plusieur manières qui sont incompatibles entre elles](https://papers.nips.cc/paper/6995-counterfactual-fairness), et l'interprétation de scores de performances doit donc se faire dans le cadre de l'une de ces définitions. |
| T4 | **Etablir et maintenir une généalogie des modèles** | Un modèle prédictif est un objet informatique complexe qui peut évoluer au fil des apprentissages. Tracer les étapes de son élaboration et de son évolution permet d'en constituer une forme de **généalogie**, pré-requis pour **reproduire ou auditer** un modèle. |
| T5 | **Garantir la chaîne de responsabilité des modèles** | Un modèle prédictif peut-être utilisé comme un système automatique, dont les règles de fonctionnement ne sont pas écrites _in extenso_ et ne se prêtent pas ou mal à être explicitées, débattues, ajustées. Des efforts sont nécessaires sur **l'interprétation et l'explication** des choix réalisés à l'aide de ces systèmes. Il apparaît également indispensable de garantir une chaîne de responsabilité claire, de personnes physiques ou morales, pour chaque modèle. |
| T6 | **Minimiser les externalités de l'activité data science** | La mise en place d'un modèle peut générer des externalités négatives, tant d'un point de vue sociétal que environnemental. Prendre conscience de ce phénomène est indispensable, ainsi que chercher à mesurer les différents impacts négatifs pour les limiter et optimiser l'utilisation des ressources. |

## Proposition de mesures

- **T1 - Protéger les données personnelles ou confidentielles**
  - Un processus et une gouvernance de gestion de la donnée personnelle et confidentielle est mis en place dans le cadre de la conception de modèles.
  - Un processus et une organisation de veille juridique et réglementaire concernant la gestion des données personnelles et la conception de modèles sont mis en place et documentés.
  - Les concepteurs de modèles sont formés en continue aux différents types d'attaques des modèles.
  - Une cartographie des risques d'attaques à travers les modèles est mise en place comprenant des mesures de prévention.

- **T2 - Prévenir les biais malencontreux**
  - Un processus de contrôle du risque de biais est documenté et mis en place.
  - Un processus de suspension ou de restriction de l'utilisation d'un modèle est documenté et mis en place lorsqu'un biais dans les données, le modèle ou l'algorithme est détecté.

- **T3 - Evaluer la performance de manière rigoureuse**
  - Les conditions de validité d'un modèle sont explicitées et documentées.
  - L'utilisation d'un modèle se restraint à une utilisation dans un périmètres contraints de conditions dans lequel celui-ci a été validé.
  - Un proceessus de vérification de la validation d'un modèle  à intervalle de période régulier est mis en place afin d'éviter la dégénérence d'un modèle.
  - Une mesure de "fairness" est mise en place et intégrée dans la mesure de performance du modèle.

- **T4 - Etablir et maintenir une généalogie des modèles**
  - Les conditions d'entrainements d'un modèle à sa mise en place et son évolution à travers le temps sont documentées.

- **T5 - Garantir la chaîne de responsabilité des modèles**
  - La chaîne de responsabilités entre le fournisseur de données, le responsable de la conception du modèle et l'exploitant du modèle est décrite et validée par l'ensemble des parties prenantes.
  - Une cartographie des modèles existant et de la criticité des processus afférents est mise en place et maintenue.
  - Une politique de gestion des incidents liés à un modèle est mise en place, comprenant :
    - Le processus d'arrêt de l''utilisation d'un modèle en cas de défaillance constatée;
    - Le mode de fonctionnement des processus impactés en cas de nécessité d'arrêt de l''utilisation d'un modèle.
  - Un responsable point de contact est défini et identifiable par les exploitants directs et indirects du modèle.

- **T6 - Minimiser les externalités de l'activité data science**
  - Une formation à l'éthique liée à l'utilisation de modèles est dispensée à l'ensemble des parties prenantes de l'organisation liées à la conception et l'exploitation de modèles.
  - Un processus de mesure des externalités d'un modèle est mis en place.
