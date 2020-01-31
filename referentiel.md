# Data science responsable et de confiance - Référentiel (WIP)

Le [référentiel](#référentiel-de-bonnes-pratiques-définissant-la-data-science-responsable-et-de-confiance) ci-dessous est en cours d'élaboration. Il procède de l'identification des [risques](#risques) que l'on cherche à prévenir dans la pratique responsable et de confiance de la data science. Il est structuré en plusieurs [thèmes](#thèmes-canevas-du-référentiel) complémentaires.

## Risques

Quels sont les risques que l'on souhaite prévenir pour pouvoir parler de data science _responsable et de confiance_ ?

| # | Risques | Exemples réels |
|:---:|:---|:---|
|  |  |  |
| **EDP** | **l'Exposition de Données Personnelles ou confidentielles** |  |
| EDP-01 | des datasets contenant des données personnelles ou confidentielles sont exposés | [ré-identification de datasets anonymisés](https://www.wired.com/2007/12/why-anonymous-data-sometimes-isnt/) |
| EDP-02 | l'exploitation malveillante d'un modèle prédictif expose des données personnelles ou confidentielles | [rétro-engineering des résultats d'un algorithme](https://www.abc.net.au/news/2019-03-01/abs-census-vulnerability/10857236) |
| EDP-03 | un algorithme d'apprentissage machine est utilisé de manière malveillante pour extraire des données personnelles ou confidentielles d'un dataset d'entraînement ou de test |  |
| EDP-04 | un changement de réglementation augmente le risque d'exposition de données personnelles ou confidentielles | Cloud Act ; [CNB - "Risques sur le Health Data Hub"](https://www.cnb.avocat.fr/sites/default/files/11.cnb-mo2020-01-11_ldh_health_data_hubfinal-p.pdf) |
|  |  |  |
| **PDI** | **la Prise de Décisions Inappropriées par des systèmes automatiques**, qui seraient préjudiciables à des personnes ou des organisations |  |
| PDI-01 | la prise de décisions infondées, injustes ou illégitimes du fait de biais discriminatoires dans les données d'entraînement | [cas Apple Card](https://twitter.com/dhh/status/1192540900393705474) ; [algorithme RH d'Amazon](https://www.lefigaro.fr/social/2018/10/11/20011-20181011ARTFIG00096-le-logiciel-de-recrutement-d-amazon-n-aimait-pas-les-femmes.php) |
| PDI-02 | la prise de décisions infondées, injustes ou illégitimes du fait de biais discriminatoires dans les données de test | cas à identifier |
| PDI-03 | la prise de décisions infondées, injustes ou illégitimes du fait de biais discriminatoires dûs à l'architecture ou la conception-même de l'algorithme d'apprentissage et/ou du modèle | word embedding > vecteur qui genre une profession (cas à creuser) |
| PDI-04 | la prise de décisions infondées, injustes ou illégitimes du fait de données empoisonnées | |
| PDI-05 | l'utilisation de modèles prédictifs dans des contextes pour lesquels ils ne sont pas suffisamment performants, pas pertinents voire dangereux, pas prévus et validés (où leur performance réelle est insuffisante par rapport au déclaré ou à l'attendu) | [exemple de Google Flu Trends en santé](https://science.sciencemag.org/content/343/6176/1203) ; [biais induits par les corpus de texte utilisés pour entraîner un modèle de word embedding](https://arxiv.org/abs/1607.06520) ; [biais et performances limitées du modèle COMPAS de prédiction de la récidive](https://advances.sciencemag.org/content/4/1/eaao5580) |
| PDI-06 | l'utilisation de modèles ayant subi une dégénérescence ou _drift_ dans le temps (par exemple, dans les cas de figure d'apprentissage en continu, lorsque les nouvelles données inputs proviennent de situations dans lesquels le modèle a été utilisé) | cas à identifier |
| PDI-07 | l'utilisation adversariale d'un système automatique basé sur un modèle prédictif de manière préjudiciable à des personnes ou des organisations | [Three Small Stickers in Intersection Can Cause Tesla Autopilot to Swerve Into Wrong Lane](https://spectrum.ieee.org/cars-that-think/transportation/self-driving/three-small-stickers-on-road-can-steer-tesla-autopilot-into-oncoming-lane) |
|  |  |  |
| **RC** | **ne pas Rendre des Comptes de manière responsable à ses parties prenantes** quant aux conséquences de l'usage de modèles prédictifs |  |
| RC-01 | dans le cas d'un incident avec ou provoqué par un modèle prédictif, ne pas avoir de personne physique ou morale identifiée à qui demander des comptes | [cas de Steve Wozniak avec l'Apple Card](https://twitter.com/stevewoz/status/1193330241478901760) |
| RC-02 | dans le cas d'un incident avec ou dû à un modèle prédictif : pour l'acteur qui met en oeuvre le modèle, ne pas savoir interpréter et expliquer la prédiction en cause | [les algorithmes de censure automatiques de Facebook ont été moins efficaces lors de l'attentat de Christchurch qu'avec les vidéos de l'EI, que détectent-ils exactement ?](https://techcrunch.com/2019/03/21/facebooks-ai-couldnt-spot-mass-murder/) |
| RC-03 | dans le cas d'un incident avec ou dû à un modèle prédictif : pour l'acteur qui met en oeuvre le modèle, ne plus être capable d'assurer un service critique | cas à identifier |
|  |  |  |
| **ESE** | **avoir une Empreinte Sociale et Environnementale irresponsable** |  |
| ESE-01 | ne pas connaître le coût énergétique ou environnemental de l'élaboration et de l'utilisation d'un modèle, ou qu'il soit disproportionné par rapport à l'usage cible du modèle | [AlphaGo en kW vs. 20W pour un humain](https://deepmind.com/blog/article/alphago-zero-starting-scratch) ; [ML Impact Calculator](https://mlco2.github.io/impact/) |
| ESE-02 | ne pas anticiper les impacts sociaux de la mise en place d'un système automatique basé sur un modèle prédictif | cas à identifier |
| ESE-03 | ne pas anticiper les effets négatifs/dangereux ou les usages malfaisants d'un modèle lors de la conception | mise en place de la reconnaissance faciale |
|  |  |  |
| **TR** | **Transverse** |  |
| TR-01 | ne pas maîtriser les conséquences négatives de l'utilisation d'un modèle donné du fait du manque d'une "gouvernance globale" et de pertes de connaissances/contexte tout au long de la chaîne données, conception, entraînement, validation, exploitation |  |
|  |  |  |
|  | **divers - à catégoriser** |  |
|  | se faire "voler" un modèle par multiples inférences (_model stealing_) |  |
|  | se faire "voler" du temps de calcul par _adversarial reprogramming_ |  |

## Thèmes, canevas du référentiel

Propositions de thèmes pour structurer les bonnes pratiques et mesures de prévention des risques qui constituent le référentiel :

| # | Thèmes | Descriptions |
|:---:|:---|:---|
| T1 | **Protéger les données personnelles ou confidentielles** | L'utilisation de données personnelles ou confidentielles fait porter le risque d'exposition de celles-ci, ce qui peut avoir des conséquences très préjudiciables pour les producteurs, gestionnaires, ou sujets de ces données. Elles doivent donc être protégées, les risques d'exposition doivent être minimisés. |
| T2 | **Prévenir les biais malencontreux** | L'utilisation de modèles prédictifs élaborés à partir de données historiques peut se révéler néfaste lorsque les données historiques décrivent des phénomènes non souhaitables. Il apparaît indispensable de s'interroger sur ce risque et d'étudier la nature des données utilisées et ce qu'elles représentent. |
| T3 | **Evaluer la performance de manière rigoureuse** | Le score de performance d'un modèle prédictif est déterminant pour son adoption dans des produits, systèmes ou processus. L'évaluation de la performance se doit donc d'être rigoureuse. Une spécification de l'équité recherchée entre populations doit également être définie. En effet, l'équité d'un modèle peut [être définie de plusieurs manières qui sont incompatibles entre elles](https://papers.nips.cc/paper/6995-counterfactual-fairness), et l'interprétation de scores de performances doit donc se faire dans le cadre de l'une de ces définitions. |
| T4 | **Etablir et maintenir une généalogie des modèles** | Un modèle prédictif est un objet informatique complexe qui peut évoluer au fil des apprentissages. Tracer les étapes de son élaboration et de son évolution permet d'en constituer une forme de **généalogie**, pré-requis pour **reproduire ou auditer** un modèle. |
| T5 | **Garantir la chaîne de responsabilité des modèles** | Un modèle prédictif peut-être utilisé comme un système automatique, dont les règles de fonctionnement ne sont pas écrites _in extenso_ et ne se prêtent pas ou mal à être explicitées, débattues, ajustées. Des efforts sont nécessaires sur **l'interprétation et l'explication** des choix réalisés à l'aide de ces systèmes. Il apparaît également indispensable de garantir une chaîne de responsabilité claire, de personnes physiques ou morales, pour chaque modèle. |
| T6 | **Anticiper, suivre et minimiser les externalités négatives de l'activité data science** | La mise en place d'un système automatique basé sur un modèle prédictif peut générer des externalités négatives sociales et environnementales. En prendre conscience est indispensable, ainsi qu'anticiper, chercher à suivre et minimiser les différents impacts négatifs. |

## Référentiel de bonnes pratiques définissant la data science responsable et de confiance

- **T1 - Protéger les données personnelles ou confidentielles**

  1. **Gouvernance des données personnelles ou confidentielles** : Dans le cadre des projets de data science, une gouvernance des données personnelles ou confidentielles est mise en place, en organisant le stockage, l'accès, le transfert, la protection, la responsabilité.

  1. **Identification de la législation et des exigences contractuelles applicables** : Toutes les exigences légales, statutaires, réglementaires et contractuelles en vigueur, ainsi que l’approche adoptée par l’organisation pour satisfaire à ces exigences, doivent être explicitement définies, documentées et mises à jour pour chaque traitement de données personnelles ou confidentielles.
  Un processus de veille réglementaire doit être mis en place et documenté.

  1. **Les principales vulnérabilités et attaques de modèles prédictifs** au regard des données confidentielles sont connues, ainsi que les bonnes pratiques et mesures de réduction des risques. Une veille technique est organisée pour tenir à jour ces connaissances. Elles sont prises en compte dans les PIA des traitements de données nécessaires aux projets de data science. Les collaborateurs intervenant sur des projets data science y sont formés régulièrement.

  1. **Les techniques de _privacy enhancement_** (comme par exemple : anonymisation, _differential privacy_, chiffrement homomorphe, etc.) sont prises en compte dans la conception de projets de data science, les choix de les utiliser ou non sont documentés et intégrés à la "généalogie de bout-en-bout" des modèles conçus, entraînés, validés et exploités.

  1. **Les approches limitant l'accès aux données ou le transfert de données** (comme par exemple : _remote execution_, _secure multi-party computation_, etc.) sont prises en compte dans la conception de projets de data science.

- **T2 - Prévenir les biais malencontreux**

  1. Prendre en compte l'origine, la distribution des données d'entraînement, et les phénomènes intempestifs, discriminatoires ou non-souhaitables qui s'y sont glissés du fait de l'époque, du contexte, des processus et outils mis en oeuvre pour les collecter.

  1. Une ou plusieurs mesures de justice et d'équité (_fairness metrics_) sont étudiées et évaluées. Les choix desquelles utiliser sont documentés et intégrés à la "généalogie de bout-en-bout" des modèles.

  1. Les risques de biais discriminatoires sont évalués sur des données de test comprenant différentes sous-populations cibles, et les variables (ou variables proxy) pouvant y conduire sont recherchées.

  1. Les données synthétiques, les approches de _data augmentation_ ou _re-weighting_ doivent être documentés et intégrés à la "généalogie de bout-en-bout" des modèles.

- **T3 - Evaluer la performance de manière rigoureuse**

  1. Les jeux de données utilisés pour le test de la performance d'un modèle doivent être isolés et protégés de manière à ne pas contaminer l'apprentissage.

  1. Prendre en compte l'origine, la distribution des données de test, et les phénomènes intempestifs, discriminatoires ou non-souhaitables qui s'y sont glissés du fait de l'époque, du contexte, des processus et outils mis en oeuvre pour les collecter.

  1. Les bonnes pratiques statistiques de validation rigoureuse de la performance d'un modèle (par exemple définition de la métrique de performance en amont de l'apprentissage), permettant d'éviter l'obtention de score de performance non significatif, doivent être connues et suivies.

  1. Dans les cas de figure d'apprentissage continu, un processus de vérification de la validation d'un modèle à intervalle régulier est mis en place afin d'éviter la dégénérescence d'un modèle.

- **T4 - Etablir et maintenir une généalogie des modèles**

  1. Une "généalogie de bout-en-bout" des modèles est alimentée et tenue à jour dans le cadre des projets de data science, tout au long des phase de collecte de données, conception, entraînement, validation et exploitation.

  1. Les "conditions de validité" ou le "contexte d'utilisation recommandée" d'un modèle conçu, entraîné et validé par l'organisation sont explicités et documentés.

  1. L'utilisation par l'organisation de modèles prédictifs s'effectue dans les conditions et pour les usages pour lesquels les modèles prédictifs en question ont été validés.

- **T5 - Garantir la chaîne de responsabilité des modèles**

  1. La chaîne de responsabilités entre le(s) fournisseur(s) de données, le responsable de la conception du modèle et l'exploitant du modèle est décrite et validée par l'ensemble des parties prenantes.

  1. Une cartographie des modèles existant et de la criticité des processus afférents est mise en place et maintenue.

  1. Une politique de gestion des incidents liés à un modèle est mise en place, comprenant :
      - Le processus d'arrêt de l'utilisation d'un modèle en cas de défaillance constatée.
      - Le mode de fonctionnement des processus impactés en cas de nécessité d'arrêt de l'utilisation d'un modèle.

  1. Un responsable point de contact est défini et identifiable par les exploitants directs et indirects du modèle.

  1. Un processus de suspension ou de restriction de l'utilisation d'un modèle est documenté et mis en place lorsqu'un biais dans les données, le modèle ou l'algorithme est détecté.

- **T6 - Anticiper, suivre et minimiser les externalités négatives de l'activité data science**

  1. Les externalités négatives liées à l'usage d'un modèle prédictif ou d'un système automatique basé dessus doivent être évaluées, prévenues et suivies.

  1. Une formation à l'éthique liée à l'utilisation de modèles est dispensée à l'ensemble des parties prenantes de l'organisation liées à la conception et l'exploitation de modèles.

- **à catégoriser**

  1. Aux frontières de décisions, un classificateur doit avoir une plage de prédiction "indéfinie". Les seuils définissant ces plages doivent être explicités et intégrés à la "généalogie de bout-en-bout" des modèles.

  1. Le "niveau d'interprétabilité" qu'il est possible d'obtenir avec un modèle donné (sur une échelle allant d'une preuve/vérité objective à une simple prédiction sans niveau de confiance) doit être explicités et intégrés aux "conditions de validité" ou au "contexte d'utilisation recommandée" d'un modèle.

## Mesures extraites de [Ethics and Algorithms toolkit](https://ethicstoolkit.ai/) à évaluer

Ethics and Algorithms toolkit est une boite à outils développée par la municipalité de San Francisco et différents organismes publics et privés.
Cette boite à outils est en deux partie :
- Une partie d'évaluation des Risques
- Une liste de mesures pour atténuer les risques en fonction des réponses données lors de la première partie.
Si cette liste de mesures est surtout réalisée dans le cadre de projets "publics" de mise en place d'algorithmes, certaines mesures peuvent être retenues dans un contexte plus général.

- Un Comité de Révision Institutionnelle a été mis en place, en charge :
  - d'examiner et approuver les projets de recherches;
  - valider la mise en oeuvre d'un algorithmes.

- Lorsque le projet a un impact social et public, un conseil consultatif est mis en place, comprenant les parties prenantes du projet ainsi que des représentants du grand public.

- Lorsque le projet a un impact social et public, un dialogue est entretenu avec le grand public à travers différents canaux :
  - Organisation d'enquête auprès du public;
  - Mise en place d'un plan de communication et de l'envoi de mémo / newsletters auprès du public;
  - Organisation de meeting / conférence pour présenter les données et usages utilisés;
  - Ouverture des données utilisées en ligne;
  - Ouverture d'un repo Github.

- Lorsqu'un projet est controversé avant même son démarrage, un moratoire doit être mis en place afin d'indentifier de nouvelles sources de données.

- Des outils de tests automatiques des algorithmes (exemple : matrice de confusion) doivent être mis en place pour évaluer la performance d'un algorithme tout au long de son existance.

- Un mécanisme d'arbitrage humain doit être mis en place s'il permet d'améliorer la performance d'un algorithme.

- Le transfert du suivi de la performance d'un algorithme à un organisme tier permet de retirer un degré de subjectivité.

- Lorsqu'il y a absence de certaines données, ou qu'un échantillon de données est trop petit, des mécanismes de poids sont mis en place pour avoir une meilleure représentation de la population bénéficiaire de l'algorithme.

- Des professionnels de la Data Science et du monde académique peuvent être engagés pour auditer un algorithme.

- Les différentes parties prenantes d'un projet d'algorithme sont capables d'expliquer chaque risque identifié lié au projet de cet algorithme.  

## Mesures extraites de [AI Now Report 2019](https://ainowinstitute.org/AI_Now_2019_Report.pdf) à évaluer

Le Ai Now Report 2019 est rapport réalisé par le AI Now Institut, centre de recherche interdisciplinaires en charge d'évaluer les impacts sociaux de l'Intelligence Artificielle.
Les recommandations présentées sont plutôt d'ordre gouvernementales et en lien avec la réglementation. Certaines idées méritent cependant d'être discutées.   

- Les politiques de diversité mises en place au sein de l'organisation prennent en compte les spécificités de l'Intelligence Artificielle et les risques sur les algorithmes mis en place.

- Les impacts environnementaux des projets de mise en place d'algorithme à grande échelle doivent être publiés auprès du grand public.

- Les collaborateurs, avec ou sans l'aide de leur syndicat, doivent pouvoir contester l'utilisation d'un algorithme intrusif.

- Les collaborateurs partie prenantes de la mise en place d'un algorithme doivent être au courant de la finalité de cette algorithme et décider de contester sa mise en place.

- Le climat, la santé et les déplacements - *déportations* - géographiques doivent être pris en compte dans l'évaluation d'un algorithme.

- Les chercheurs en algorithme doivent être responsables des risques et menaces de leurs algorithmes et doivent mieux documenter les origines de leurs modèles et données utilisées.
