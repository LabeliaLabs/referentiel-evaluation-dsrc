# Data science responsable et de confiance - Référentiel d'évaluation

Le [référentiel d'évaluation](#référentiel-dévaluation-de-la-maturité-dune-organisation) ci-dessous est en cours d'élaboration. Il procède de l'identification des [risques](#risques) que l'on cherche à prévenir dans la pratique responsable et de confiance de la data science. Il est structuré en plusieurs [thèmes](#thèmes-et-canevas-du-référentiel-dévaluation) complémentaires.

## Référentiel d'évaluation de la maturité d'une organisation

L'évaluation est composée des 7 sections suivantes :

- [Section 1 - Protéger les données personnelles ou confidentielles](#section-1---protéger-les-données-personnelles-ou-confidentielles)
- [Section 2 - Prévenir les biais malencontreux](#section-2---prévenir-les-biais-malencontreux)
- [Section 3 - Evaluer la performance de manière rigoureuse](#section-3---evaluer-la-performance-de-manière-rigoureuse)
- [Section 4 - Etablir et maintenir une généalogie des modèles](#section-4---etablir-et-maintenir-une-généalogie-des-modèles)
- [Section 5 - Garantir la chaîne de responsabilité des modèles](#section-5---garantir-la-chaîne-de-responsabilité-des-modèles)
- [Section 6 - Utiliser des modèles prédictifs appris](#section-6---utiliser-des-modèles-prédictifs-appris)
- [Section 7 - Anticiper, suivre et minimiser les externalités de l'activité data science](#section-7---anticiper-suivre-et-minimiser-les-externalités-de-lactivité-data-science)

---

### Section 1 - Protéger les données personnelles ou confidentielles

L'utilisation de données personnelles ou confidentielles fait porter le risque d'exposition de celles-ci, ce qui peut avoir des conséquences très préjudiciables pour les producteurs, gestionnaires, ou sujets de ces données. En particulier dans les projets de data science, elles doivent donc être protégées et les risques qu'elles fuitent ou soient exposées doivent être minimisés.

[_[⇧ retour à la liste des sections](#restructuration-en-un-référentiel-dévaluation-de-la-maturité-dune-organisation)_]  
[_[⇩ prochaine section](#section-2---prévenir-les-biais-malencontreux)_]

---

Q1.1 : **Législation et exigences contractuelles applicables - Identification**  
En ce qui concerne les données personnelles et/ou confidentielles, les exigences légales, statutaires, réglementaires et contractuelles en vigueur et concernant votre organisation sont :

R1.1 :  
_(Type : réponse unique)_  
_(Sélectionner une seule réponse, correspondant le mieux au niveau de maturité de l'organisation sur ce sujet)_

- [ ] 1.1.a Pas encore identifiées
- [ ] 1.1.b Partiellement identifiées ou en cours d'identification
- [ ] 1.1.c Identifiées
- [ ] 1.1.d Identifiées et maîtrisées par les collaborateurs
- [ ] 1.1.e Identifiées, documentées et maîtrisées par les collaborateurs

<details>
<summary>Expl1.1 :</summary>

Mettre en place des processus pour connaître et suivre l'évolution des réglementations applicables (très spécifiques dans certains secteurs), ainsi que pour documenter les approches et choix retenus pour être en conformité à chaque projet de data science. Exemple(s) intéressant(s) : [Welfare surveillance system violates human rights, Dutch court rules](https://www.theguardian.com/technology/2020/feb/05/welfare-surveillance-system-violates-human-rights-dutch-court-rules).

</details>

---

Q1.2 : **Législation et exigences contractuelles applicables - Approche de mise en conformité**  
Pour satisfaire à ces exigences, l’approche adoptée par votre organisation est :

R1.2 :  
_(Type : réponse unique)_  
_(Sélectionner une seule réponse, correspondant le mieux au niveau de maturité de l'organisation sur ce sujet)_

- [ ] 1.2.a Informelle, basée sur la responsabilité et la compétence de chacun
- [ ] 1.2.b Formalisée et accessible à tous les collaborateurs
- [ ] 1.2.c Formalisée et maîtrisée par les collaborateurs
- [ ] 1.2.d Formalisée, maîtrisée par les collaborateurs, documentée pour chaque traitement de données personnelles ou confidentielles

<details>
<summary>Expl1.2 :</summary>

Il s'agit de s'interroger sur la gestion des données personnelles ou confidentielles (stockage, accès, transfert, protection, responsabilités...), et de documenter les choix effectués.

</details>

---

Q1.3 : **Veille réglementaire**  
Un processus de veille réglementaire est-il mis en place, en interne ou via un prestataire spécialisé, pour connaître les évolutions applicables et impactantes pour votre organisation ?

R1.3 :  
_(Type : réponse unique)_  
_(Sélectionner une seule réponse, correspondant le mieux au niveau de maturité de l'organisation sur ce sujet)_

- [ ] 1.3.a Nous ne faisons pas vraiment de veille réglementaire
- [ ] 1.3.b Nous faisons une veille informelle, chaque collaborateur remonte les informations sur un moyen de communication dédiée
- [ ] 1.3.c Nous avons une veille formalisée, les responsables sont identifiés, le processus est documenté

<details>
<summary>Expl1.3 :</summary>

Au-delà de l'identification des réglementations et des approches de mise en conformité, il est important de mettre en place des processus de veille pour connaître et suivre **l'évolution** des réglementations applicables (qui peuvent être très spécifiques dans certains secteurs). Exemple(s) intéressant(s) : [Welfare surveillance system violates human rights, Dutch court rules](https://www.theguardian.com/technology/2020/feb/05/welfare-surveillance-system-violates-human-rights-dutch-court-rules).

</details>

---

Q1.4 : **Législation et exigences contractuelles applicables - Audit et certification**  
La conformité de l'organisation aux exigences relatives aux données personnelles et confidentielles a-t-elle été auditée et est-elle reconnue par une certification, un organisme tiers ou équivalent ?

R1.4 :  
_(Type : réponse unique)_  
_(Sélectionner une seule réponse, correspondant le mieux au niveau de maturité de l'organisation sur ce sujet)_

- [ ] 1.4.a Oui
- [ ] 1.4.b Non

<details>
<summary>Expl1.4 :</summary>

Dans de nombreux secteurs il existe des exigences de conformité spécifiques. Il est généralement possible de formaliser la conformité d'une organisation par une certification ou un audit spécialisé, l'obtention d'un label.

</details>

---

Q1.5 : **Principe de minimisation**  
Dans le cadre des projets de data science, le principe de minimisation doit guider la collecte et l'utilisation de données personnelles ou confidentielles. Comment est-il mis en oeuvre au sein de votre organisation ?

R1.5 :  
_(Type : réponse unique)_  
_(Sélectionner une seule réponse, correspondant le mieux au niveau de maturité de l'organisation sur ce sujet)_

- [ ] 1.5.a Nous faisons en sorte de n'utiliser aucune données personnelles ou confidentielles. Nous ne sommes pas concernés par cet univers de risque
- [ ] 1.5.b Nous avons besoin d'en utiliser dans certains projets et le principe de minimisation est alors systématiquement appliqué
- [ ] 1.5.c Le principe de minimisation est connu des collaborateurs, qui l'appliquent en général
- [ ] 1.5.d Le réflexe "qui peut le plus peut le moins" vis-à-vis des données existe encore ici et là au sein de notre organisation. Dans certains projets, nous conservons des jeux de données beaucoup plus riches en données personnelles et confidentielles que ce qui est strictement utile au projet
  
---

_Les éléments suivants au sein de cette section ne s'appliquent qu'aux organisations n'ayant pas sélectionné la première réponse de R1.5. Les organisations non concernées sont donc invitées à passer à la [Section 2](#section-2-prévenir-les-biais-malencontreux)._

---

Q1.6 : **Projet impliquant un nouveau traitement de données personnelles ou confidentielles**  
_(Condition : R1.5 <> 1ère réponse)_  
Pour chaque traitement de données personnelles ou confidentielles nécessaire dans le cadre d'un projet de data science, au sein de votre organisation :

R1.6 :  
_(Type : réponses multiples possibles)_  
_(Sélectionner tous les éléments de réponse correspondant à des pratiques de votre organisation)_

- [ ] 1.6.a Nous élaborons un _Privacy Impact Assessment_ (PIA)
- [ ] 1.6.b Nous mettons en oeuvre des mesures de protections (concernant notamment le transfert, le stockage, et l'accès aux données concernées)
- [ ] 1.6.c Nous documentons les PIA et mesures mises en oeuvre et nous les conservons au sein des projets
- [ ] 1.6.d Nous contractualisons les relations avec les fournisseurs et les clients et les responsabilités qui en découlent

---

Q1.7 : **Sécurité de l'apprentissage automatique et _PETs_ - Niveau de connaissance**  
_(Condition : R1.5 <> 1ère réponse)_  
La sécurité de l'apprentissage automatique (_ML security_) est un domaine en plein développement. Dans certains cas de figure, les modèles prédictifs appris sur des données confidentielles peuvent révéler des éléments de ces données confidentielles. Au sein de votre organisation, au sujet des vulnérabilités liées aux modèles de ML et aux _Privacy Enhancing Technologies (PETs)_, le niveau de connaissance générale des collaborateurs intervenant sur les projets de data science est :

R1.7 :  
_(Type : réponse unique)_  
_(Sélectionner une seule réponse, correspondant le mieux au niveau de maturité de l'organisation sur ce sujet)_

- [ ] 1.7.a Débutant
- [ ] 1.7.b Intermédiaire
- [ ] 1.7.c Confirmé
- [ ] 1.7.d Expert

<details>
<summary>Expl1.7 :</summary>

L'état de l'art de la sécurité du ML est en constante évolution. S'il est impossible de se prémunir contre toutes les vulnérabilités à tout instant, il est crucial de s'en préoccuper et se tenir au courant. Le [OWASP Top Five ML risks](https://github.com/OWASP/Top-5-Machine-Learning-Risks/blob/master/Top%205%20Machine%20Learning%20Risks.md) est par exemple un point d'entrée intéressant.

</details>

<details>
<summary>Ressources1.7 :</summary>

- (Web article) *[Top Five ML risks](https://github.com/OWASP/Top-5-Machine-Learning-Risks/blob/master/Top%205%20Machine%20Learning%20Risks.md)*, OWASP
- (Web article) *[The secret-sharer: evaluating and testing unintended memorization in neural networks](https://blog.acolyer.org/2019/09/23/the-secret-sharer/)*, A. Colyer, 2019
- (Academic paper) *[Membership Inference Attacks against Machine Learning Models](https://arxiv.org/abs/1610.05820)*, R. Shokri, M. Stronati, C. Song, V. Shmatikov, 2017
- (Tool) *[ML Privacy Meter](https://github.com/privacytrustlab/ml_privacy_meter): a tool to quantify the privacy risks of machine learning models with respect to inference attacks*
- (Web article) *[Demystifying the membership inference attack](https://medium.com/disaitek/demystifying-the-membership-inference-attack-e33e510a0c39)*, Disaitek, 2019
- (Academic paper) *[Inverting Gradients - How easy is it to break privacy in federated learning?](https://arxiv.org/abs/2003.14053)*, J. Geiping, H. Bauermeister, H. Dröge, M. Moeller, 2020
- (Software) Outils pour la *differential privacy* : Google *[differential privacy library](https://github.com/google/differential-privacy)*, et le wrapper Python [PyDP](https://github.com/OpenMined/PyDP) d'OpenMined
- (Web article) La *distillation* d'un modèle, en plus de la compression qu'elle apporte, peut être utilisée comme une mesure de protection du modèle et des données d'entraînement utilisées, voir par exemple *[Knowledge Distillation : Simplified](https://towardsdatascience.com/knowledge-distillation-simplified-dd4973dbc764)*, Towards Data Science, 2019
- (Academic paper) *[Distilling the Knowledge in a Neural Network](https://arxiv.org/abs/1503.02531)*, G. Hinton, O. Vinyals, J. Dean, 2015

</details>

---

Q1.8 : **Sécurité de l'apprentissage automatique et _PETs_ - Mise en oeuvre**  
_(Condition : R1.5 <> 1ère réponse)_  
Toujours au sujet des vulnérabilités liées aux modèles de ML et aux _PETs_ :

R1.8 :  
_(Type : réponses multiples possibles)_  
_(Sélectionner tous les éléments de réponse correspondant à des pratiques de votre organisation)_

- [ ] 1.8.a Une veille technique est mise en oeuvre
- [ ] 1.8.b Les collaborateurs reçoivent régulièrement des informations / formations qui leur permettent de monter en compétences
- [ ] 1.8.c Dans certains projets, nous mettons en oeuvre des _PETs_ permettant de réduire les risques liés aux modèles que nous élaborons
- [ ] 1.8.d Sur chaque projet, les vulnérabilités qui s'y appliquent et les _PETs_ mises en oeuvre sont documentées dans la généalogie de bout-en-bout de chaque modèle

<details>
<summary>Expl1.8 :</summary>

L'état de l'art de la sécurité du ML est en constante évolution. S'il est impossible de se prémunir contre toutes les vulnérabilités à tout instant, il est crucial de s'en préoccuper et d'organiser une veille. Le [OWASP Top Five ML risks](https://github.com/OWASP/Top-5-Machine-Learning-Risks/blob/master/Top%205%20Machine%20Learning%20Risks.md) est par exemple un point d'entrée intéressant.

Selon les niveaux de risque et de sensibilité des projets, certaines approches *PETs* seront sélectionnées et implémentées. Il est important de suivre l'évolution de l'état de l'art et des pratiques, et de documenter les choix réalisés. On introduit ici la notion de "généalogie de bout-en-bout".

</details>

<details>
<summary>Ressources1.8 :</summary>

- (Web article) *[Top Five ML risks](https://github.com/OWASP/Top-5-Machine-Learning-Risks/blob/master/Top%205%20Machine%20Learning%20Risks.md)*, OWASP
- (Web article) *[The secret-sharer: evaluating and testing unintended memorization in neural networks](https://blog.acolyer.org/2019/09/23/the-secret-sharer/)*, A. Colyer, 2019
- (Academic paper) *[Membership Inference Attacks against Machine Learning Models](https://arxiv.org/abs/1610.05820)*, R. Shokri, M. Stronati, C. Song, V. Shmatikov, 2017
- (Tool) *[ML Privacy Meter](https://github.com/privacytrustlab/ml_privacy_meter): a tool to quantify the privacy risks of machine learning models with respect to inference attacks*
- (Web article) *[Demystifying the membership inference attack](https://medium.com/disaitek/demystifying-the-membership-inference-attack-e33e510a0c39)*, Disaitek, 2019
- (Academic paper) *[Inverting Gradients - How easy is it to break privacy in federated learning?](https://arxiv.org/abs/2003.14053)*, J. Geiping, H. Bauermeister, H. Dröge, M. Moeller, 2020
- (Software) Outils pour la *differential privacy* : Google *[differential privacy library](https://github.com/google/differential-privacy)*, et le wrapper Python [PyDP](https://github.com/OpenMined/PyDP) d'OpenMined
- (Web article) La *distillation* d'un modèle, en plus de la compression qu'elle apporte, peut être utilisée comme une mesure de protection du modèle et des données d'entraînement utilisées, voir par exemple *[Knowledge Distillation : Simplified](https://towardsdatascience.com/knowledge-distillation-simplified-dd4973dbc764)*, Towards Data Science, 2019
- (Academic paper) *[Distilling the Knowledge in a Neural Network](https://arxiv.org/abs/1503.02531)*, G. Hinton, O. Vinyals, J. Dean, 2015

</details>

---

Q1.9 : **Notifications d’incidents de sécurité aux autorités de régulation**  
_(Condition : R1.5 <> 1ère réponse)_  
Dans le cas de figure où un modèle que l'organisation a élaboré est utilisé ou accessible par une(des) partie(s) prenante(s) externe(s), et qu'une vulnérabilité nouvelle est publiée, présente un risque de s'y appliquer et crée ainsi un risque d'exposition de données personnelles ou confidentielles :

R1.9 :  
_(Type : réponses multiples possibles)_  
_(Sélectionner tous les éléments de réponse correspondant à des pratiques de votre organisation)_

- [ ] 1.9.a Nous avons une procédure décrivant la marche à suivre
- [ ] 1.9.b Notre procédure inclut une communication aux parties prenantes en question
- [ ] 1.9.c Notre procédure référence les autorités auxquelles nous devons faire un signalement

<details>
<summary>Expl1.9 :</summary>

Il existe dans certains secteurs des obligations de signalement des incidents de sécurité aux autorités de régulation (e.g. CNIL, ANSSI, ARS...). Un point d'entrée intéressant : [Notifications d’incidents de sécurité aux autorités de régulation : comment s’organiser et à qui s’adresser ?](https://www.cnil.fr/fr/notifications-dincidents-de-securite-aux-autorites-de-regulation-comment-sorganiser-et-qui-sadresser) sur le site de la CNIL.

</details>

---
---

### Section 2 - Prévenir les biais malencontreux

L'utilisation de modèles prédictifs élaborés à partir de données historiques peut se révéler contre-productive lorsque les données historiques sont contaminées par des phénomènes problématiques (e.g. qualité de certains points de données, données non comparables, phénomène social non souhaitable du fait de l'époque...). Il apparaît indispensable de s'interroger sur ce risque et d'étudier la nature des données utilisées, les conditions dans lesquelles elles ont été produites et assembées, et ce qu'elles représentent.
Dans certains cas, une spécification de l'équité recherchée entre populations doit également être définie. L'équité d'un modèle peut [être définie de plusieurs manières qui peuvent être incompatibles entre elles](https://papers.nips.cc/paper/6995-counterfactual-fairness), et l'interprétation de scores de performances doit donc se faire dans le cadre de l'une de ces définitions.

[_[⇧ retour à la liste des sections](#restructuration-en-un-référentiel-dévaluation-de-la-maturité-dune-organisation)_]  
[_[⇩ prochaine section](#section-3---evaluer-la-performance-de-manière-rigoureuse)_]

---

Q2.1 : **Analyse des données d'entraînement utilisées**  
Au sein des projets de data science et lors de l'élaboration de jeux de données d'entraînement, un travail de réflexion et recherche de phénomènes intempestifs ou parasites du fait de l'époque, du contexte, des outils ou processus d'enregistrement peut s'avérer crucial pour prévenir des biais malencontreux. Votre organisation :

R2.1 :  
_(Type : réponse unique)_  
_(Sélectionner une seule réponse, correspondant le mieux au niveau de maturité de l'organisation sur ce sujet)_

- [ ] 2.1.a Fonctionne de manière informelle à ce sujet et s'appuie sur la compétence et la responsabilité des collaborateurs impliquées
- [ ] 2.1.b Dispose d'une approche documentée et systématiquement mise en oeuvre

<details>
<summary>Expl2.1 :</summary>

Il s'agit de s'obliger à s'interroger sur ces sujets et donc à réfléchir aux données utilisées, la manière dont elles ont été produites etc.

</details>

<details>
<summary>Ressources2.1 :</summary>

- (Technical guide) *[Tour of Data Sampling Methods for Imbalanced Classification](https://machinelearningmastery.com/data-sampling-methods-for-imbalanced-classification/)*
- (Web article) *[Hidden Bias](https://pair.withgoogle.com/explorables/hidden-bias/)* explorable from [PAIR](https://pair.withgoogle.com/)

</details>

---

Q2.2 : **Risques de discrimination à l'encontre de certains groupes sociaux**  
Votre organisation est-elle concernée par des cas de figure où des modèles prédictifs sont utilisés dans des environnements thématiques pour lesquels des risques de discrimination à l'encontre de certains groupes sociaux (genre, origine, âge, etc.) existent ?

R2.2 :  
_(Type : réponse unique)_  
_(Sélectionner une seule réponse, correspondant le mieux au niveau de maturité de l'organisation sur ce sujet)_

- [ ] 2.2.a Concerné
- [ ] 2.2.b Non concerné

---

_Les éléments suivants au sein de cette section ne s'appliquent qu'aux organisations ayant sélectionné la réponse "Concerné" de R2.2. Les organisations non concernées sont donc invitées à passer à la [Section 3](#section-3-evaluer-la-performance-de-manière-rigoureuse)._

---

Q2.3 : **Prévention des biais discriminatoires**  
_(Condition : R2.2 = Concerné)_  
Dans les cas de figure où les modèles prédictifs que votre organisation élabore sont utilisés dans des environnements thématiques où il y a des risques de discrimination à l'encontre de certains groupes sociaux (genre, origine, âge, etc.) :

R2.3 :  
_(Type : réponses multiples possibles)_  
_(Sélectionner tous les éléments de réponse correspondant à des pratiques de votre organisation)_

- [ ] 2.3.a Nous portons une attention particulière à l'identification de variables protégées et à leurs proxys éventuels
- [ ] 2.3.b Nous procédons à des évaluations sur des données de test comprenant différentes sous-populations afin d'identifier les éventuels biais problématiques
- [ ] 2.3.c Nous sélectionnons et mettons en oeuvre une ou plusieurs mesure(s) de justice et d'équité (_fairness metric_)
- [ ] 2.3.d Nous mettons en oeuvre des approches de type _data augmentation_ ou _re-weighting_
- [ ] 2.3.e Les pratiques ci-dessus que nous mettons en oeuvre sont dûment documentées intégrées à la généalogie de bout-en-bout des modèles concernés

<details>
<summary>Expl2.3 :</summary>

Il s'agit de s'interroger systématiquement, à chaque projet de data science et selon l'objectif et l'usage cible du modèle que l'on veut élaborer, sur les features pouvant directement ou indirectement être à l'origine d'un risque de biais discriminatoire.
Complément sur l'utilisation de données synthétiques et d'approches de _data augmentation_, _re-weighting_ : lorsque de telles techniques sont utilisées il est important de les expliciter, au risque sinon de perdre de l'information sur la manière dont un modèle a été élaboré.

</details>

<details>
<summary>Ressources2.3 :</summary>

- (Web article) *[Measuring fairness](https://pair.withgoogle.com/explorables/measuring-fairness)* explorable, [PAIR](https://pair.withgoogle.com/)
- (Software) *[AI Fairness 360](https://developer.ibm.com/technologies/artificial-intelligence/projects/ai-fairness-360/): an open source software toolkit that can help detect and remove bias in machine learning models*, IBM
- (Academic paper) *Fairness metrics* : *[counterfactual fairness](https://papers.nips.cc/paper/6995-counterfactual-fairness)*
- (Academic paper) *Fairness metrics* : *[adversarial debiaising](https://arxiv.org/pdf/1801.07593.pdf)*

</details>

---
---

### Section 3 - Evaluer la performance de manière rigoureuse

Le score de performance d'un modèle prédictif est déterminant pour son adoption dans des produits, systèmes ou processus. L'évaluation de la performance se doit donc d'être rigoureuse. Par ailleurs un modèle prédictif peut-être utilisé comme un système automatique, dont les règles de fonctionnement ne sont pas écrites _in extenso_ et ne se prêtent pas ou mal à être explicitées, débattues, ajustées. Des efforts sont donc nécessaires sur l'interprétation et l'explication des choix réalisés à l'aide de ces systèmes.

[_[⇧ retour à la liste des sections](#restructuration-en-un-référentiel-dévaluation-de-la-maturité-dune-organisation)_]  
[_[⇩ prochaine section](#section-4---etablir-et-maintenir-une-généalogie-des-modèles)_]

---

Q3.1 : **Séparation des jeux de données de test**  
Au sein des projets de data science et lors de l'élaboration de jeux de données de test, il est capital d'assurer la non-contamination par des données d'entraînement. Votre organisation :

R3.1 :  
_(Type : combiné)_  
_(Sélectionner tous les éléments de réponse correspondant à des pratiques de votre organisation. Attention, certaines combinaisons ne seraient pas cohérentes)_

- [ ] 3.1.a Fonctionne de manière informelle à ce sujet et s'appuie sur la compétence et la responsabilité des collaborateurs impliquées
- [ ] 3.1.b Dispose d'une approche documentée et systématiquement mise en oeuvre d'isolation des testsets
- [ ] 3.1.c Utilise un outil de versionnage et de traçabilité des jeux de données d'entraînement et de test utilisés, permettant ainsi de vérifier ou auditer ultérieurement la non-contamination des données de tests
- [ ] 3.1.d Prévoit systématiquement l'élaboration de deux testsets ou plus pour gagner en résilience

---

Q3.2 : **Projets d'apprentissage distribué préservant la confidentialité**  
Dans les cas de figure de projets de data science basé sur l'apprentissage distribué ou fédéré (_distributed learning_ ou _federated learning_) sur des jeux de données multiples et dont la confidentialité doit être préservée vis-à-vis des autres (_privacy-preserving_) :

R3.2 :  
_(Type : réponse unique)_  
_(Sélectionner une seule réponse, correspondant le mieux au niveau de maturité de l'organisation sur ce sujet)_

- [ ] 3.2.a Nous ne participons pas à des projets de _privacy-preserving distributed learning_ | _(Lorsque cette réponse est sélectionnée, les autres ne peuvent pas l'être)_
- [ ] 3.2.b Nous maîtrisons et mettons en oeuvre des approches permettant d'élaborer des jeux de données de test de manière à ce qu'il n'y ait pas de contamination croisée entre données d'entraînement et de test provenant des différents partenaires
- [ ] 3.2.c À ce stade nous ne maîtrisons pas les méthodes permettant d'élaborer des jeux de données de test de manière à ce qu'il n'y ait pas de contamination croisée entre données d'entraînement et de test provenant des différents partenaires

---

Q3.3 : **Analyse des données de test**  
Au sein des projets de data science et lors de l'élaboration de jeux de données de test, un travail de réflexion et recherche de phénomènes intempestifs ou parasites du fait de l'époque, du contexte, des outils ou processus d'enregistrement peut s'avérer crucial pour la signification des scores de performance. Votre organisation :

R3.3 :  
_(Type : réponse unique)_  
_(Sélectionner une seule réponse, correspondant le mieux au niveau de maturité de l'organisation sur ce sujet)_

- [ ] 3.3.a Fonctionne de manière informelle à ce sujet et s'appuie sur la compétence et la responsabilité des collaborateurs impliquées
- [ ] 3.3.b Dispose d'une approche documentée et systématiquement mise en oeuvre

<details>
<summary>Expl3.3 :</summary>

L'utilisation de modèles prédictifs testés sur des données historiques peut se révéler contre-productive lorsque les données historiques en question sont contaminées par des phénomènes problématiques (e.g. qualité de certains points de données, données non comparables, phénomène social non souhaitable du fait de l'époque...). Il apparaît indispensable de s'interroger sur ce risque et d'étudier la nature des données utilisées, les conditions dans lesquelles elles ont été produites et assemblées, et ce qu'elles représentent.

</details>

---

Q3.4 : **Validation des performances**  
Votre organisation met-elle en oeuvre les approches suivantes :

R3.4 :  
_(Type : réponses multiples possibles)_  
_(Sélectionner tous les éléments de réponse correspondant à des pratiques de votre organisation)_

- [ ] 3.4.a Lors de l'élaboration d'un modèle, nous choisissons la ou les métrique(s) de performance en amont de l'apprentissage automatique, parmi les métriques les plus standards possibles
- [ ] 3.4.b La mise en oeuvre de mesures de robustesse (*robustness metrics*) est considérée et évaluée pour chaque projet d'élaboration d'un modèle, et appliquée par défaut dans les cas de figure où les données d'entrées peuvent être soumises à des perturbations fines (e.g. images, sons)
- [ ] 3.4.c Les pratiques ci-dessus que nous mettons en oeuvre sont dûment documentées intégrées à la généalogie de bout-en-bout des modèles concernés, y compris les métriques de performance choisies

<details>
<summary>Expl3.4 :</summary>

Voir par exemple le *[p-hacking / data dredging](https://fr.wikipedia.org/wiki/Data_dredging)*.

</details>

<details>
<summary>Ressources3.4 :</summary>

- (Academic paper) *Robustness metrics* : *[noise sensitivity score](https://arxiv.org/abs/1806.01477)*.

</details>

---

Q3.5 : **Suivi de la performance dans le temps**  
Dans les cas de figure où des modèles prédictifs élaborés par votre organisation sont utilisés dans des systèmes en production :

R3.5 :  
_(Type : combiné)_  
_(Sélectionner tous les éléments de réponse correspondant à des pratiques de votre organisation. Attention, certaines combinaisons ne seraient pas cohérentes)_

- [ ] 3.5.a Les modèles que nous élaborons ne sont pas utilisés actuellement | _(Lorsque cette réponse est sélectionnée, les autres ne peuvent pas l'être)_
- [ ] 3.5.b La performance est systématiquement ré-évaluée lorsque le modèle est mis à jour
- [ ] 3.5.c La performance est systématiquement ré-évaluée lorsque le contexte d'utilisation du modèle évolue, ce qui peut créer un risque sur la performance du modèle du fait de l'évolution de l'espace des données d'entrée
- [ ] 3.5.d La distribution des données d'entrée est monitorée, et la performance est ré-évaluée régulièrement sur des données de test actualisées
- [ ] 3.5.e Des contrôles aléatoires sont réalisés sur des prédictions afin d'en contrôler la cohérence

<details>
<summary>Expl3.5 :</summary>

Même sur un modèle stable il existe un risque que les données d'entrée ne soient plus dans le domaine au bout d'un certain temps (population & distribution), exemple : une variable qui ne serait plus renseignée à la même fréquence qu'avant par les utilisateurs dans un SI. Il est donc nécessaire de contrôler régulièrement la performance d'un modèle utilisé dans son contexte d'utilisation.

</details>

<details>
<summary>Ressources3.5 :</summary>

- (Technical guide) *[Continuous delivery for machine learning](https://martinfowler.com/articles/cd4ml.html)*, D. Sato, A. Wider, C. Windheuser, Septembre 2019
- (Technical guide) *[Monitoring Machine Learning Models in Production - A comprehensive guide](https://christophergs.com/machine%20learning/2020/03/14/how-to-monitor-machine-learning-models/)*, ChristopherGS, Mars 2020
- (Web article) *[Google’s medical AI was super accurate in a lab. Real life was a different story](https://www.technologyreview.com/2020/04/27/1000658/google-medical-ai-accurate-lab-real-life-clinic-covid-diabetes-retina-disease/)*, MIT Technology Review

</details>

---

Q3.6 : **Seuils de décision et plages d'indécision**  
Lors de l'élaboration d'un modèle de classification, pour la définition des seuils de décision, votre organisation :

R3.6 :  
_(Type : combiné)_  
_(Sélectionner tous les éléments de réponse correspondant à des pratiques de votre organisation. Attention, certaines combinaisons ne seraient pas cohérentes)_

- [ ] 3.6.a Fonctionne de manière informelle à ce sujet et s'appuie sur la compétence et la responsabilité des collaborateurs impliquées
- [ ] 3.6.b Dispose d'une approche documentée et systématiquement mise en oeuvre
- [ ] 3.6.c Dispose d'une approche documentée et systématiquement mise en oeuvre, qui inclut la possibilité de maintenir des plages d'indécision
- [ ] 3.6.d Les choix réalisés pour chaque modèle et mis en oeuvre sont dûment documentées intégrées à la généalogie de bout-en-bout des modèles concernés

<details>
<summary>Ressources3.6 :</summary>

- (Web article) *[Opening the algorithm’s black box and understand its outputs](https://medium.com/@asaboni/opening-the-algorithms-black-box-and-understand-its-outputs-e2363b0a887c)*, A. Saboni (Octo Technologies), April 2020

</details>

---

Q3.7 : **Explicabilité et interprétabilité**  
Au sein des projets de data science qui visent à élaborer des modèles prédictifs :

R3.7 :  
_(Type : combiné)_  
_(Sélectionner tous les éléments de réponse correspondant à des pratiques de votre organisation. Attention, certaines combinaisons ne seraient pas cohérentes)_

- [ ] 3.7.a Notre organisation n'est pour l'instant pas familière avec les méthodes et outils d'explicabilité et d'interprétabilité des modèles
- [ ] 3.7.b Nous nous intéressons au sujet de l'explicabilité et l'interprétabilité des modèles et dialoguons avec nos parties prenantes sur ce sujet
- [ ] 3.7.c Nous faisons en sorte que les modèles que nous élaborons fournissent lorsque cela est pertinent a minima un niveau de confiance avec chaque prédiction réalisée
- [ ] 3.7.d Nous déterminons le meilleur compromis entre la performance et l'interprétabilité pour chaque modèle que nous élaborons, ce qui nous amène parfois à opter pour un modèle plus simple à expliquer aux personnes concernées (un modèle performant permettra de diminuer les risques d’erreur tandis qu’un modèle interprétable permettra de mieux justifier les résultats du modèle)
- [ ] 3.7.e Nous maîtrisons et mettons en oeuvre des approches avancées pour l'explicabilité et l'interprétabilité des modèles

<details>
<summary>Ressources3.7 :</summary>

- (Web article) *[La confiance des utilisateurs dans les systèmes impliquant de l’Intelligence Artificielle](https://blog.octo.com/la-confiance-des-utilisateurs-dans-les-systemes-impliquant-de-lintelligence-artificielle/)*, Blog Octo Technologies, octobre 2019
- (Technical guide) *[Interpretable Machine Learning, A Guide for Making Black Box Models Explainable](https://christophm.github.io/interpretable-ml-book/)*, Christoph Molnar
- (Web article) Dans certains cas la réglementation impose de pouvoir expliquer aux personnes concernées comment fonctionne un algorithme (voir par exemple [l'article 22 du RGPD](https://www.cnil.fr/fr/reglement-europeen-protection-donnees/chapitre3#Article22), [l'article 10 de la loi Informatique et libertés](https://www.legifrance.gouv.fr/affichTexteArticle.do;?idArticle=LEGIARTI000037090394&cidTexte=LEGITEXT000006068624&dateTexte=20180624), cités notamment dans le [Serment d'Hippocrate pour data scientist](https://hippocrate.tech/))

</details>

---
---

### Section 4 - Etablir et maintenir une généalogie des modèles

Un modèle prédictif est un objet informatique complexe qui peut évoluer au fil des apprentissages. Tracer les étapes de son élaboration et de son évolution permet d'en constituer une forme de **généalogie**, pré-requis pour **reproduire ou auditer** un modèle.

[_[⇧ retour à la liste des sections](#restructuration-en-un-référentiel-dévaluation-de-la-maturité-dune-organisation)_]  
[_[⇩ prochaine section](#section-5---garantir-la-chaîne-de-responsabilité-des-modèles)_]

---

Q4.1 : **"Généalogie de bout-en-bout" des modèles**  
Tracer les étapes de l'élaboration d'un modèle permet d'en constituer une forme de **généalogie**. Au sein de votre organisation, une généalogie de bout-en-bout des modèles est alimentée et tenue à jour dans le cadre des projets de data science, tout au long des phase de collecte de données, conception, entraînement, validation et exploitation des modèles :

R4.1 :  
_(Type : réponse unique)_  
_(Sélectionner une seule réponse, correspondant le mieux au niveau de maturité de l'organisation sur ce sujet)_

- [ ] 4.1.a À ce stade nous n'avons pas mis en oeuvre d'approche de ce type
- [ ] 4.1.b Ces informations existent et sont enregistrées afin de ne pas être perdues, mais elles peuvent l'être de manière désordonnée et ne sont pas versionnées
- [ ] 4.1.c Elles sont rassemblées en un unique document qui accompagne systématiquement le modèle
- [ ] 4.1.d Elles sont rassemblées en un unique document qui accompagne systématiquement le modèle et versionnées

<details>
<summary>Expl4.1 :</summary>

Ce concept de "généalogie de bout-en-bout" d'un modèle prédictif appris peut se décliner sous la forme par exemple d'un document de référence reprenant tous les choix importants ainsi que tout l'historique d'élaboration du modèle (données utilisées, pré-traitements réalisés, type d'apprentissage et architecture du modèle, seuils de décision, métriques de tests, compromis réalisés et leurs modalités (par exemple entre performance et privacy ou coût computationnel), etc.), et de processus internes organisant cette activité.

</details>

<details>
<summary>Ressources4.1 :</summary>

- (Software) [Substra Framework](http://doc.substra.ai/): *an open source framework offering distributed orchestration of machine learning tasks among partners while guaranteeing secure and trustless traceability of all operations*
- (Software) [MLflow](https://mlflow.org/): *an open source platform to manage the ML lifecycle, including experimentation, reproducibility, deployment, and a central model registry*
- (Software) [DVC](https://dvc.org/): *an Open-source Version Control System for Machine Learning Projects*
- (Tool) [DAGsHub](https://dagshub.com/docs/): *a platform for data version control and collaboration, based on DVC*

</details>

---

Q4.2 : **Conditions et limites d'utilisation d'un modèle**  
Dans le cadre des projets de data science, les "conditions et limites de validité" d'un modèle conçu, entraîné et validé par l'organisation :

R4.2 :  
_(Type : combiné)_  
_(Sélectionner tous les éléments de réponse correspondant à des pratiques de votre organisation. Attention, certaines combinaisons ne seraient pas cohérentes)_

- [ ] 4.2.a Ne sont pas documentées | _(Lorsque cette réponse est sélectionnée, les autres ne peuvent pas l'être)_
- [ ] 4.2.b Sont explicitées et documentées
- [ ] 4.2.c Sont versionnées
- [ ] 4.2.d Contiennent une description des risques que présenterait une utilisation en dehors des "conditions et limités de validité"
- [ ] 4.2.e Les documents présentant ces "conditions et limites de validité" accompagnent systématiquement les modèles tout au long de leur cycle de vie

<details>
<summary>Expl4.2 :</summary>

Il s'agit d'expliciter et d'adjoindre au modèle la description du contexte d'utilisation pour lequel il a été conçu et dans lequel sa performance annoncée est significative. Ce concept de "conditions et limites de validité" peut se décliner sous la forme d'un document synthétique ou d'une section spécifique dans la "généalogie de bout-en-bout".

</details>

<details>
<summary>Ressources4.2 :</summary>

- (Web article) [Model Cards](https://modelcards.withgoogle.com/about) de Google est un framework ouvert et évolutif, et propose 2 exemples : *To explore the possibilities of model cards in the real world, we've designed examples for two features of our Cloud Vision API, Face Detection and Object Detection. They provide simple overviews of both models' ideal forms of input, visualize some of their key limitations, and present basic performance metrics.*

</details>

---
---

### Section 5 - Garantir la chaîne de responsabilité des modèles

Utiliser des systèmes automatiques basés sur des modèles dont les règles ont été "apprises" (et non définies et formalisées) interroge le fonctionnement des organisations. Il apparaît indispensable de garantir une chaîne de responsabilité claire, de personnes physiques ou morales, pour chaque modèle.

[_[⇧ retour à la liste des sections](#restructuration-en-un-référentiel-dévaluation-de-la-maturité-dune-organisation)_]  
[_[⇩ prochaine section](#section-6---utiliser-des-modèles-prédictifs-appris)_]

---

Q5.1 : **Chaîne de valeur et de responsabilités**  
Dans le cas de figure des projets de data science où plusieurs acteurs, y compris internes à l'organisation (équipes, départements, filiales), sont parties prenantes tout au long de la chaîne de valeur et de responsabilités :

R5.1 :  
_(Type : combiné)_  
_(Sélectionner tous les éléments de réponse correspondant à des pratiques de votre organisation. Attention, certaines combinaisons ne seraient pas cohérentes)_

- [ ] 5.1.a Au sein de notre organisation les projets de data science sont menés de bout-en-bout par des équipes autonomes, y compris l'élaboration de jeux de données et l'exploitation pour son propre compte des modèles. En conséquence, pour chaque projet une équipe autonome est seule responsable | _(Lorsque cette réponse est sélectionnée, les autres ne peuvent pas l'être)_
- [ ] 5.1.b Nous procédons systématiquement à l'identification des risques et responsabilités de chacune des parties prenantes internes ou externes avec lesquelles nous collaborons
- [ ] 5.1.c Nous contractualisons systématiquement avec les acteurs amont (e.g. fournisseurs de données) et aval (e.g. clients, partenaires utilisateurs de modèles)

<details>
<summary>Expl5.1 :</summary>

Il est important de s'assurer que les organisations en amont et en aval de la chaîne identifient et endossent bien leurs responsabilités sur leurs segments de la chaîne de valeur.

</details>

---

Q5.2 : **Répartition de la création de valeur**  
Dans les cas de figure des projets de data science où plusieurs partenaires concourent aux côtés de votre organisation à l'élaboration d'un modèle, et que celui-ci est ou sera l'objet d'une activité économique :

R5.2 :  
_(Type : combiné)_  
_(Sélectionner tous les éléments de réponse correspondant à des pratiques de votre organisation. Attention, certaines combinaisons ne seraient pas cohérentes)_

- [ ] 5.2.a Notre organisation exerce ses activités de data science de manière autonome, y compris l'élaboration de jeux de données et l'exploitation pour son propre compte des modèles. Elle n'est donc pas concernée  | _(Lorsque cette réponse est sélectionnée, les autres ne peuvent pas l'être)_
- [ ] 5.2.b À ce stade nous n'avons pas structuré cet aspect des projets de data science multi-partenaires | _(Lorsque cette réponse est sélectionnée, les autres ne peuvent pas l'être)_
- [ ] 5.2.c Dans ces cas de figure nous contractualisons le volet économique de la relation avec les parties prenantes impliquées en amont du projet
- [ ] 5.2.d Notre organisation s'est dotée d'une politique encadrant de manière responsable le partage de valeur avec les parties prenantes impliquées

<details>
<summary>Expl5.2 :</summary>

Lorsque plusieurs partenaires collaborent pour l'élaboration d'un modèle, il est important que la répartition de valeur consécutives à une activité économique dans laquelle le modèle joue un rôle soit explicitée et contractualisée. Dans certains cas de figure cette question peut être complexe, par exemple lorsqu'un modèle est entraîné de manière distribuée sur plusieurs jeux de données.

</details>

<details>
<summary>Ressource5.2 :</summary>

- (Code repository) [Exploration of dataset contributivity to a model in collaborative ML projects](https://github.com/SubstraFoundation/distributed-learning-contributivity), un projet open source animé par Substra Foundation

</details>

---

Q5.3 : **Sous-traitance de tout ou partie des activités data science**  
Les activités data science sous-traitées à une ou des organisation(s) tierce(s) sont soumises aux mêmes exigences que celles que votre organisation s'applique à elle-même :

R5.3 :  
_(Type : combiné)_  
_(Sélectionner une seule réponse, correspondant le mieux au niveau de maturité de l'organisation sur ce sujet)_

- [ ] 5.3.a Non concerné, nous ne sous-traitons pas ces activités | _(Lorsque cette réponse est sélectionnée, les autres ne peuvent pas l'être)_
- [ ] 5.3.b Oui, nos réponses à cette évaluation tiennent compte des pratiques de nos sous-traitants
- [ ] 5.3.c Non, nos réponses à cette évaluation ne s'appliquent pas à nos sous-traitants et sur certains points il est possible qu'ils soient moins avancés que nous

<details>
<summary>Expl5.3 :</summary>

Comme dans les cadres connues du management des SI (ISO 27001) ou du RGPD, il est important de ne pas diluer les responsabilités dans des chaînes de sous-traitance non maîtrisées. Cela doit s'appliquer par exemple aux consultants, freelances qui viennent renforcer une équipe interne sur un projet de data science. Il est par exemple possible de demander aux sous-traitants de réaliser cette même évaluation pour leur propre compte et de partager avec vous leurs résultats.

</details>

---

### Section 6 - Utiliser des modèles prédictifs appris

Utiliser des systèmes automatiques basés sur des modèles dont les règles ont été "apprises" (et non définies et formalisées) interroge le fonctionnement des organisations. Il est important de préserver la capacité de réaction et la résilience de l'organisation utilisatrice, notamment pour traiter les cas de figure où les modèles prédictifs auront été à l'origine d'un résultat non souhaitable pour l'organisation et ses parties prenantes.

[_[⇧ retour à la liste des sections](#restructuration-en-un-référentiel-dévaluation-de-la-maturité-dune-organisation)_]  
[_[⇩ prochaine section](#section-7---anticiper-suivre-et-minimiser-les-externalités-de-lactivité-data-science)_]

---

Q6.1 : **Utilisation de modèles prédictifs pour son propre compte**  
Si votre organisation utilise pour son propre compte des modèles prédictifs :

R6.1 :  
_(Type : combiné)_  
_(Sélectionner tous les éléments de réponse correspondant à des pratiques de votre organisation. Attention, certaines combinaisons ne seraient pas cohérentes)_

- [ ] 6.1.a Notre organisation n'utilise pas de modèles prédictifs élaboré par apprentissage automatique pour son propre compte | _(Lorsque cette réponse est sélectionnée, les autres ne peuvent pas l'être)_
- [ ] 6.1.b **Un registre des modèles prédictifs** identifie tous les modèles utilisés par l'organisation, nous le maintenons à jour
- [ ] 6.1.c Pour chaque modèle nous disposons d'un **responsable point de contact** défini, identifiable et contactable simplement
- [ ] 6.1.d Pour chaque modèle, nous réalisons systématiquement une **évaluation des risques** consécutifs à d'éventuels, incidents, défaillances, biais
- [ ] 6.1.e Des outils de monitoring sont mis en place afin d'assurer une surveillance continue des systèmes de ML et peuvent déclencher des alertes directement auprès de l'équipe responsable
- [ ] 6.1.f Pour chaque modèle, nous définissons et testons une procédure de suspension du modèle et un mode de fonctionnement dégradé sans le modèle, pour parer au cas de figure où le modèle serait sujet à une défaillance ou un comportement anormal
- [ ] 6.1.g Pour chaque modèle, nous étudions sa généalogie de bout-en-bout et ses conditions et limites d'utilisation pour comprendre le modèle avant de l'utiliser
- [ ] 6.1.h Nous utilisons toujours les modèles pour des **usages en adéquation avec leurs conditions et limites d'utilisation**

<details>
<summary>Expl6.1 :</summary>

Utiliser des systèmes automatiques basés sur des modèles dont les règles ont été "apprises" (et non définies et formalisées) interroge le fonctionnement des organisations. Il est important d'évaluer les conséquences et les réactions en cas d'incident. Par ailleurs il est important qu'une personne responsable soit clairement identifiée de manière à ne laisser aucune partie prenante démunie face à une conséquence inattendue ou inappropriée. Enfin il est important de s'interroger sur les "conditions et limites de validité" des modèles que l'on utilise afin de s'assurer que l'usage que l'on prévoit est bien en adéquation.

</details>

---

Q6.2 : **Utilisation de modèles prédictifs pour le compte de tiers**  
Si votre organisation fournit à ses clients ou à des tiers, ou opère pour le compte de tiers des applications basées sur des modèles prédictifs :

R6.2 :  
_(Type : combiné)_  
_(Sélectionner tous les éléments de réponse correspondant à des pratiques de votre organisation. Attention, certaines combinaisons ne seraient pas cohérentes)_

- [ ] 6.2.a Notre organisation ne fournit pas à ses clients ou des tiers, et n'opère pas pour le compte de tiers d'application basée sur des modèles prédictifs élaboré par apprentissage automatique | _(Lorsque cette réponse est sélectionnée, les autres ne peuvent pas l'être)_
- [ ] 6.2.b **Un registre des modèles prédictifs** identifie tous les modèles ou applications utilisés par ses clients et/ou par l'organisation pour le compte de tiers, nous le maintenons à jour
- [ ] 6.2.c Pour chaque modèle ou application pour un client ou un tiers nous disposons d'un **responsable point de contact** défini, identifiable et contactable simplement
- [ ] 6.2.d Pour chaque modèle ou application pour un client ou un tiers, nous réalisons systématiquement une **évaluation des risques** consécutifs à d'éventuels, incidents, défaillances, biais
- [ ] 6.2.e Des outils de monitoring sont mis en place afin d'assurer une surveillance continue des systèmes de ML et peuvent déclencher des alertes directement auprès de l'équipe responsable
- [ ] 6.2.f Pour chaque modèle ou application pour un client ou un tiers, nous définissons et testons une procédure de suspension du modèle et un mode de fonctionnement dégradé sans le modèle, pour parer au cas de figure où le modèle serait sujet à une défaillance ou un comportement anormal
- [ ] 6.2.g Pour chaque modèle ou application pour un client ou un tiers, nous étudions sa généalogie de bout-en-bout et ses conditions et limites d'utilisation pour comprendre le modèle avant de l'utiliser
- [ ] 6.2.h Nous fournissons à nos clients ou opérons pour leur compte des modèles ou applications pour des **usages en adéquation avec leurs conditions et limites d'utilisation**

<details>
<summary>Expl6.2 :</summary>

Utiliser des systèmes automatiques basés sur des modèles dont les règles ont été "apprises" (et non définies et formalisées) interroge le fonctionnement des organisations. Il est important d'évaluer les conséquences et les réactions en cas d'incident. Par ailleurs il est important qu'une personne responsable soit clairement identifiée de manière à ne laisser aucune partie prenante démunie face à une conséquence inattendue ou inappropriée. Enfin il est important de s'interroger sur les "conditions et limites de validité" des modèles que l'on utilise afin de s'assurer que l'usage que l'on prévoit est bien en adéquation.

</details>

---

Q6.3 : **Gestion des prédictions problématiques, processus de contournement, _human agency_**  
Les systèmes automatiques, en particulier lorsqu'ils s'appuient sur des modèles prédictifs appris, sont utilisés en production généralement pour gagner en efficacité. Il se trouve que par nature, ils génèrent de temps en temps des résultats non souhaitables pour l'organisation et ses parties prenantes (e.g. prédiction erronée), puisqu'ils ne généraliseront jamais une performance de 100%.

R6.3 :  
_(Type : combiné)_  
_(Sélectionner tous les éléments de réponse correspondant à des pratiques de votre organisation. Attention, certaines combinaisons ne seraient pas cohérentes)_

- [ ] 6.3.a Notre organisation n'utilise pas de modèles prédictifs élaboré par apprentissage automatique pour son propre compte ou celui de ses clients, et ne fournit pas à ses clients d'application basée sur des modèles prédictifs | _(Lorsque cette réponse est sélectionnée, les autres ne peuvent pas l'être)_
- [ ] 6.3.b Nous appliquons systématiquement le principe de *human agency*, les sorties des modèles prédictifs que nous mettons en oeuvre sont utilisées par des opérateurs humains, et ne servent pas de déterminants à des décisions automatiques | _(Lorsque cette réponse est sélectionnée, les autres ne peuvent pas l'être)_
- [ ] 6.3.c Nous intégrons dans les systèmes automatiques s'appuyant sur des modèles prédictifs appris les fonctionnalités permettant de gérer ces cas de résultats non souhaitables. Cela est fait _ex ante_, en sollicitant un opérateur humain dans un certain nombre de cas où l'intervalle de confiance pour la décision automatique n'est pas satisfaisant
- [ ] 6.3.d Nous intégrons dans les systèmes automatiques s'appuyant sur des modèles prédictifs appris les fonctionnalités permettant de gérer ces cas de résultats non souhaitables. Cela est fait selon une modalité de gestion d'incident, c'est-à-dire de correction _ex post_ du résultat non souhaitable
- [ ] 6.3.e Nous mettons en place des mécanismes permettant à un opérateur humain, dans certaines conditions définies, d'aller contre une décision d'un modèle s'il identifie que le modèle commet une erreur

<details>
<summary>Expl6.3 :</summary>

Utiliser des systèmes automatiques basés sur des modèles dont les règles ont été "apprises" (et non définies et formalisées) interroge le fonctionnement des organisations. Il est important de préserver la capacité de réaction et la résilience de l'organisation.

</details>

<details>
<summary>Ressources6.3 :</summary>

- (Technical guide) *[Monitoring Machine Learning Models in Production - A comprehensive guide](https://christophergs.com/machine%20learning/2020/03/14/how-to-monitor-machine-learning-models/)*, ChristopherGS, March 2020

</details>

---

Q6.4 : **Transparence vis-à-vis des parties prenantes interagissant avec un modèle prédictif appris**  
Votre organisation utilise pour son propre compte, fournit à ses clients ou opère pour le compte de ses clients des applications basées sur des modèles prédictifs, avec lesquels sont à même d'interagir des utilisateurs. Que met-elle en place pour en informer les utilisateurs ?

R6.4 :  
_(Type : combiné)_  
_(Sélectionner tous les éléments de réponse correspondant à des pratiques de votre organisation. Attention, certaines combinaisons ne seraient pas cohérentes)_

- [ ] 6.4.a Notre organisation n'utilise pas de modèles prédictifs élaborés par apprentissage automatique pour son propre compte ou celui de ses clients, et ne fournit pas à ses clients d'application basée sur des modèles prédictifs | _(Lorsque cette réponse est sélectionnée, les autres ne peuvent pas l'être)_
- [ ] 6.4.b Les utilisateurs ne sont pas informés qu'ils interagissent avec un modèle prédictif appris | _(Lorsque cette réponse est sélectionnée, les autres ne peuvent pas l'être)_
- [ ] 6.4.c Une notice d'information est mise à disposition dans les conditions générales d'utilisation du système ou un document équivalent, en libre accès
- [ ] 6.4.d L'utilisation du système ou du service est explicite vis-à-vis de l'utilisateur quant au fait qu'un modèle prédictif appris est utilisé
- [ ] 6.4.e Le système ou le service propose à l'utilisateur des informations supplémentaires sur les résultats qu'aurait fourni le système ou le service dans des cas de figure légèrement différents
- [ ] 6.4.f Lorsque le système ou le service est conçu pour s'adapter au comportement de l'utilisateur et l'influencer (par exemple pour maximiser son temps d'utilisation ou les sommes qu'il dépense), et présente des risques non négligeables de manipulation ou d'addiction, l'utilisateur en est clairement informé

<details>
<summary>Expl6.4 :</summary>

Utiliser des systèmes automatiques basés sur des modèles dont les règles ont été "apprises" (et non définies et formalisées) interroge le fonctionnement des organisations mais également le rapport des utilisateurs aux systèmes et services numériques. Dans la plupart des cas il est important d'informer les utilisateurs qu'ils ne font pas face à des règles de gestion classiques.

</details>

<details>
<summary>Ressources6.4 :</summary>

- (Academic paper) *[Counterfactual Explanations without Opening the Black Box: Automated Decisions and the GDPR](https://arxiv.org/abs/1711.00399)*, S. Wachter, B. Mittelstadt, C. Russell, 2018
- (Technical guide) *[Interpretable Machine Learning - Counterfactual explanations](https://christophm.github.io/interpretable-ml-book/counterfactual.html)*, C. Molnar, 2020

</details>

---

### Section 7 - Anticiper, suivre et minimiser les externalités de l'activité data science

La mise en place d'un système automatique basé sur un modèle prédictif peut générer des externalités négatives sociales et environnementales. En prendre conscience est indispensable, ainsi qu'anticiper, chercher à suivre et minimiser les différents impacts négatifs.

[_[⇧ retour à la liste des sections](#restructuration-en-un-référentiel-dévaluation-de-la-maturité-dune-organisation)_]

---

Q7.1 : **Impact CO2**  
Au sujet de l'impact CO2 de son activité data science, au sein de votre organisation :

R7.1 :  
_(Type : réponse unique)_  
_(Sélectionner une seule réponse, correspondant le mieux au niveau de maturité de l'organisation sur ce sujet)_

- [ ] 7.1.a À ce stade nous ne nous sommes pas penchés sur l'impact CO2 de notre activité data science ou de nos modèles prédictifs
- [ ] 7.1.b Nous avons défini des indicateurs pour savoir quoi mesurer précisément
- [ ] 7.1.c Nous avons défini des indicateurs et nous incluons leurs mesures dans les généalogies de bout-en-bout des modèles
- [ ] 7.1.d Nous avons défini des indicateurs et nous les suivons régulièrement
- [ ] 7.1.e Nous avons défini des indicateurs, nous les suivons régulièrement, et nous nous sommes fixés des objectifs d'amélioration

<details>
<summary>Expl7.1 :</summary>

Il est important de s'interroger et de conscientiser les coûts environnementaux.

</details>

<details>
<summary>Ressources7.1 :</summary>

- (Tool) *[ML Impact Calculator](https://mlco2.github.io/impact/)*

</details>

---

Q7.2 : **Impact social**  
Dans certains cas, la mise en place d'un système automatique basé sur un modèle prédictif peut générer des externalités négatives sur les parties prenantes amont (par exemple annotation de données), et sur les parties prenantes aval (par exemple automatisation de certains postes). Lors de chaque projet d'élaboration ou d'utilisation d'un modèle prédictif, votre organisation :

R7.2 :  
_(Type : réponse unique)_  
_(Sélectionner une seule réponse, correspondant le mieux au niveau de maturité de l'organisation sur ce sujet)_

- [ ] 7.2.a À ce stade nous ne nous penchons pas sur l'impact social de notre activité data science ou de nos modèles prédictifs
- [ ] 7.2.b Dans certains cas nous nous interrogeons sur l'impact social
- [ ] 7.2.c Nous menons ce travail de réflexion sur l'impact social à chaque projet
- [ ] 7.2.d Nous menons ce travail de réflexion sur l'impact social à chaque projet et l'impact social est documenté dans la généalogie de bout-en-bout de chaque modèle
- [ ] 7.2.e Nous menons ce travail de réflexion sur l'impact social à chaque projet, l'impact social est documenté dans la généalogie de bout-en-bout de chaque modèle, et nous entamons systématiquement un dialogue avec les parties prenantes concernées amont et aval

<details>
<summary>Expl7.2 :</summary>

Il est important de s'interroger et d'échanger avec ses parties prenantes. Cela vaut tant pour l'aval (e.g. automatisation de certains emplois) que pour l'amont (e.g. tâches d'annotations de données parfois d'une très grande violence).

</details>

---

Q7.3 : **Ethique et non-malfaisance**  
Au sein de votre organisation :

R7.3 :  
_(Type : combiné)_  
_(Sélectionner tous les éléments de réponse correspondant à des pratiques de votre organisation. Attention, certaines combinaisons ne seraient pas cohérentes)_

- [ ] 7.3.a À ce stade nous ne nous sommes pas encore penchés sur la dimension éthique | _(Lorsque cette réponse est sélectionnée, les autres ne peuvent pas l'être)_
- [ ] 7.3.b Les collaborateurs concernés par les activités data science reçoivent une formation à l'éthique
- [ ] 7.3.c Notre organisation s'est dotée d'une politique en matière d'éthique
- [ ] 7.3.d Sur les projets le justifiant, nous mettons en place un comité d'éthique indépendant ou nous sollicitons l'évaluation d'un organisme validant l'éthique des projets

<details>
<summary>Expl7.3 :</summary>

Travailler sur de grands volumes de données dont certaines peuvent être sensibles, utiliser des systèmes automatiques basés sur des modèles dont les règles ont été "apprises" (et non définies et formalisées) interrogent le fonctionnement des organisations et la responsabilité individuelle de chacun. Il est important que l'organisation s'assure que les enjeux éthiques ne sont pas inconnus de son personnel.

</details>

<details>
<summary>Ressources7.3 :</summary>

- (Official report) Rapport *[Éthique et responsabilité des algorithmes publics](https://www.etalab.gouv.fr/wp-content/uploads/2020/01/Rapport-ENA-Ethique-et-responsabilit%C3%A9-des-algorithmes-publics.pdf)*, Etalab / ENA, Janvier 2020
- (Public declaration) *[Déclaration de Montréal pour l'IA responsable](https://www.declarationmontreal-iaresponsable.com/la-declaration)*
- (Public declaration) *[Serment Holberton-Turing](https://www.holbertonturingoath.org/accueil)*
- (Public declaration) *[Serment d'Hippocrate pour data scientist](https://hippocrate.tech/)*
- (Public declaration) *[Future of Life's AI principles](https://futureoflife.org/ai-principles/)*
- (Public declaration) *[Charte internationale pour une IA inclusive](https://charteia.arborus.org/)*, Arborus et Orange

</details>

---
---

## Risques

Quels sont les risques que l'on souhaite prévenir pour pouvoir parler de data science _responsable_ et _de confiance_ ?

Découpage en thèmes :

- EDP : l'Exposition de Données Personnelles ou confidentielles
- PDI : la Prise de Décisions Inappropriées par des systèmes automatiques
- RC : ne pas Rendre des Comptes de manière responsable à ses parties prenantes
- ESE : avoir une Empreinte Sociale et Environnementale irresponsable
- TR : transverses
- _à catégoriser_

| # | Risques | Exemples réels ou commentaires |
|:---:|:---|:---|
|  |  |  |
| **EDP** | **l'Exposition de Données Personnelles ou confidentielles** (e.g. données personnelles ou données privées d'une organisation) |  |
| EDP-01 | des datasets contenant des données personnelles ou confidentielles sont exposés | [ré-identification de datasets anonymisés](https://www.wired.com/2007/12/why-anonymous-data-sometimes-isnt/) ; [article Nature](https://www.nature.com/articles/s41467-019-10933-3/) : "Using our model, we find that 99.98% of Americans would be correctly re-identified in any dataset using 15 demographic attributes."|
| EDP-02 | un algorithme d'apprentissage machine est utilisé de manière malveillante pour extraire ou exposer des données personnelles ou confidentielles d'un dataset d'entraînement ou de test |  |
| EDP-03 | l'exploitation malveillante d'un modèle prédictif expose des données personnelles ou confidentielles | [rétro-engineering des résultats d'un algorithme](https://www.abc.net.au/news/2019-03-01/abs-census-vulnerability/10857236) |
| EDP-04 | des dispositions réglementaires font peser des risques, ou un changement réglementaire augmente les risques d'exposition de données personnelles ou confidentielles | Cloud Act ; [FATCA](https://www.cnil.fr/fr/cnil-direct/question/loi-fatca-que-faire) en contradiction avec le droit européen ; [CNB - Mise en garde HDH](https://www.cnb.avocat.fr/sites/default/files/11.cnb-mo2020-01-11_ldh_health_data_hubfinal-p.pdf) |
|  |  |  |
| **PDI** | **la Prise de Décisions Inappropriées par des systèmes automatiques**, qui seraient préjudiciables à des personnes ou des organisations | Par _inapproprié_ on entend ici infondé, injuste ou illégitime. |
| PDI-01 | la prise de décisions inappropriées du fait de biais discriminatoires dans les données d'entraînement ou de test | [cas Apple Card](https://twitter.com/dhh/status/1192540900393705474) ; [algorithme RH d'Amazon](https://www.lefigaro.fr/social/2018/10/11/20011-20181011ARTFIG00096-le-logiciel-de-recrutement-d-amazon-n-aimait-pas-les-femmes.php) ; [reconnaissance faciale](https://www.thesun.co.uk/news/5182512/chinese-users-claim-iphonex-face-recognition-cant-tell-them-apart/) ; [biais dans les systèmes de reconnaissance visuelle](https://arxiv.org/pdf/1902.11097.pdf) |
| PDI-02 | la prise de décisions inappropriées du fait de données empoisonnées (de manière malveillante, ou du fait de phénomènes diffus, mal compris) | l'exemple du [social cooling](https://usbeketrica.com/article/le-social-cooling-symptome-numerique-de-la-surveillance-de-masse) illustre la difficulté d'appréhender la fiabilité ou la signification de certains types de données |
| PDI-03 | la prise de décisions inappropriées du fait de l'utilisation de données synthétiques | _# ce risque est mal identifié/défini à ce stade #_ |
| PDI-04 | la prise de décisions inappropriées du fait de biais discriminatoires dûs à l'architecture ou la conception même de l'algorithme d'apprentissage et/ou du modèle | [modèles de word embedding](https://arxiv.org/abs/1607.06520), [doc2vec](https://www.pnas.org/content/115/16/E3635) ; utilisation de variables protégées directement |
| PDI-05 | l'utilisation de modèles prédictifs dans des contextes pour lesquels ils ne sont pas suffisamment performants, pas pertinents voire dangereux, pas prévus et validés (où leur performance réelle est insuffisante par rapport au déclaré ou à l'attendu) | [exemple de Google Flu Trends en santé](https://science.sciencemag.org/content/343/6176/1203) ; [biais et performances limitées du modèle COMPAS de prédiction de la récidive](https://advances.sciencemag.org/content/4/1/eaao5580) |
| PDI-06 | l'utilisation de modèles ayant subi une dégénérescence ou _drift_ dans le temps (par exemple, dans les cas de figure d'apprentissage en continu, lorsque les nouvelles données inputs proviennent, même indirectement, de situations dans lesquels le modèle a été utilisé) | cas à identifier (problème de capteurs de mesure en maintenance prédictive, trading...) |
| PDI-07 | l'utilisation adversariale d'un modèle prédictif de manière préjudiciable à des personnes ou des organisations | [Three Small Stickers in Intersection Can Cause Tesla Autopilot to Swerve Into Wrong Lane](https://spectrum.ieee.org/cars-that-think/transportation/self-driving/three-small-stickers-on-road-can-steer-tesla-autopilot-into-oncoming-lane) |
|  |  |  |
| **RC** | **ne pas Rendre des Comptes de manière responsable à ses parties prenantes** quant aux conséquences de l'usage de modèles prédictifs |  |
| RC-01 | dans le cas d'un incident avec ou provoqué par un modèle prédictif, ne pas avoir de personne physique ou morale identifiée à qui demander des comptes | [cas de Steve Wozniak avec l'Apple Card](https://twitter.com/stevewoz/status/1193330241478901760) |
| RC-02 | dans le cas d'un incident avec ou dû à un modèle prédictif : pour l'acteur qui met en oeuvre et opère le modèle, ne pas savoir réagir face à une demande d'interpréter et expliquer une prédiction mise en cause | [les algorithmes de censure automatiques de Facebook ont été moins efficaces lors de l'attentat de Christchurch qu'avec les vidéos de l'EI : que détectent-ils exactement ?](https://techcrunch.com/2019/03/21/facebooks-ai-couldnt-spot-mass-murder/) ; [An Algorithm that grants Freedom, or Takes it away](https://www.nytimes.com/2020/02/06/technology/predictive-algorithms-crime.html) |
| RC-03 | dans le cas d'un incident avec ou dû à un modèle prédictif : pour l'acteur qui met en oeuvre et opère le modèle, ne plus être capable d'assurer un service critique | cas à identifier |
| RC-04 | au sein d'une organisation qui utilise des systèmes automatiques basés sur des modèles prédictifs, ne pas connaître ou ne pas savoir identifier facilement qui sont les responsables de ces systèmes |  |
|  |  |  |
| **ESE** | **avoir une Empreinte Sociale et Environnementale irresponsable** |  |
| ESE-01 | ne pas connaître ou ne pas se préoccuper du coût énergétique ou environnemental de l'élaboration et de l'utilisation d'un modèle, ou qu'il soit disproportionné par rapport à l'usage cible du modèle | [AlphaGo en kW vs. 20W pour un humain](https://deepmind.com/blog/article/alphago-zero-starting-scratch) ; [ML Impact Calculator](https://mlco2.github.io/impact/) |
| ESE-02 | ne pas anticiper les impacts sociaux de l'élaboration ou de la mise en place d'un système automatique basé sur un modèle prédictif | en amont pour la production de données annotées par exemple, en aval pour l'évolution des activités impactées |
| ESE-03 | ne pas anticiper les effets négatifs/dangereux ou les usages malfaisants d'un modèle lors de la conception | [Implication analysis and release strategy of gpt2 by OpenAI](https://openai.com/blog/better-language-models/) |
|  |  |  |
| **TR** | **Transverse** |  |
| TR-01 | ne pas maîtriser les conséquences négatives de l'utilisation d'un modèle donné du fait du manque d'une "gouvernance globale" tout au long de la chaîne de valeur de bout-en-bout (données, conception, entraînement, validation, exploitation) |  |
| TR-02 | ne pas maîtriser les conséquences de l'utilisation d'un modèle du fait du manque de connaissance de sa généalogie et de maîtrise de ses conditions nominales d'utilisation | modèles qui deviennent des références et/ou fournis par des tiers |
|  |  |  |
|  | **divers - à catégoriser** |  |
|  | se faire "voler" un modèle par multiples inférences (_model stealing_) |  |
|  | se faire "voler" du temps de calcul par _adversarial reprogramming_ |  |
|  |  | placement d'offres d'emploi sur les flux d'utilisateurs sélectionnés par un modèle prédictif : y a-t-il un sens à s'interroger sur un risque de discrimination, ou bien est-ce analogue à un chasseur de tête qui décide d'appeler les candidats qui l'intéressent de manière discrétionnaire ? |

## Thèmes et canevas du référentiel d'évaluation

Propositions de thèmes pour structurer les bonnes pratiques et mesures de prévention des risques qui constituent le référentiel d'évaluation :

| # | Thèmes | Descriptions |
|:---:|:---|:---|
| T1 | **Protéger les données personnelles ou confidentielles** | L'utilisation de données personnelles ou confidentielles fait porter le risque d'exposition de celles-ci, ce qui peut avoir des conséquences très préjudiciables pour les producteurs, gestionnaires, ou sujets de ces données. Elles doivent donc être protégées, les risques d'exposition doivent être minimisés. |
| T2 | **Prévenir les biais malencontreux** | L'utilisation de modèles prédictifs élaborés à partir de données historiques peut se révéler néfaste lorsque les données historiques décrivent des phénomènes non souhaitables. Il apparaît indispensable de s'interroger sur ce risque et d'étudier la nature des données utilisées et ce qu'elles représentent. |
| T3 | **Evaluer la performance de manière rigoureuse** | Le score de performance d'un modèle prédictif est déterminant pour son adoption dans des produits, systèmes ou processus. L'évaluation de la performance se doit donc d'être rigoureuse. Une spécification de l'équité recherchée entre populations doit également être définie. En effet, l'équité d'un modèle peut [être définie de plusieurs manières qui peuvent être incompatibles entre elles](https://papers.nips.cc/paper/6995-counterfactual-fairness), et l'interprétation de scores de performances doit donc se faire dans le cadre de l'une de ces définitions. |
| T4 | **Etablir et maintenir une généalogie des modèles** | Un modèle prédictif est un objet informatique complexe qui peut évoluer au fil des apprentissages. Tracer les étapes de son élaboration et de son évolution permet d'en constituer une forme de **généalogie**, pré-requis pour **reproduire ou auditer** un modèle. |
| T5 | **Garantir la chaîne de responsabilité des modèles** | Un modèle prédictif peut-être utilisé comme un système automatique, dont les règles de fonctionnement ne sont pas écrites _in extenso_ et ne se prêtent pas ou mal à être explicitées, débattues, ajustées. Des efforts sont nécessaires sur **l'interprétation et l'explication** des choix réalisés à l'aide de ces systèmes. Il apparaît également indispensable de garantir une chaîne de responsabilité claire, de personnes physiques ou morales, pour chaque modèle. |
| T6 | **Anticiper, suivre et minimiser les externalités négatives de l'activité data science** | La mise en place d'un système automatique basé sur un modèle prédictif peut générer des externalités négatives sociales et environnementales. En prendre conscience est indispensable, ainsi qu'anticiper, chercher à suivre et minimiser les différents impacts négatifs. |
