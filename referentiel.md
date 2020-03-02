# Data science responsable et de confiance - Référentiel (WIP)

Le [référentiel](#référentiel-de-la-data-science-responsable-et-de-confiance) ci-dessous est en cours d'élaboration (section 3 ci-dessous). Il procède de l'identification des [risques](#risques) que l'on cherche à prévenir dans la pratique responsable et de confiance de la data science (section 1 ci-dessous). Il est structuré en plusieurs [thèmes](#thèmes-canevas-du-référentiel) complémentaires (section 2 ci-dessous).

## 1. Risques

Quels sont les risques que l'on souhaite prévenir pour pouvoir parler de data science _responsable_ et _de confiance_ ?

| # | Risques | Exemples réels |
|:---:|:---|:---|
|  |  |  |
| **EDP** | **l'Exposition de Données Personnelles ou confidentielles** (e.g. données personnelles ou données privées d'une organisation) |  |
| EDP-01 | des datasets contenant des données personnelles ou confidentielles sont exposés | [ré-identification de datasets anonymisés](https://www.wired.com/2007/12/why-anonymous-data-sometimes-isnt/) ; [article Nature](https://www.nature.com/articles/s41467-019-10933-3/) : "Using our model, we find that 99.98% of Americans would be correctly re-identified in any dataset using 15 demographic attributes."|
| EDP-02 | l'exploitation malveillante d'un modèle prédictif expose des données personnelles ou confidentielles | [rétro-engineering des résultats d'un algorithme](https://www.abc.net.au/news/2019-03-01/abs-census-vulnerability/10857236) |
| EDP-03 | un algorithme d'apprentissage machine est utilisé de manière malveillante pour extraire des données personnelles ou confidentielles d'un dataset d'entraînement ou de test |  |
| EDP-04 | des dispositions réglementaires font peser des risques, ou un changement réglementaire augmente les risques d'exposition de données personnelles ou confidentielles | Cloud Act ; [FATCA](https://www.cnil.fr/fr/cnil-direct/question/loi-fatca-que-faire) en contradiction avec le droit européen ; [CNB - Mise en garde HDH](https://www.cnb.avocat.fr/sites/default/files/11.cnb-mo2020-01-11_ldh_health_data_hubfinal-p.pdf) |
|  |  |  |
| **PDI** | **la Prise de Décisions Inappropriées par des systèmes automatiques**, qui seraient préjudiciables à des personnes ou des organisations (inappropriées : infondées, injustes ou illégitimes) |  |
| PDI-01 | la prise de décisions inappropriées du fait de biais discriminatoires dans les données d'entraînement ou de test | [cas Apple Card](https://twitter.com/dhh/status/1192540900393705474) ; [algorithme RH d'Amazon](https://www.lefigaro.fr/social/2018/10/11/20011-20181011ARTFIG00096-le-logiciel-de-recrutement-d-amazon-n-aimait-pas-les-femmes.php) ; [reconnaissance faciale](https://www.thesun.co.uk/news/5182512/chinese-users-claim-iphonex-face-recognition-cant-tell-them-apart/) ; [biais dans les systèmes de reconnaissance visuelle](https://arxiv.org/pdf/1902.11097.pdf) |
| PDI-02 | la prise de décisions inappropriées du fait de biais discriminatoires dûs à l'architecture ou la conception même de l'algorithme d'apprentissage et/ou du modèle | [doc2vec](https://www.pnas.org/content/115/16/E3635) |
| PDI-03 | la prise de décisions inappropriées du fait de données empoisonnées (de manière malveillante, ou du fait de phénomènes diffus, mal compris) | [social cooling](https://usbeketrica.com/article/le-social-cooling-symptome-numerique-de-la-surveillance-de-masse) |
| PDI-04 | la prise de décisions inappropriées du fait de l'utilisation de données synthétiques (**_à préciser_**) | |
| PDI-05 | l'utilisation de modèles prédictifs dans des contextes pour lesquels ils ne sont pas suffisamment performants, pas pertinents voire dangereux, pas prévus et validés (où leur performance réelle est insuffisante par rapport au déclaré ou à l'attendu) | [exemple de Google Flu Trends en santé](https://science.sciencemag.org/content/343/6176/1203) ; [biais induits par les corpus de texte utilisés pour entraîner un modèle de word embedding](https://arxiv.org/abs/1607.06520) ; [biais et performances limitées du modèle COMPAS de prédiction de la récidive](https://advances.sciencemag.org/content/4/1/eaao5580) |
| PDI-06 | l'utilisation de modèles ayant subi une dégénérescence ou _drift_ dans le temps (par exemple, dans les cas de figure d'apprentissage en continu, lorsque les nouvelles données inputs proviennent, même indirectement, de situations dans lesquels le modèle a été utilisé) | cas à identifier (problème de capteurs de mesure en maintenance prédictive, trading...) |
| PDI-07 | l'utilisation adversariale d'un modèle prédictif de manière préjudiciable à des personnes ou des organisations | [Three Small Stickers in Intersection Can Cause Tesla Autopilot to Swerve Into Wrong Lane](https://spectrum.ieee.org/cars-that-think/transportation/self-driving/three-small-stickers-on-road-can-steer-tesla-autopilot-into-oncoming-lane) |
|  |  |  |
| **RC** | **ne pas Rendre des Comptes de manière responsable à ses parties prenantes** quant aux conséquences de l'usage de modèles prédictifs |  |
| RC-01 | dans le cas d'un incident avec ou provoqué par un modèle prédictif, ne pas avoir de personne physique ou morale identifiée à qui demander des comptes | [cas de Steve Wozniak avec l'Apple Card](https://twitter.com/stevewoz/status/1193330241478901760) |
| RC-02 | dans le cas d'un incident avec ou dû à un modèle prédictif : pour l'acteur qui met en oeuvre et opère le modèle, ne pas savoir réagir face à une demande d'interpréter et expliquer une prédiction mise en cause | [les algorithmes de censure automatiques de Facebook ont été moins efficaces lors de l'attentat de Christchurch qu'avec les vidéos de l'EI, que détectent-ils exactement ?](https://techcrunch.com/2019/03/21/facebooks-ai-couldnt-spot-mass-murder/) |
| RC-03 | dans le cas d'un incident avec ou dû à un modèle prédictif : pour l'acteur qui met en oeuvre et opère le modèle, ne plus être capable d'assurer un service critique | cas à identifier |
| RC-04 | au sein d'une organisation qui utilise des systèmes automatiques basés sur des modèles prédictifs, ne pas connaître ou ne pas savoir identifier facilement qui sont les responsables de ces systèmes |  |
|  |  |  |
| **ESE** | **avoir une Empreinte Sociale et Environnementale irresponsable** |  |
| ESE-01 | ne pas connaître ou ne pas se préoccuper du coût énergétique ou environnemental de l'élaboration et de l'utilisation d'un modèle, ou qu'il soit disproportionné par rapport à l'usage cible du modèle | [AlphaGo en kW vs. 20W pour un humain](https://deepmind.com/blog/article/alphago-zero-starting-scratch) ; [ML Impact Calculator](https://mlco2.github.io/impact/) |
| ESE-02 | ne pas anticiper les impacts sociaux de l'élaboration ou de la mise en place d'un système automatique basé sur un modèle prédictif | en amont pour la production de données annotées par exemple, en aval pour l'évolution des activités impactées |
| ESE-03 | ne pas anticiper les effets négatifs/dangereux ou les usages malfaisants d'un modèle lors de la conception | [Implication analysis and release strategy of gpt2 by OpenAI](https://openai.com/blog/better-language-models/) |
|  |  |  |
| **TR** | **Transverse** |  |
| TR-01 | ne pas maîtriser les conséquences négatives de l'utilisation d'un modèle donné du fait du manque d'une "gouvernance globale" et de pertes de connaissances/contexte tout au long de la chaîne de valeur de bout-en-bout (données, conception, entraînement, validation, exploitation) |  |
| TR-02 | ne pas maîtriser les conséquences de l'utilisation d'un modèle du fait du manque de connaissance de sa généalogie et de maîtrise de ses conditions nominales d'utilisation | modèles qui deviennent des références et/ou fournis par des tiers |
|  |  |  |
|  | **divers - à catégoriser** |  |
|  | se faire "voler" un modèle par multiples inférences (_model stealing_) |  |
|  | se faire "voler" du temps de calcul par _adversarial reprogramming_ |  |
|  |  | placement d'offres d'emploi sur les flux d'utilisateurs sélectionnés par un modèle prédictif : y a-t-il un sens à s'interroger sur un risque de discrimination, ou bien est-ce analogue à un chasseur de tête qui décide d'appeler les candidats qui l'intéressent de manière discrétionnaire ? |

## 2. Thèmes - Canevas du référentiel

Propositions de thèmes pour structurer les bonnes pratiques et mesures de prévention des risques qui constituent le référentiel :

| # | Thèmes | Descriptions |
|:---:|:---|:---|
| T1 | **Protéger les données personnelles ou confidentielles** | L'utilisation de données personnelles ou confidentielles fait porter le risque d'exposition de celles-ci, ce qui peut avoir des conséquences très préjudiciables pour les producteurs, gestionnaires, ou sujets de ces données. Elles doivent donc être protégées, les risques d'exposition doivent être minimisés. |
| T2 | **Prévenir les biais malencontreux** | L'utilisation de modèles prédictifs élaborés à partir de données historiques peut se révéler néfaste lorsque les données historiques décrivent des phénomènes non souhaitables. Il apparaît indispensable de s'interroger sur ce risque et d'étudier la nature des données utilisées et ce qu'elles représentent. |
| T3 | **Evaluer la performance de manière rigoureuse** | Le score de performance d'un modèle prédictif est déterminant pour son adoption dans des produits, systèmes ou processus. L'évaluation de la performance se doit donc d'être rigoureuse. Une spécification de l'équité recherchée entre populations doit également être définie. En effet, l'équité d'un modèle peut [être définie de plusieurs manières qui sont incompatibles entre elles](https://papers.nips.cc/paper/6995-counterfactual-fairness), et l'interprétation de scores de performances doit donc se faire dans le cadre de l'une de ces définitions. |
| T4 | **Etablir et maintenir une généalogie des modèles** | Un modèle prédictif est un objet informatique complexe qui peut évoluer au fil des apprentissages. Tracer les étapes de son élaboration et de son évolution permet d'en constituer une forme de **généalogie**, pré-requis pour **reproduire ou auditer** un modèle. |
| T5 | **Garantir la chaîne de responsabilité des modèles** | Un modèle prédictif peut-être utilisé comme un système automatique, dont les règles de fonctionnement ne sont pas écrites _in extenso_ et ne se prêtent pas ou mal à être explicitées, débattues, ajustées. Des efforts sont nécessaires sur **l'interprétation et l'explication** des choix réalisés à l'aide de ces systèmes. Il apparaît également indispensable de garantir une chaîne de responsabilité claire, de personnes physiques ou morales, pour chaque modèle. |
| T6 | **Anticiper, suivre et minimiser les externalités négatives de l'activité data science** | La mise en place d'un système automatique basé sur un modèle prédictif peut générer des externalités négatives sociales et environnementales. En prendre conscience est indispensable, ainsi qu'anticiper, chercher à suivre et minimiser les différents impacts négatifs. |

## 3. Référentiel de la data science responsable et de confiance

- **T1 - Protéger les données personnelles ou confidentielles**

  1. **Gouvernance des données personnelles ou confidentielles** : Dans le cadre des projets de data science, une gouvernance des données personnelles ou confidentielles est mise en place, en organisant le stockage, l'accès, le transfert, la protection, la responsabilité.

  1. **Collecte des données personnelles ou confidentielles** : Dans le cadre de projets de data science, le nombre et le type de données collectées sont minimisés aux usages identifiés. Les données personnelles ne sont collectées que par nécessité. Un principe de minimisation de la collecte est appliquée.   

  1. **Identification de la législation et des exigences contractuelles applicables** : Toutes les exigences légales, statutaires, réglementaires et contractuelles en vigueur, ainsi que l’approche adoptée par l’organisation pour satisfaire à ces exigences, doivent être explicitement définies, documentées et mises à jour pour chaque traitement de données personnelles ou confidentielles.
  Un processus de veille réglementaire doit être mis en place et documenté.

  1. **Les principales vulnérabilités et attaques de modèles prédictifs** au regard des données confidentielles sont connues, ainsi que les bonnes pratiques et mesures de réduction des risques. Une veille technique est organisée pour tenir à jour ces connaissances. Elles sont prises en compte dans les PIA des traitements de données nécessaires aux projets de data science. Les collaborateurs intervenant sur des projets data science y sont formés régulièrement.

  1. **Les approches limitant l'accès aux données ou le transfert de données, ainsi que les techniques de _privacy enhancement_** (comme par exemple : _remote execution_, _secure multi-party computation_, anonymisation, _differential privacy_, chiffrement homomorphe, etc.) sont prises en compte dans la conception de projets de data science, les choix de les utiliser ou non sont documentés et intégrés à la "généalogie de bout-en-bout" des modèles conçus, entraînés, validés et exploités.

  1. **Lien avec les autorités :** En cas d'attaques ou de mise en danger de données personnelles ou confidentielles, les autorités compétentes sont averties des failles et vulnérabilités rencontrées.   

- **T2 - Prévenir les biais malencontreux**

  1. **Analyse des données d'entrainement utilisées :** Prendre en compte l'origine, la distribution des données d'entraînement, et les phénomènes intempestifs, discriminatoires ou non-souhaitables qui s'y sont glissés du fait de l'époque, du contexte, des processus et outils mis en oeuvre pour les collecter.

  1. **Mesures de Fairness :** Une ou plusieurs mesures de justice et d'équité (_fairness metrics_) sont étudiées et évaluées. Les choix desquelles utiliser sont documentés et intégrés à la "généalogie de bout-en-bout" des modèles.

  1. **Mesures de robustesse :** Une ou plusieurs mesures de robustesse (_robustness metrics_) sont étudiées et évaluées. Les choix desquelles utiliser sont documentés et intégrés à la "généalogie de bout-en-bout" des modèles.  

  1. **Identification des biais discriminatoires :** Les risques de biais discriminatoires sont évalués sur des données de test comprenant différentes sous-populations cibles, et les variables (ou variables proxy) pouvant y conduire sont recherchées.

  1. **Utilisation de données synthétiques :** Les données synthétiques, les approches de _data augmentation_ ou _re-weighting_ doivent être documentés et intégrés à la "généalogie de bout-en-bout" des modèles.

- **T3 - Evaluer la performance de manière rigoureuse**

  1. **Séparation des jeux de test :** Les jeux de données utilisés pour le test de la performance d'un modèle doivent être isolés et protégés de manière à ne pas contaminer l'apprentissage.

  1. **Contamination des données de test :** Un processus d'identification et de correction dont être mis en place en cas de contamination des données de test.  

  1. **Analyse des données de test :** Prendre en compte l'origine, la distribution des données de test, et les phénomènes intempestifs, discriminatoires ou non-souhaitables qui s'y sont glissés du fait de l'époque, du contexte, des processus et outils mis en oeuvre pour les collecter.

  1. **Validation des performances :** Les bonnes pratiques statistiques de validation rigoureuse de la performance d'un modèle (par exemple définition de la métrique de performance en amont de l'apprentissage), permettant d'éviter l'obtention de score de performance non significatif, doivent être connues et suivies.

  1. **Persistance dans le temps :** Un processus de vérification de la validation d'un modèle à intervalle régulier est mis en place afin d'éviter la dégénérescence d'un modèle.

  1. **Gestion des changements :** Un processus de vérification de la validation d'un modèle est mis en place à chaque changement significatif, et lors de toute nouvelle mise en production d'un modèle.

  1. **Nouvelle application :** Un processus de vérification de la validation d'un modèle est mis en place à chaque nouvelle application différente du modèle.

  1. **Contrôle aléatoire humain :** Un processus de contrôle aléatoire humain est mis en place pour s'assurer de la conformité du modèle et des résultats attendus.  

  1. **Persistance des tests :** La pertinence des tests effectués sur les modèles et leurs applications est évaluée à intervalle régulier.

  1. **Prédictions indéfinies :** Aux frontières de décisions, un classificateur doit avoir une plage de prédiction "indéfinie". Les seuils définissant ces plages doivent être explicités et intégrés à la "généalogie de bout-en-bout" des modèles.

- **T4 - Etablir et maintenir une généalogie des modèles**

  1. **Une "généalogie de bout-en-bout" des modèles** alimentée et tenue à jour dans le cadre des projets de data science, tout au long des phase de collecte de données, conception, entraînement, validation et exploitation.

  1. **Conditions d'utilisation d'un modèle :** Les "conditions de validité" ou le "contexte d'utilisation recommandée" d'un modèle conçu, entraîné et validé par l'organisation sont explicités et documentés.

  1. **Limites d'utilisation d'un modèle :** Les "limites d'utilisation" d'un modèle conçu, entraîné et validé par l'organisation sont explicitées et documentées.

  1. **Usage des modèles :** L'utilisation par l'organisation de modèles prédictifs s'effectue dans les conditions et pour les usages pour lesquels les modèles prédictifs en question ont été validés.

  1. **Le "niveau d'interprétabilité"** qu'il est possible d'obtenir avec un modèle donné (sur une échelle allant d'une preuve/vérité objective à une simple prédiction sans niveau de confiance) doit être explicités et intégrés aux "conditions de validité" ou au "contexte d'utilisation recommandée" d'un modèle.

  1. **Interprétabilité :** Des outils d'interprétabilité doivent être mis à disposition de toutes les parties prenantes, adaptés en sophistication en fonction de leur niveau de compréhension des algorithmes et modèles.

- **T5 - Garantir la chaîne de responsabilité des modèles**

  1. **La chaîne de responsabilités** entre le(s) fournisseur(s) de données, le responsable de la conception du modèle et l'exploitant du modèle est décrite et validée par l'ensemble des parties prenantes.

  1. **Une politique de gestion des incidents** liés à un modèle est mise en place, comprenant :
      - Une cartographie des modèles existant et de la criticité des processus afférents.
      - Le processus d'arrêt de l'utilisation d'un modèle en cas de défaillance constatée.
      - Le mode de fonctionnement des processus impactés en cas de nécessité d'arrêt de l'utilisation d'un modèle.
      - Un processus de suspension ou de restriction de l'utilisation d'un modèle est documenté lorsqu'un biais dans les données, le modèle ou l'algorithme est détecté.

  1. **Responsabilité :** Un responsable point de contact est défini et identifiable par les exploitants directs et indirects du modèle.
    - _A définir : indépendance ou non ? quel rôle précis ? Une personne par rôle (modèle, données, applications) ?_

  1. **Un processus de contournement** est mis en place permettant à un être humain opérateur, dans certaines conditions définies, d'aller contre une décision du modèle s'il soupçonne que le modèle commet une erreur.

  1. **Sous-traitance :** les tâches sous-traitées auprès d'un organisme tier sont soumises aux mêmes exigences.

- **T6 - Anticiper, suivre et minimiser les externalités négatives de l'activité data science**

  1. **Les externalités négatives environnementales** liées à l'usage d'un modèle prédictif ou d'un système automatique basé dessus doivent être évaluées, prévenues et suivies.

  1. **Les externalités négatives societales** (exemple : impact sur les emplois, ...) liées à l'usage d'un modèle prédictif ou d'un système automatique basé dessus doivent être évaluées, prévenues et suivies.

  1. **Une formation à l'éthique** liée à l'utilisation de modèles est dispensée à l'ensemble des parties prenantes de l'organisation liées à la conception et l'exploitation de modèles.
