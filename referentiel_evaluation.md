# Data science responsable et de confiance - Référentiel d'évaluation

Le [référentiel d'évaluation](#référentiel-dévaluation-de-la-maturité-dune-organisation) ci-dessous est le fruit travail participatif initié au printemps 2019 par Substra Foundation et en cours depuis. Il procède de l'identification des [risques](#risques) que l'on cherche à prévenir en visant une pratique responsable et de confiance de la data science, et des bonnes pratiques qui permettent d'y faire face. Il regroupe également pour chaque sujet des ressources techniques qui peuvent être de bons points d'entrée pour les organisations intéressées.

## Référentiel d'évaluation de la maturité d'une organisation

L'évaluation est composée des 6 sections suivantes :

- [Section 1 - Protéger les données personnelles ou confidentielles](#section-1---protéger-les-données-personnelles-ou-confidentielles)
- [Section 2 - Prévenir les biais, élaborer des modèles non discriminatoires](#section-2---prévenir-les-biais-élaborer-des-modèles-non-discriminatoires)
- [Section 3 - Evaluer la performance de manière rigoureuse](#section-3---evaluer-la-performance-de-manière-rigoureuse)
- [Section 4 - Assurer la reproductibilité des modèles et en établir la chaîne de responsabilité](#section-4---assurer-la-reproductibilité-des-modèles-et-en-établir-la-chaîne-de-responsabilité)
- [Section 5 - Utiliser des modèles en confiance et de manière responsable](#section-5---utiliser-des-modèles-en-confiance-et-de-manière-responsable)
- [Section 6 - Anticiper, suivre et minimiser les externalités négatives de l'activité data science](#section-6---anticiper-suivre-et-minimiser-les-externalités-de-lactivité-data-science)

---

### Section 1 - Protéger les données à caractère personnel ou confidentielles

L'utilisation de données à caractère personnel ou confidentielles fait porter le risque d'exposition de celles-ci, ce qui peut avoir des conséquences très préjudiciables pour les producteurs, gestionnaires, ou sujets de ces données. En particulier dans les projets de data science, elles doivent donc être protégées et les risques qu'elles fuitent ou soient exposées doivent être minimisés.

[_[⇧ retour à la liste des sections](#référentiel-dévaluation-de-la-maturité-dune-organisation)_]  
[_[⇩ prochaine section](#section-2---prévenir-les-biais-élaborer-des-modèles-non-discriminatoires)_]

---

Q1.1 : **Législation et exigences contractuelles applicables - Identification**  
En ce qui concerne les données à caractère personnel ou confidentielles, les exigences légales, statutaires, réglementaires et contractuelles en vigueur et concernant votre organisation sont :

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

Il est crucial de mettre en place des processus pour connaître et suivre l'évolution des réglementations applicables (très spécifiques dans certains domaines, par exemple dans le secteur bancaire), ainsi que pour documenter les approches et choix retenus pour être en conformité à chaque projet de data science. Exemple(s) intéressant(s) : [Welfare surveillance system violates human rights, Dutch court rules](https://www.theguardian.com/technology/2020/feb/05/welfare-surveillance-system-violates-human-rights-dutch-court-rules).

</details>

<details>
<summary>Ressources1.1 :</summary>

- (Official report) [Big data, artificial intelligence, machine learning and data protection](https://ico.org.uk/media/for-organisations/documents/2013559/big-data-ai-ml-and-data-protection.pdf), EU Information Commissioner's Office, 2017
- (Web article) [Artificial Intelligence and the GDPR: how do they interact?](https://www.avocats-mathias.com/technologies-avancees/artificial-intelligence-gdpr), Mathias Avocats, Novembre 2017
- (Web article) [How to develop Artificial Intelligence that is GDPR-friendly](https://techgdpr.com/blog/develop-artificial-intelligence-ai-gdpr-friendly/), Tech GDRP blog, Février 2019
- (Video) [What is the impact of GDPR on AI and Machine Learning?](https://www.youtube.com/watch?v=RLEtyfmsfs4&app=desktop), SwissAI Machine Learning Meetup, Septembre 2018
- (Technical guide) [L'Atelier RGPD](https://atelier-rgpd.cnil.fr/), formation en ligen proposée par la CNIL

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
La conformité de l'organisation aux exigences relatives aux données personnelles et confidentielles a-t-elle été auditée et est-elle reconnue par une certification, un label ou équivalent ?

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

<details>
<summary>Expl1.5 :</summary>

Le principe de minimisation est parfois aussi évoqué par l'expression *privacy by design*. Il est un des piliers du RGPD.

</details>
  
---

_Les éléments suivants au sein de cette section ne s'appliquent qu'aux organisations n'ayant pas sélectionné la première réponse de R1.5. Les organisations non concernées sont donc invitées à passer à la [Section 2](#section-2-prévenir-les-biais-élaborer-des-modèles-non-discriminatoires)._

---

Q1.6 : **Projet impliquant un nouveau traitement de données personnelles ou confidentielles**  
_(Condition : R1.5 <> 1.5.a)_  
Pour chaque traitement de données personnelles ou confidentielles nécessaire dans le cadre d'un projet de data science, au sein de votre organisation :

R1.6 :  
_(Type : réponses multiples possibles)_  
_(Sélectionner tous les éléments de réponse correspondant à des pratiques de votre organisation)_

- [ ] 1.6.a Nous élaborons une analyse d'impact relative à la protection des données (AIPD ; en anglais *Privacy Impact Assessment*)
- [ ] 1.6.b Nous mettons en oeuvre des mesures de protections (concernant notamment le transfert, le stockage, et l'accès aux données concernées)
- [ ] 1.6.c Nous contractualisons les relations avec les fournisseurs et les clients et les responsabilités qui en découlent

<details>
<summary>Expl1.6 :</summary>

Le *Privacy Impact Assessment* (PIA) est une méthode d'évaluation de l'impact d'un traitement de données, proche des méthodes classiques d'évaluation des risques. Dans certains cas, par exemple lorsqu'un traitement présente des risques élevés pour les droits et libertés des personnes physiques, le RGPD rend obligatoire la réalisation d'un PIA avant la mise en oeuvre du traitement.

</details>

---

Q1.7 : **Sécurité de l'apprentissage automatique - Niveau de connaissance**  
_(Condition : R1.5 <> 1.5.a)_  
La sécurité de l'apprentissage automatique (_ML security_) est un domaine en constante évolution. Dans certains cas de figure, les modèles prédictifs appris sur des données confidentielles peuvent révéler des éléments de ces données confidentielles (cf. articles cités en ressources). Au sein de votre organisation, au sujet des vulnérabilités liées aux modèles de ML et aux techniques pour s'en prémunir, le niveau de connaissance générale des collaborateurs intervenant sur les projets de data science est :

R1.7 :  
_(Type : réponse unique)_  
_(Sélectionner une seule réponse, correspondant le mieux au niveau de maturité de l'organisation sur ce sujet)_

- [ ] 1.7.a Complètement débutant
- [ ] 1.7.b Basique
- [ ] 1.7.c Confirmé
- [ ] 1.7.d Expert

<details>
<summary>Expl1.7 :</summary>

L'état de l'art de la sécurité du ML est en constante évolution. S'il est impossible de se prémunir contre toutes les vulnérabilités à tout instant, il est crucial de s'en préoccuper et d'organiser une veille. L'article [Demystifying the Membership Inference Attack](https://medium.com/disaitek/demystifying-the-membership-inference-attack-e33e510a0c39) est par exemple un point d'entrée intéressant dans un contexte de données sensibles.

</details>

<details>
<summary>Ressources1.7 :</summary>

- (Technical guide) *[Privacy Enhancing Technologies Decision Tree (v2)](https://www.private-ai.ca/PETs_Decision_Tree.png)*, Private AI, 2020
- (Web article) *[The secret-sharer: evaluating and testing unintended memorization in neural networks](https://blog.acolyer.org/2019/09/23/the-secret-sharer/)*, A. Colyer, 2019
- (Academic paper) *[Membership Inference Attacks against Machine Learning Models](https://arxiv.org/abs/1610.05820)*, R. Shokri, M. Stronati, C. Song, V. Shmatikov, 2017
- (Software & Tools) *[ML Privacy Meter](https://github.com/privacytrustlab/ml_privacy_meter): a tool to quantify the privacy risks of machine learning models with respect to inference attacks*
- (Web article) *[Demystifying the membership inference attack](https://medium.com/disaitek/demystifying-the-membership-inference-attack-e33e510a0c39)*, Disaitek, 2019
- (Academic paper) *[Inverting Gradients - How easy is it to break privacy in federated learning?](https://arxiv.org/abs/2003.14053)*, J. Geiping, H. Bauermeister, H. Dröge, M. Moeller, 2020
- (Web article) *[Top Five ML risks](https://github.com/OWASP/Top-5-Machine-Learning-Risks/blob/master/Top%205%20Machine%20Learning%20Risks.md)*, OWASP
- (Software & Tools) Outils pour la *differential privacy* : Google *[differential privacy library](https://github.com/google/differential-privacy)*, et le wrapper Python [PyDP](https://github.com/OpenMined/PyDP) d'OpenMined
- (Web article) La *distillation* d'un modèle, en plus de la compression qu'elle apporte, peut être utilisée comme une mesure de protection du modèle et des données d'entraînement utilisées, voir par exemple *[Knowledge Distillation: Simplified](https://towardsdatascience.com/knowledge-distillation-simplified-dd4973dbc764)*, Towards Data Science, 2019
- (Academic paper) *[Distilling the Knowledge in a Neural Network](https://arxiv.org/abs/1503.02531)*, G. Hinton, O. Vinyals, J. Dean, 2015

</details>

---

Q1.8 : **Sécurité de l'apprentissage automatique - Mise en oeuvre**  
_(Condition : R1.5 <> 1.5.a)_  
Toujours au sujet des vulnérabilités liées aux modèles de ML et aux techniques pour s'en prémunir :

R1.8 :  
_(Type : réponses multiples possibles)_  
_(Sélectionner tous les éléments de réponse correspondant à des pratiques de votre organisation)_

- [ ] 1.8.a Nous faisons une veille technique sur les principales attaques et mesures pour s'en prémunir
- [ ] 1.8.b Les collaborateurs reçoivent régulièrement des informations et formations qui leur permettent de développer leurs compétences dans ce domaine
- [ ] 1.8.c Dans certains projets, nous mettons en oeuvre des techniques spécifiques permettant de réduire les risques liés aux modèles que nous élaborons (par exemple : confidentialité différentielle, distillation...)
- [ ] 1.8.d Sur chaque projet, les vulnérabilités qui s'y appliquent et les techniques mises en oeuvre sont documentées (par exemple dans la généalogie de bout-en-bout de chaque modèle, voir Section 4 et élément 4.1 pour plus d'information sur ce concept)

<details>
<summary>Expl1.8 :</summary>

L'état de l'art de la sécurité du ML est en constante évolution. S'il est impossible de se prémunir contre toutes les vulnérabilités à tout instant, il est crucial de s'en préoccuper et d'organiser une veille. L'article [Demystifying the Membership Inference Attack](https://medium.com/disaitek/demystifying-the-membership-inference-attack-e33e510a0c39) est par exemple un point d'entrée intéressant dans un contexte de données sensibles.

Selon les niveaux de risque et de sensibilité des projets, certaines approches techniques pour s'en prémunir seront sélectionnées et implémentées. Il est important de suivre l'évolution de l'état de l'art et des pratiques, et de documenter les choix réalisés. On introduit ici la notion de "généalogie de bout-en-bout".

</details>

<details>
<summary>Ressources1.8 :</summary>

- (Technical guide) *[Privacy Enhancing Technologies Decision Tree (v2)](https://www.private-ai.ca/PETs_Decision_Tree.png)*, Private AI, 2020
- (Web article) *[The secret-sharer: evaluating and testing unintended memorization in neural networks](https://blog.acolyer.org/2019/09/23/the-secret-sharer/)*, A. Colyer, 2019
- (Academic paper) *[Membership Inference Attacks against Machine Learning Models](https://arxiv.org/abs/1610.05820)*, R. Shokri, M. Stronati, C. Song, V. Shmatikov, 2017
- (Software & Tools) *[ML Privacy Meter](https://github.com/privacytrustlab/ml_privacy_meter): a tool to quantify the privacy risks of machine learning models with respect to inference attacks*
- (Web article) *[Demystifying the membership inference attack](https://medium.com/disaitek/demystifying-the-membership-inference-attack-e33e510a0c39)*, Disaitek, 2019
- (Academic paper) *[Inverting Gradients - How easy is it to break privacy in federated learning?](https://arxiv.org/abs/2003.14053)*, J. Geiping, H. Bauermeister, H. Dröge, M. Moeller, 2020
- (Web article) *[Top Five ML risks](https://github.com/OWASP/Top-5-Machine-Learning-Risks/blob/master/Top%205%20Machine%20Learning%20Risks.md)*, OWASP
- (Software & Tools) Outils pour la *differential privacy* : Google *[differential privacy library](https://github.com/google/differential-privacy)*, et le wrapper Python [PyDP](https://github.com/OpenMined/PyDP) d'OpenMined
- (Web article) La *distillation* d'un modèle, en plus de la compression qu'elle apporte, peut être utilisée comme une mesure de protection du modèle et des données d'entraînement utilisées, voir par exemple *[Knowledge Distillation: Simplified](https://towardsdatascience.com/knowledge-distillation-simplified-dd4973dbc764)*, Towards Data Science, 2019
- (Academic paper) *[Distilling the Knowledge in a Neural Network](https://arxiv.org/abs/1503.02531)*, G. Hinton, O. Vinyals, J. Dean, 2015

</details>

---

Q1.9 : **Notifications d’incidents de sécurité aux autorités de régulation**  
_(Condition : R1.5 <> 1.5.a)_  
Dans le cas de figure où un modèle que l'organisation a élaboré est utilisé ou accessible par une ou plusieurs parties prenantes externes, et qu'une vulnérabilité nouvelle est publiée, présente un risque de s'y appliquer et crée ainsi un risque d'exposition de données personnelles ou confidentielles :

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

### Section 2 - Prévenir les biais, élaborer des modèles non discriminatoires

L'utilisation de modèles prédictifs élaborés à partir de données historiques peut se révéler contre-productive lorsque les données historiques sont contaminées par des phénomènes problématiques (e.g. qualité de certains points de données, données non comparables, phénomène social non souhaitable du fait de l'époque...). Or un enjeu-clé pour la data science responsable et de confiance est de respecter le principe de diversité, non-discrimination et équité (décrit par exemple à la section 1.5 des [Ethics Guidelines for Trustworthy AI](https://ec.europa.eu/newsroom/dae/document.cfm?doc_id=60419) de l'UE). Il apparaît donc indispensable de s'interroger sur ce risque et d'étudier la nature des données utilisées, les conditions dans lesquelles elles ont été produites et assembées, et ce qu'elles représentent.
Entre autres, dans certains cas une spécification de l'équité recherchée entre populations doit également être définie. L'équité d'un modèle peut [être définie de plusieurs manières qui peuvent être incompatibles entre elles](https://papers.nips.cc/paper/6995-counterfactual-fairness), et l'interprétation de scores de performances doit donc se faire dans le cadre de l'une de ces définitions.

[_[⇧ retour à la liste des sections](#référentiel-dévaluation-de-la-maturité-dune-organisation)_]  
[_[⇩ prochaine section](#section-3---evaluer-la-performance-de-manière-rigoureuse)_]

---

Q2.1 : **Analyse des données d'entraînement utilisées**  
Au sein des projets de data science et lors de l'élaboration de jeux de données d'entraînement, un travail de réflexion et recherche de phénomènes problématiques (e.g. qualité de certains points de données, données non comparables du fait des outils ou processus d'enregistrement, phénomène social non souhaitable du fait de l'époque, du contexte, etc.) peut s'avérer crucial pour prévenir des biais portant atteinte au principe de non-discrimination, de diversité et d'équité. Votre organisation :

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

- (Web article) *[Hidden Bias](https://pair.withgoogle.com/explorables/hidden-bias/)* explorable from [PAIR](https://pair.withgoogle.com/)
- (Technical guide) *[Tour of Data Sampling Methods for Imbalanced Classification](https://machinelearningmastery.com/data-sampling-methods-for-imbalanced-classification/)*

</details>

---

Q2.2 : **Risques de discrimination à l'encontre de certains groupes sociaux**  
Votre organisation est-elle concernée par des cas de figure où des modèles prédictifs sont utilisés dans des environnements thématiques pour lesquels des risques de discrimination à l'encontre de certains groupes sociaux (genre, origine, âge, etc.) existent ? (L'élément d'évaluation suivant est dédié à ces cas de figure) :

R2.2 :  
_(Type : réponse unique)_  
_(Sélectionner une seule réponse, correspondant le mieux au niveau de maturité de l'organisation sur ce sujet)_

- [ ] 2.2.a Concerné
- [ ] 2.2.b Non concerné

---

_Les éléments suivants au sein de cette section ne s'appliquent qu'aux organisations ayant sélectionné la réponse "Concerné" de R2.2. Les organisations non concernées sont donc invitées à passer à la [Section 3](#section-3-evaluer-la-performance-de-manière-rigoureuse-et-expliquer-les-prédictions)._

---

Q2.3 : **Prévention des biais discriminatoires**  
_(Condition : R2.2 <> 2.2.b)_  
Dans les cas de figure où les modèles prédictifs que votre organisation élabore sont utilisés dans des environnements thématiques où il y a des risques de discrimination à l'encontre de certains groupes sociaux (genre, origine, âge, etc.) :

R2.3 :  
_(Type : réponses multiples possibles)_  
_(Sélectionner tous les éléments de réponse correspondant à des pratiques de votre organisation)_

- [ ] 2.3.a Nous portons une attention particulière à l'identification d'attributs protégés et à leurs proxys éventuels (par exemple étude une à une des variables utilisées en entrées du modèle pour recenser les corrélations qu’elles pourraient avoir avec des données sensibles)
- [ ] 2.3.b Nous procédons à des évaluations sur des données de test comprenant différentes sous-populations afin d'identifier les éventuels biais problématiques
- [ ] 2.3.c Nous sélectionnons et mettons en oeuvre une ou plusieurs mesure(s) de justice et d'équité (_fairness metric_)
- [ ] 2.3.d Nous mettons en oeuvre des approches de type _data augmentation_ ou _re-weighting_ dans le but de réduire les éventuels biais des jeux de données
- [ ] 2.3.e Les pratiques ci-dessus que nous mettons en oeuvre sont dûment documentées et intégrées à la généalogie de bout-en-bout des modèles concernés

<details>
<summary>Expl2.3 :</summary>

Il s'agit de s'interroger systématiquement, à chaque projet de data science et selon l'objectif et l'usage cible du modèle que l'on veut élaborer, sur les features pouvant directement ou indirectement être à l'origine d'un risque de biais discriminatoire. On parle d'attribut protégé (*protected attribute* ou *protected variable* en anglais) pour désigner les attributs dont les valeurs définissent des sous-populations à risque de discrimination.
Complément sur l'utilisation de données synthétiques et d'approches de _data augmentation_, _re-weighting_ dans le but de réduire les éventuels biais des jeux de données : lorsque de telles techniques sont utilisées il est important de les expliciter, au risque sinon de perdre de l'information sur la manière dont un modèle a été élaboré.

</details>

<details>
<summary>Ressources2.3 :</summary>

- (Web article) *[Unfair biases in Machine Learning: what, why, where and how to obliterate them](https://www.mlsecurity.ai/post/unfair-biases-in-machine-learning-what-why-where-and-how-to-obliterate-them)*, blog ML Security, P. Irolla, Avril 2020
- (Web article) [Awful AI](https://github.com/daviddao/awful-ai), un registre des services ou projets d'IA inquiétants, David Dao
- (Technical guide) *[A Tutorial on Fairness in Machine Learning](https://towardsdatascience.com/a-tutorial-on-fairness-in-machine-learning-3ff8ba1040cb)*, blog Towards Data Science, Z. Zhong, Octobre 2018
- (Web article) *[Measuring fairness](https://pair.withgoogle.com/explorables/measuring-fairness)* explorable, [PAIR](https://pair.withgoogle.com/)
- (Software & Tools) *[AI Fairness 360](https://developer.ibm.com/technologies/artificial-intelligence/projects/ai-fairness-360/): an open source software toolkit that can help detect and remove bias in machine learning models*, IBM
- (Academic paper) *Fairness metrics* : *[counterfactual fairness](https://papers.nips.cc/paper/6995-counterfactual-fairness)*
- (Academic paper) *Fairness metrics* : *[adversarial debiaising](https://arxiv.org/pdf/1801.07593.pdf)*
- (Technical guide) Livre *Fair ML* : *[Fairness and machine learning - Limitations and opportunities](https://fairmlbook.org/)*, Solon Barocas, Moritz Hardt, Arvind Narayanan, Décembre 2019

</details>

---
---

### Section 3 - Evaluer la performance de manière rigoureuse

Les performances des modèles sont déterminantes pour leur adoption dans des produits, systèmes ou processus. L'évaluation de la performance se doit donc d'être rigoureuse.

[_[⇧ retour à la liste des sections](#référentiel-dévaluation-de-la-maturité-dune-organisation)_]  
[_[⇩ prochaine section](#section-4---assurer-la-reproductibilité-des-modèles-et-en-établir-la-chaîne-de-responsabilité)_]

---

Q3.1 : **Séparation des jeux de données de test**  
Au sein des projets de data science et lors de l'élaboration de jeux de données de test, il est capital d'assurer la non-contamination par des données d'entraînement. Votre organisation :

R3.1 :  
_(Type : réponses multiples possibles)_  
_(Sélectionner tous les éléments de réponse correspondant à des pratiques de votre organisation. Attention, certaines combinaisons ne seraient pas cohérentes)_

- [ ] 3.1.a Fonctionne de manière informelle à ce sujet et s'appuie sur la compétence et la responsabilité des collaborateurs impliquées
- [ ] 3.1.b Dispose d'une approche documentée et systématiquement mise en oeuvre d'isolation des jeux de données de test
- [ ] 3.1.c Utilise un outil de versionnage et de traçabilité des jeux de données d'entraînement et de test utilisés, permettant ainsi de vérifier ou auditer ultérieurement la non-contamination des données de tests
- [ ] 3.1.d Prévoit systématiquement l'élaboration de deux jeux de données de test ou plus pour gagner en résilience

<details>
<summary>Expl3.1 :</summary>

Assurer l'étanchéité des jeux de données d'entraînement et de test est un principe connu et maîtrisé par la plupart des organisations. Il peut se révéler délicats dans certaines configurations particulières (e.g. apprentissage continu, apprentissage distribué *privacy-preserving*...).

</details>

---

Q3.2 : **Projets d'apprentissage distribué préservant la confidentialité**  
Dans les cas de figure de projets de data science basé sur l'apprentissage distribué ou fédéré (*distributed learning* ou *federated learning*) sur des jeux de données multiples et dont la confidentialité doit être préservée vis-à-vis des autres (*privacy-preserving*) :

R3.2 :  
_(Type : réponse unique)_  
_(Sélectionner une seule réponse, correspondant le mieux au niveau de maturité de l'organisation sur ce sujet)_

- [ ] 3.2.a Nous ne participons pas à des projets d'apprentissage distribué *privacy-preserving* | _(Concerné / Non concerné)_
- [ ] 3.2.b Nous maîtrisons et mettons en oeuvre des approches permettant d'élaborer des jeux de données de test de manière à ce qu'il n'y ait pas de contamination croisée entre données d'entraînement et de test provenant des différents partenaires
- [ ] 3.2.c À ce stade nous ne maîtrisons pas les méthodes permettant d'élaborer des jeux de données de test de manière à ce qu'il n'y ait pas de contamination croisée entre données d'entraînement et de test provenant des différents partenaires

<details>
<summary>Expl3.2 :</summary>

Dans ce type de projet d'apprentissage distribué dans des conditions où les données sont maintenues confidentielles, se pose la question de comment composer un jeu de données de test en s'assurant que celles-ci ne figurent pas aussi dans le jeu de données d'entraînement (par exemple chez un autre partenaire).

</details>

<details>
<summary>Ressources3.2 :</summary>

- (Academic paper) [Stratified cross-validation for unbiased and privacy-preserving federated learning](https://arxiv.org/abs/2001.08090), R. Bey, R. Goussault, M. Benchoufi, R. Porcher, Janvier 2020

</details>

---

Q3.3 : **Analyse des données de test**  
Au sein des projets de data science et lors de l'élaboration de jeux de données de test, un travail de réflexion et recherche de phénomènes problématiques (e.g. qualité de certains points de données, données non comparables du fait des outils ou processus d'enregistrement, phénomène social non souhaitable du fait de l'époque, du contexte, etc.) peut s'avérer crucial pour la signification des scores de performance. Votre organisation :

R3.3 :  
_(Type : réponse unique)_  
_(Sélectionner une seule réponse, correspondant le mieux au niveau de maturité de l'organisation sur ce sujet)_

- [ ] 3.3.a Fonctionne de manière informelle à ce sujet et s'appuie sur la compétence et la responsabilité des collaborateurs impliquées
- [ ] 3.3.b Dispose d'une approche documentée et systématiquement mise en oeuvre

<details>
<summary>Expl3.3 :</summary>

L'utilisation de modèles prédictifs testés sur des données historiques peut se révéler contre-productive lorsque les données historiques en question sont contaminées par des phénomènes problématiques. Il apparaît indispensable de s'interroger sur ce risque et d'étudier la nature des données utilisées, les conditions dans lesquelles elles ont été produites et assemblées, et ce qu'elles représentent.

</details>

---

Q3.4 : **Validation des performances**  
Votre organisation met-elle en oeuvre les approches suivantes :

R3.4 :  
_(Type : réponses multiples possibles)_  
_(Sélectionner tous les éléments de réponse correspondant à des pratiques de votre organisation)_

- [ ] 3.4.a Lors de l'élaboration d'un modèle, nous choisissons la ou les métrique(s) de performance en amont de l'apprentissage automatique, parmi les métriques les plus standards possibles
- [ ] 3.4.b La mise en oeuvre de mesures ou tests de robustesse (*robustness metrics*) est considérée et évaluée pour chaque projet d'élaboration d'un modèle, et appliquée par défaut dans les cas de figure où les données d'entrées peuvent être soumises à des perturbations fines (e.g. images, sons)
- [ ] 3.4.c Les pratiques ci-dessus que nous mettons en oeuvre sont documentées et intégrées à la généalogie de bout-en-bout des modèles concernés, y compris les métriques de performance choisies

<details>
<summary>Expl3.4 :</summary>

Sur le fait de choisir les métriques en amont, voir par exemple le risque de *[p-hacking / data dredging](https://fr.wikipedia.org/wiki/Data_dredging)*.
Sur la robustesse, une définition intuitive est qu'un modèle est robuste lorsque sa performance est stable quand les données d'entrée reçoivent des perturbations. Pour plus d'informations voir les ressources techniques indiquées.

</details>

<details>
<summary>Ressources3.4 :</summary>

- (Web article) *[The Comprehensive Guide to Model Validation Framework: What is a Robust Machine Learning Model?](https://medium.com/@ODSC/the-comprehensive-guide-to-model-validation-framework-what-is-a-robust-machine-learning-model-7bdbc41c1702)*, Open Data Science, Mars 2020
- (Web article) *[Testing Robustness Against Unforeseen Adversaries](https://openai.com/blog/testing-robustness/)*, Open AI, Août 2019
- (Academic paper) *Robustness metrics* : *[noise sensitivity score](https://arxiv.org/abs/1806.01477)*.
- (Technical guide) *[Adversarial Robustness - Theory and Practice](https://adversarial-ml-tutorial.org/)*, Z. Kolter et A. Madry

</details>

---

Q3.5 : **Suivi de la performance dans le temps**  
Dans les cas de figure où des modèles prédictifs élaborés par votre organisation sont utilisés dans des systèmes en production :

R3.5 :  
_(Type : réponses multiples possibles)_  
_(Sélectionner tous les éléments de réponse correspondant à des pratiques de votre organisation. Attention, certaines combinaisons ne seraient pas cohérentes)_

- [ ] 3.5.a Les modèles que nous élaborons ne sont pas utilisés dans des systèmes en production | _(Concerné / Non concerné)_
- [ ] 3.5.b La performance est systématiquement ré-évaluée lorsque le modèle est mis à jour
- [ ] 3.5.c La performance est systématiquement ré-évaluée lorsque le contexte d'utilisation du modèle évolue, ce qui peut créer un risque sur la performance du modèle du fait de l'évolution de l'espace des données d'entrée
- [ ] 3.5.d La distribution des données d'entrée est monitorée, et la performance est ré-évaluée régulièrement sur des données de test actualisées
- [ ] 3.5.e Des contrôles aléatoires sont réalisés sur des prédictions afin d'en contrôler la cohérence

<details>
<summary>Expl3.5 :</summary>

Même sur un modèle stable il existe un risque que les données d'entrée ne soient plus dans le domaine au bout d'un certain temps (population & distribution), exemple : une variable qui ne serait plus renseignée à la même fréquence qu'avant par les utilisateurs dans un SI. Il est donc nécessaire de contrôler régulièrement la performance d'un modèle utilisé dans son contexte d'utilisation.
Suivre l'évolution de la performance des modèles dans le temps est également particulièrement important dans les cas de figure d'apprentissage continu, présentant un risque de dégénérescence des modèles.

</details>

<details>
<summary>Ressources3.5 :</summary>

- (Technical guide) *[Continuous delivery for machine learning](https://martinfowler.com/articles/cd4ml.html)*, D. Sato, A. Wider, C. Windheuser, Septembre 2019
- (Technical guide) *[Monitoring Machine Learning Models in Production - A comprehensive guide](https://christophergs.com/machine%20learning/2020/03/14/how-to-monitor-machine-learning-models/)*, Christopher Samiullah, Mars 2020
- (Web article) *[Google’s medical AI was super accurate in a lab. Real life was a different story](https://www.technologyreview.com/2020/04/27/1000658/google-medical-ai-accurate-lab-real-life-clinic-covid-diabetes-retina-disease/)*, MIT Technology Review

</details>

---

Q3.6 : **Seuils de décision et plages d'indécision**  
Pour la définition des seuils de décision des modèles ou des systèmes automatiques s'appuyant dessus, votre organisation :

R3.6 :  
_(Type : réponses multiples possibles)_  
_(Sélectionner tous les éléments de réponse correspondant à des pratiques de votre organisation. Attention, certaines combinaisons ne seraient pas cohérentes)_

- [ ] 3.6.a Fonctionne de manière informelle à ce sujet et s'appuie sur la compétence et la responsabilité des collaborateurs impliquées
- [ ] 3.6.b Dispose d'une approche documentée et systématiquement mise en oeuvre
- [ ] 3.6.c Prend en compte la possibilité de maintenir des plages d'indécision dans certains cas de figure
- [ ] 3.6.d Les choix réalisés pour chaque modèle et mis en oeuvre sont documentés et intégrés à la généalogie de bout-en-bout des modèles concernés

<details>
<summary>Expl3.6 :</summary>

L'étude et à la sélection de seuils de décisions pertinents pour un problème de data science donné (*threshold selection*) est lié aux métriques retenues. Comme le présente l'article indiqué dans les ressources de cet élément d'évaluation, il peut être intéressant dans certains cas de considérer la possibilité de définir des plages d'indécision.

</details>

<details>
<summary>Ressources3.6 :</summary>

- (Web article) *[Opening the algorithm’s black box and understand its outputs](https://medium.com/@asaboni/opening-the-algorithms-black-box-and-understand-its-outputs-e2363b0a887c)*, A. Saboni (Octo Technologies), April 2020

</details>

---

Q3.7 : **Audits par des tierces parties indépendantes et *verifiable claims***  
Lorsque votre organisation communique sur les résultats ou la performance d'un système d'IA, et s'appuie sur de telles communications pour son développement et vis-à-vis de ses parties prenantes :

R3.7 :  
_(Type : réponse unique)_  
_(Sélectionner une seule réponse, correspondant le mieux au niveau de maturité de l'organisation sur ce sujet)_

- [ ] 3.7.a Nous ne communiquons pas et n'utilisons pas les résultats ou la performance de nos systèmes d'IA comme argument vis-à-vis de nos parties prenantes, nous ne sommes pas concernés par cet élément d'évaluation | _(Concerné / Non concerné)_
- [ ] 3.7.b Nous communiquons sur nos résultats et nous appuyons sur ceux-ci pour notre développement sans faire auditer auparavant nos travaux par une tierce partie indépendante, sans mettre à disposition d'éléments de preuve
- [ ] 3.7.c Nous faisons auditer nos travaux par une tierce partie indépendante, ou nous mettons à disposition des éléments de preuve, avant de communiquer sur nos résultats et de nous en prévaloir vis-à-vis de nos parties prenantes

<details>
<summary>Expl3.7 :</summary>

L'élaboration d'un modèle prédictif, et la détermination d'une mesure de performance de référence, signifiante et fiable, sont des défis complexes. Il est donc souvent délicat pour une organisation d'affirmer l'obtention d'excellents résultats et de s'en prévaloir avec certitude. Et lorsque cela est toutefois possible, il peut être plus délicat encore de mettre à disposition publiquement des éléments de preuve sans avoir à révéler d'information précieuse composant la propriété intellectuelle de l'organisation et la valeur même des travaux réalisés. Dans ces cas de figure, il est recommandé de faire procéder à un audit par une tierce partie indépendante (e.g. sécurité, privacy, fairness, fiabilité...), afin de sécuriser les résultats dont l'organisation souhaite se prévaloir.

</details>

<details>
<summary>Ressources3.7 :</summary>

- (Academic paper) [Toward Trustworthy AI Development: Mechanisms for Supporting Verifiable Claims](https://arxiv.org/pdf/2004.07213.pdf), §2 p.8-20, Avril 2020

</details>

---
---

### Section 4 - Assurer la reproductibilité des modèles et en établir la chaîne de responsabilité

Un modèle prédictif est un objet informatique complexe qui peut évoluer au fil des apprentissages. Tracer les étapes de son élaboration et de son évolution permet d'en constituer une forme de **généalogie**, pré-requis pour **reproduire ou auditer** un modèle. Par ailleurs utiliser des systèmes automatiques basés sur des modèles dont les règles ont été "apprises" (et non définies et formalisées) interroge le fonctionnement des organisations. Il apparaît indispensable de garantir une chaîne de responsabilité claire, de personnes physiques ou morales, pour chaque modèle.

[_[⇧ retour à la liste des sections](#référentiel-dévaluation-de-la-maturité-dune-organisation)_]  
[_[⇩ prochaine section](#section-5---utiliser-des-modèles-en-confiance-et-de-manière-responsable)_]

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

Ce concept de "généalogie de bout-en-bout" d'un modèle prédictif appris peut se décliner sous la forme par exemple d'un document de référence reprenant tous les choix importants ainsi que tout l'historique d'élaboration du modèle (données utilisées, pré-traitements réalisés, type d'apprentissage et architecture du modèle, seuils de décision, métriques de tests...), etc.), et de processus internes organisant cette activité. En particulier, il est intéressant d'y faire figurer les choix de compromis (*trade-offs*) qui ont été faits et pourquoi (e.g. trade-offs précision-spécificité, performance-privacy, performance-coût computationnel, etc.).

</details>

<details>
<summary>Ressources4.1 :</summary>

- (Software & Tools) [Substra Framework](http://doc.substra.ai/): *an open source framework offering distributed orchestration of machine learning tasks among partners while guaranteeing secure and trustless traceability of all operations*
- (Software & Tools) [MLflow](https://mlflow.org/): *an open source platform to manage the ML lifecycle, including experimentation, reproducibility, deployment, and a central model registry*
- (Software & Tools) [DVC](https://dvc.org/): *an Open-source Version Control System for Machine Learning Projects*
- (Software & Tools) [DAGsHub](https://dagshub.com/docs/): *a platform for data version control and collaboration, based on DVC*

</details>

---

Q4.2 : **Conditions et limites d'utilisation d'un modèle**  
Dans le cadre des projets de data science, les "conditions et limites de validité" d'un modèle conçu, entraîné et validé par l'organisation :

R4.2 :  
_(Type : réponses multiples possibles)_  
_(Sélectionner tous les éléments de réponse correspondant à des pratiques de votre organisation. Attention, certaines combinaisons ne seraient pas cohérentes)_

- [ ] 4.2.a Ne sont pas documentées
- [ ] 4.2.b Sont explicitées et documentées
- [ ] 4.2.c Sont versionnées
- [ ] 4.2.d Contiennent une description des risques que présenterait une utilisation en dehors des "conditions et limites de validité"
- [ ] 4.2.e Les documents présentant ces "conditions et limites de validité" accompagnent systématiquement les modèles tout au long de leur cycle de vie

<details>
<summary>Expl4.2 :</summary>

Il s'agit d'expliciter et d'adjoindre au modèle la description du contexte d'utilisation pour lequel il a été conçu et dans lequel sa performance annoncée est significative. Ce concept de "conditions et limites de validité" peut se décliner sous la forme d'un document synthétique ou d'une section spécifique dans la "généalogie de bout-en-bout".

</details>

<details>
<summary>Ressources4.2 :</summary>

- (Academic paper) [Model Cards for Model Reporting](https://arxiv.org/abs/1810.03993), M. Mitchell, S. Wu, A. Zaldivar, P. Barnes, L. Vasserman, B. Hutchinson, E. Spitzer, I. D. Raji, T. Gebru, Janvier 2019
- (Web article) [Model Cards](https://modelcards.withgoogle.com/about) de Google est un framework ouvert et évolutif, et propose 2 exemples : *To explore the possibilities of model cards in the real world, we've designed examples for two features of our Cloud Vision API, Face Detection and Object Detection. They provide simple overviews of both models' ideal forms of input, visualize some of their key limitations, and present basic performance metrics.*

</details>

---

Q4.3 : **Analyse et partage d'incidents**  
Dans le cadre des projets de data science, lorsqu'un comportement inattendu d'un modèle est observé :

R4.3 :  
_(Type : réponses multiples possibles)_  
_(Sélectionner tous les éléments de réponse correspondant à des pratiques de votre organisation. Attention, certaines combinaisons ne seraient pas cohérentes)_

- [ ] 4.3.a À ce stade nous ne faisons pas d'analyse des incidents ou comportements inattendus observés
- [ ] 4.3.b Nous analysons les incidents ou comportements inattendus rencontrés et les publions lorsque cela est pertinent (e.g. article, blog)
- [ ] 4.3.c Nous nous impliquons dans des clubs, cercles, ou associations professionnelles dans le domaine de la data science, et y faisons des retours d'expérience des incidents comportements inattendus que nous observons

<details>
<summary>Expl4.3 :</summary>

La compréhension voire la maîtrise du comportement d'un modèle prédictif appris sont des défis complexes. De nombreuses recherches sont en cours pour développer des méthodes et des outils dans ce domaine, mais beaucoup reste à faire. Le partage par les praticiens des incidents et comportements inattendus qu'ils rencontrent contribue faire progresser la communauté.

</details>

<details>
<summary>Ressources4.3 :</summary>

- (Software & Tools) [AI Incident Registry](http://aiid.partnershiponai.org/), Partnership on AI
- (Web article) [Specification gaming examples in AI](https://docs.google.com/spreadsheets/d/e/2PACX-1vRPiprOaC3HsCf5Tuum8bRfzYUiKLRqJmbOoC-32JorNdfyTiRRsR6Ea5eWtvsWzuxo8bjOxCG84dAg/pubhtml), Victoria Krakovna
- (Web article) [Learning from Tay's introduction](https://blogs.microsoft.com/blog/2016/03/25/learning-tays-introduction/) : analyse d'incident relative au chatbot Tay, Microsoft, 2016
- (Academic paper) [Toward Trustworthy AI Development: Mechanisms for Supporting Verifiable Claims](https://arxiv.org/pdf/2004.07213.pdf), §2.4 p.19, Avril 2020

</details>

---

Q4.4 : **Chaîne de valeur et de responsabilités**  
Dans le cas de figure des projets de data science où plusieurs acteurs, y compris internes à l'organisation (équipes, départements, filiales), sont parties prenantes tout au long de la chaîne de valeur et de responsabilités :

R4.4 :  
_(Type : réponses multiples possibles)_  
_(Sélectionner tous les éléments de réponse correspondant à des pratiques de votre organisation. Attention, certaines combinaisons ne seraient pas cohérentes)_

- [ ] 4.4.a Au sein de notre organisation les projets de data science sont menés de bout-en-bout par des équipes autonomes, y compris l'élaboration de jeux de données et l'exploitation pour son propre compte des modèles. En conséquence, pour chaque projet une équipe autonome est seule responsable | _(Concerné / Non concerné)_
- [ ] 4.4.b Nous procédons systématiquement à l'identification des risques et responsabilités de chacune des parties prenantes internes ou externes avec lesquelles nous collaborons
- [ ] 4.4.c Nous contractualisons systématiquement avec les acteurs amont (e.g. fournisseurs de données) et aval (e.g. clients, partenaires utilisateurs de modèles)

<details>
<summary>Expl4.4 :</summary>

Il est important de s'assurer que les organisations en amont et en aval de la chaîne identifient et endossent bien leurs responsabilités sur leurs segments de la chaîne de valeur.

</details>

---

Q4.5 : **Sous-traitance de tout ou partie des activités data science**  
Les activités data science sous-traitées à une ou des organisation(s) tierce(s) sont soumises aux mêmes exigences que celles que votre organisation s'applique à elle-même :

R4.5 :  
_(Type : réponse unique)_  
_(Sélectionner une seule réponse, correspondant le mieux au niveau de maturité de l'organisation sur ce sujet)_

- [ ] 4.5.a Non concerné, nous ne sous-traitons pas ces activités | _(Concerné / Non concerné)_
- [ ] 4.5.b Oui, nos réponses à cette évaluation tiennent compte des pratiques de nos sous-traitants
- [ ] 4.5.c Non, nos réponses à cette évaluation ne s'appliquent pas à nos sous-traitants et sur certains points il est possible qu'ils soient moins avancés que nous

<details>
<summary>Expl4.5 :</summary>

Comme dans les cadres connues du management des SI (ISO 27001) ou du RGPD, il est important de ne pas diluer les responsabilités dans des chaînes de sous-traitance non maîtrisées. Cela doit s'appliquer par exemple aux consultants, freelances qui viennent renforcer une équipe interne sur un projet de data science. Il est par exemple possible de demander aux sous-traitants de réaliser cette même évaluation pour leur propre compte et de partager avec vous leurs résultats.

</details>

---

Q4.6 : **Répartition de la création de valeur**  
Dans les cas de figure des projets de data science où plusieurs partenaires concourent aux côtés de votre organisation à l'élaboration d'un modèle, et que celui-ci est ou sera l'objet d'une activité économique :

R4.6 :  
_(Type : réponses multiples possibles)_  
_(Sélectionner tous les éléments de réponse correspondant à des pratiques de votre organisation. Attention, certaines combinaisons ne seraient pas cohérentes)_

- [ ] 4.6.a Notre organisation exerce ses activités de data science de manière autonome, y compris l'élaboration de jeux de données et l'exploitation pour son propre compte des modèles. Elle n'est donc pas concernée | _(Concerné / Non concerné)_
- [ ] 4.6.b À ce stade nous n'avons pas structuré cet aspect des projets de data science multi-partenaires
- [ ] 4.6.c Dans ces cas de figure nous contractualisons le volet économique de la relation avec les parties prenantes impliquées en amont du projet
- [ ] 4.6.d Notre organisation s'est dotée d'une politique encadrant de manière responsable le partage de valeur avec les parties prenantes impliquées

<details>
<summary>Expl4.6 :</summary>

Lorsque plusieurs partenaires collaborent pour l'élaboration d'un modèle, il est important que la répartition de valeur consécutives à une activité économique dans laquelle le modèle joue un rôle soit explicitée et contractualisée. Dans certains cas de figure cette question peut être complexe, par exemple lorsqu'un modèle est entraîné de manière distribuée sur plusieurs jeux de données.

</details>

<details>
<summary>Ressources4.6 :</summary>

- (Code repository) [Exploration of dataset contributivity to a model in collaborative ML projects](https://github.com/SubstraFoundation/distributed-learning-contributivity), un projet open source animé par [Substra Foundation](https://www.substra.ai/)

</details>

---
---

### Section 5 - Utiliser des modèles en confiance et de manière responsable

un modèle prédictif peut-être utilisé comme un système automatique, dont les règles de fonctionnement ne sont pas écrites _in extenso_ et ne se prêtent pas ou mal à être explicitées, débattues, ajustées. Utiliser des systèmes automatiques basés sur des modèles dont les règles ont été "apprises" (et non définies et formalisées) interroge donc le fonctionnement des organisations. Il est important de préserver la capacité de réaction et la résilience de l'organisation utilisatrice, notamment pour traiter les cas de figure où les modèles prédictifs auront été à l'origine d'un résultat non souhaitable pour l'organisation ou ses parties prenantes. Par ailleurs, des efforts sont donc nécessaires sur l'interprétation et l'explication des choix réalisés à l'aide de ces systèmes.

[_[⇧ retour à la liste des sections](#référentiel-dévaluation-de-la-maturité-dune-organisation)_]  
[_[⇩ prochaine section](#section-6---anticiper-suivre-et-minimiser-les-externalités-de-lactivité-data-science)_]

---

Q5.1 : **Utilisation de modèles prédictifs pour son propre compte**  
Si votre organisation utilise pour son propre compte des modèles prédictifs :

R5.1 :  
_(Type : réponses multiples possibles)_  
_(Sélectionner tous les éléments de réponse correspondant à des pratiques de votre organisation. Attention, certaines combinaisons ne seraient pas cohérentes)_

- [ ] 5.1.a Notre organisation n'utilise pas de modèles prédictifs élaborés par apprentissage automatique pour son propre compte | _(Concerné / Non concerné)_
- [ ] 5.1.b **Un registre des modèles prédictifs** identifie tous les modèles utilisés par l'organisation, nous le maintenons à jour
- [ ] 5.1.c Pour chaque modèle nous disposons d'un **responsable point de contact** défini, identifiable et contactable simplement
- [ ] 5.1.d Pour chaque modèle, nous réalisons systématiquement une **évaluation des risques** consécutifs à d'éventuels incidents, défaillances ou biais
- [ ] 5.1.e Des outils de monitoring sont mis en place afin d'assurer une surveillance continue des systèmes de ML et peuvent déclencher des alertes directement auprès de l'équipe responsable
- [ ] 5.1.f Pour chaque modèle, nous définissons et testons une procédure de suspension du modèle et un mode de fonctionnement dégradé sans le modèle, pour parer au cas de figure où le modèle serait sujet à une défaillance ou un comportement anormal
- [ ] 5.1.g Pour chaque modèle, nous étudions sa généalogie de bout-en-bout (toutes les étapes et tous les choix qui ont conduit à son élaboration et son évaluation), ainsi que ses conditions et limites d'utilisation, pour comprendre le modèle avant de l'utiliser
- [ ] 5.1.h Nous utilisons toujours les modèles pour des **usages en adéquation avec leurs conditions et limites d'utilisation**

<details>
<summary>Expl5.1 :</summary>

Utiliser des systèmes automatiques basés sur des modèles dont les règles ont été "apprises" (et non définies et formalisées) interroge le fonctionnement des organisations. Il est important d'évaluer les conséquences et les réactions en cas d'incident. Par ailleurs il est important qu'une personne responsable soit clairement identifiée de manière à ne laisser aucune partie prenante démunie face à une conséquence inattendue ou inappropriée. Enfin il est important de s'interroger sur les "conditions et limites de validité" des modèles que l'on utilise afin de s'assurer que l'usage que l'on prévoit est bien en adéquation.

</details>

---

Q5.2 : **Développement de modèles prédictifs pour le compte de tiers**  
Si votre organisation fournit à ses clients ou à des tiers, ou opère pour le compte de tiers des applications basées sur des modèles prédictifs :

R5.2 :  
_(Type : réponses multiples possibles)_  
_(Sélectionner tous les éléments de réponse correspondant à des pratiques de votre organisation. Attention, certaines combinaisons ne seraient pas cohérentes)_

- [ ] 5.2.a Notre organisation ne fournit pas à ses clients ou des tiers, et n'opère pas pour le compte de tiers d'application basée sur des modèles prédictifs élaborés par apprentissage automatique | _(Concerné / Non concerné)_
- [ ] 5.2.b **Un registre des modèles prédictifs** identifie tous les modèles ou applications utilisés par ses clients et/ou par l'organisation pour le compte de tiers, nous le maintenons à jour
- [ ] 5.2.c Pour chaque modèle ou application pour un client ou un tiers nous disposons d'un **responsable point de contact** défini, identifiable et joignable simplement
- [ ] 5.2.d Pour chaque modèle ou application pour un client ou un tiers, nous réalisons systématiquement une **évaluation des risques** consécutifs à d'éventuels, incidents, défaillances, biais
- [ ] 5.2.e Des outils de monitoring sont mis en place afin d'assurer une surveillance continue des systèmes de ML et peuvent déclencher des alertes directement auprès de l'équipe responsable
- [ ] 5.2.f Pour chaque modèle ou application pour un client ou un tiers, nous définissons et testons une procédure de suspension du modèle et un mode de fonctionnement dégradé sans le modèle, pour parer au cas de figure où le modèle serait sujet à une défaillance ou un comportement anormal
- [ ] 5.2.g Pour chaque modèle ou application pour un client ou un tiers, nous étudions sa généalogie de bout-en-bout et ses conditions et limites d'utilisation pour comprendre le modèle avant de l'utiliser
- [ ] 5.2.h Nous fournissons à nos clients ou opérons pour leur compte des modèles ou applications pour des **usages en adéquation avec leurs conditions et limites d'utilisation**

<details>
<summary>Expl5.2 :</summary>

Utiliser des systèmes automatiques basés sur des modèles dont les règles ont été "apprises" (et non définies et formalisées) interroge le fonctionnement des organisations. Il est important d'évaluer les conséquences et les réactions en cas d'incident. Par ailleurs il est important qu'une personne responsable soit clairement identifiée de manière à ne laisser aucune partie prenante démunie face à une conséquence inattendue ou inappropriée. Enfin il est important de s'interroger sur les "conditions et limites de validité" des modèles que l'on utilise afin de s'assurer que l'usage que l'on prévoit est bien en adéquation.

</details>

---

Q5.3 : **Gestion des prédictions problématiques, processus de contournement, _human agency_**  
Les systèmes automatiques, en particulier lorsqu'ils s'appuient sur des modèles prédictifs appris, sont utilisés en production généralement pour gagner en efficacité. Il se trouve que par nature, ils génèrent de temps en temps des résultats non souhaitables pour l'organisation et ses parties prenantes (e.g. prédiction erronée), puisqu'ils ne généraliseront jamais une performance de 100%.

R5.3 :  
_(Type : réponse unique)_  
_(Sélectionner une seule réponse, correspondant le mieux au niveau de maturité de l'organisation sur ce sujet)_

- [ ] 5.3.a Notre organisation n'utilise pas de modèles prédictifs élaboré par apprentissage automatique pour son propre compte ou celui de ses clients, et ne fournit pas à ses clients d'application basée sur des modèles prédictifs | _(Concerné / Non concerné)_
- [ ] 5.3.b Nous implémentons des modèles prédictifs élaborés par apprentissage automatique dans des systèmes automatiques intégrés, sans mécanismes permettant de pallier à ou d'éviter des résultats non souhaitables dûs aux prédictions des modèles
- [ ] 5.3.c Nous intégrons dans les systèmes automatiques s'appuyant sur des modèles prédictifs les fonctionnalités permettant de gérer ces cas de résultats non souhaitables. Pour ces cas de figure, nous mettons en place des mécanismes permettant à un opérateur humain d'aller contre une décision automatique pour gérer de tels résultats non souhaitables ou incidents
- [ ] 5.3.d En complément des mécanismes de gestion d'incident, dans les systèmes automatiques s'appuyant sur des modèles prédictifs, lorsque l'intervalle de confiance pour la décision automatique n'est pas satisfaisant un opérateur humain est sollicité
- [ ] 5.3.e Nous appliquons systématiquement le principe de *human agency*, les sorties des modèles prédictifs que nous mettons en oeuvre sont utilisées par des opérateurs humains, et ne servent pas de déterminants à des décisions automatiques

<details>
<summary>Expl5.3 :</summary>

Utiliser des systèmes automatiques basés sur des modèles dont les règles ont été "apprises" (et non définies et formalisées) interroge le fonctionnement des organisations. Il est important de préserver la capacité de réaction et la résilience de l'organisation.

</details>

<details>
<summary>Ressources5.3 :</summary>

- (Technical guide) *[Monitoring Machine Learning Models in Production - A comprehensive guide](https://christophergs.com/machine%20learning/2020/03/14/how-to-monitor-machine-learning-models/)*, Christopher Samiullah, March 2020

</details>

---

Q5.4 : **Explicabilité et interprétabilité**  
Au sein des projets de data science qui visent à élaborer des modèles prédictifs :

R5.4 :  
_(Type : réponses multiples possibles)_  
_(Sélectionner tous les éléments de réponse correspondant à des pratiques de votre organisation. Attention, certaines combinaisons ne seraient pas cohérentes)_

- [ ] 5.4.a Notre organisation n'est pour l'instant pas familière avec les méthodes et outils d'explicabilité et d'interprétabilité des modèles
- [ ] 5.4.b Nous nous intéressons au sujet de l'explicabilité et l'interprétabilité des modèles et dialoguons avec nos parties prenantes sur ce sujet
- [ ] 5.4.c Nous faisons en sorte que les modèles que nous élaborons fournissent lorsque cela est pertinent a minima un niveau de confiance avec chaque prédiction réalisée
- [ ] 5.4.d Nous déterminons le meilleur compromis entre la performance et l'interprétabilité pour chaque modèle que nous élaborons, ce qui nous amène parfois à opter pour un modèle plus simple à expliquer aux personnes concernées (un modèle performant permettra de diminuer les risques d’erreur tandis qu’un modèle interprétable permettra de mieux justifier les résultats du modèle)
- [ ] 5.4.e Nous maîtrisons et mettons en oeuvre des approches avancées pour l'explicabilité et l'interprétabilité des modèles

<details>
<summary>Expl5.4 :</summary>

L'explicabilité et l'interprétabilité sont des enjeux-clés, en lien avec les exigences croissantes de transparence, d'impartialité et de responsabilité. Dans certains cas, la réglementation impose même de pouvoir expliquer aux personnes concernées comment fonctionne un algorithme.
Des ressources techniques comme SHAP ou LIME permettent d'entrer de plain-pied dans le sujet (voir les ressources associées à cet élément d'évaluation).

</details>

<details>
<summary>Ressources5.4 :</summary>

- (Web article) *[La confiance des utilisateurs dans les systèmes impliquant de l’Intelligence Artificielle](https://blog.octo.com/la-confiance-des-utilisateurs-dans-les-systemes-impliquant-de-lintelligence-artificielle/)*, Blog Octo Technologies, Octobre 2019
- (Technical guide) *[Interpretable Machine Learning, A Guide for Making Black Box Models Explainable](https://christophm.github.io/interpretable-ml-book/)*, Christoph Molnar
- (Web article) *[Understanding model predictions with LIME](https://towardsdatascience.com/understanding-model-predictions-with-lime-a582fdff3a3b)*, blog L. Hulstaert, 2018
- (Software & Tools) *[SHAP](https://github.com/slundberg/shap): A game theoretic approach to explain the output of any machine learning model*
- (Web article) Dans certains cas la réglementation impose de pouvoir expliquer aux personnes concernées comment fonctionne un algorithme (voir par exemple [l'article 22 du RGPD](https://www.cnil.fr/fr/reglement-europeen-protection-donnees/chapitre3#Article22), [l'article 10 de la loi Informatique et libertés](https://www.legifrance.gouv.fr/affichTexteArticle.do;?idArticle=LEGIARTI000037090394&cidTexte=LEGITEXT000006068624&dateTexte=20180624), cités notamment dans le [Serment d'Hippocrate pour data scientist](https://hippocrate.tech/))

</details>

---

Q5.5 : **Transparence vis-à-vis des parties prenantes interagissant avec un modèle prédictif appris**  
Votre organisation utilise pour son propre compte, fournit à ses clients ou opère pour le compte de ses clients des applications basées sur des modèles prédictifs, avec lesquels sont à même d'interagir des utilisateurs. Que met-elle en place pour en informer les utilisateurs ?

R5.5 :  
_(Type : réponses multiples possibles)_  
_(Sélectionner tous les éléments de réponse correspondant à des pratiques de votre organisation. Attention, certaines combinaisons ne seraient pas cohérentes)_

- [ ] 5.5.a Notre organisation n'utilise pas de modèles prédictifs élaborés par apprentissage automatique pour son propre compte ou celui de ses clients, et ne fournit pas à ses clients d'application basée sur des modèles prédictifs | _(Concerné / Non concerné)_
- [ ] 5.5.b Les utilisateurs ne sont pas informés qu'ils interagissent avec un modèle prédictif appris
- [ ] 5.5.c Une notice d'information est mise à disposition dans les conditions générales d'utilisation du système ou un document équivalent, en libre accès
- [ ] 5.5.d Le système ou le service est explicite vis-à-vis de l'utilisateur quant au fait qu'un modèle prédictif appris est utilisé
- [ ] 5.5.e Le système ou le service propose à l'utilisateur des informations supplémentaires sur les résultats qu'aurait fourni le système ou le service dans des cas de figure légèrement différents

<details>
<summary>Expl5.5 :</summary>

Utiliser des systèmes automatiques basés sur des modèles dont les règles ont été "apprises" (et non définies et formalisées) interroge le fonctionnement des organisations mais également le rapport des utilisateurs aux systèmes et services numériques. Dans la plupart des cas il est important d'informer les utilisateurs qu'ils ne font pas face à des règles de gestion classiques.

</details>

<details>
<summary>Ressources5.5 :</summary>

- (Academic paper) *[Counterfactual Explanations without Opening the Black Box: Automated Decisions and the GDPR](https://arxiv.org/abs/1711.00399)*, S. Wachter, B. Mittelstadt, C. Russell, 2018
- (Technical guide) *[Interpretable Machine Learning - Counterfactual explanations](https://christophm.github.io/interpretable-ml-book/counterfactual.html)*, C. Molnar, 2020

</details>

---
---

### Section 6 - Anticiper, suivre et minimiser les externalités négatives de l'activité data science

La mise en place d'un système automatique basé sur un modèle prédictif peut générer des externalités négatives sociales et environnementales. En prendre conscience est indispensable, ainsi qu'anticiper, chercher à suivre et minimiser les différents impacts négatifs.

[_[⇧ retour à la liste des sections](#référentiel-dévaluation-de-la-maturité-dune-organisation)_]

---

Q6.1 : **Impact CO2**  
Au sujet de l'impact CO2 de son activité data science, au sein de votre organisation :

R6.1 :  
_(Type : réponse unique)_  
_(Sélectionner une seule réponse, correspondant le mieux au niveau de maturité de l'organisation sur ce sujet)_

- [ ] 6.1.a À ce stade nous ne nous sommes pas penchés sur l'impact CO2 de notre activité data science ou de nos modèles prédictifs
- [ ] 6.1.b Nous avons défini des indicateurs pour savoir quoi mesurer précisément
- [ ] 6.1.c Nous avons défini des indicateurs et nous incluons leurs mesures dans les généalogies de bout-en-bout des modèles
- [ ] 6.1.d Nous avons défini des indicateurs et nous les suivons régulièrement
- [ ] 6.1.e Nous avons défini des indicateurs, nous les suivons régulièrement, et nous nous sommes fixés des objectifs d'amélioration

<details>
<summary>Expl6.1 :</summary>

Il est important de s'interroger et de conscientiser les coûts environnementaux.

</details>

<details>
<summary>Ressources6.1 :</summary>

- (Software & Tools) *[ML Impact Calculator](https://mlco2.github.io/impact/)*

</details>

---

Q6.2 : **Impact social**  
Dans certains cas, la mise en place d'un système automatique basé sur un modèle prédictif peut générer des externalités négatives sur les parties prenantes amont (par exemple annotation de données), et sur les parties prenantes aval (par exemple automatisation de certains postes). Lors de chaque projet d'élaboration ou d'utilisation d'un modèle prédictif, votre organisation :

R6.2 :  
_(Type : réponse unique)_  
_(Sélectionner une seule réponse, correspondant le mieux au niveau de maturité de l'organisation sur ce sujet)_

- [ ] 6.2.a À ce stade nous ne nous penchons pas sur l'impact social de notre activité data science ou de nos modèles prédictifs
- [ ] 6.2.b Dans certains cas nous nous interrogeons sur l'impact social
- [ ] 6.2.c Nous menons ce travail de réflexion sur l'impact social à chaque projet
- [ ] 6.2.d Nous menons ce travail de réflexion sur l'impact social à chaque projet et l'impact social est documenté dans la généalogie de bout-en-bout de chaque modèle
- [ ] 6.2.e Nous menons ce travail de réflexion sur l'impact social à chaque projet, l'impact social est documenté dans la généalogie de bout-en-bout de chaque modèle, et nous entamons systématiquement un dialogue avec les parties prenantes concernées amont et aval

<details>
<summary>Expl6.2 :</summary>

Il est important de s'interroger et d'échanger avec ses parties prenantes. Cela vaut tant pour l'aval (e.g. automatisation de certains emplois) que pour l'amont (e.g. tâches d'annotations de données parfois d'une très grande violence).

</details>

---

Q6.3 : **Ethique et non-malfaisance**  
Au sein de votre organisation :

R6.3 :  
_(Type : réponses multiples possibles)_  
_(Sélectionner tous les éléments de réponse correspondant à des pratiques de votre organisation. Attention, certaines combinaisons ne seraient pas cohérentes)_

- [ ] 6.3.a À ce stade nous ne nous sommes pas encore penchés sur la dimension éthique
- [ ] 6.3.b Les collaborateurs concernés par les activités data science reçoivent une formation à l'éthique
- [ ] 6.3.c Notre organisation s'est dotée d'une politique en matière d'éthique
- [ ] 6.3.d Sur les projets le justifiant, nous mettons en place un comité d'éthique indépendant ou nous sollicitons l'évaluation d'un organisme validant l'éthique des projets

<details>
<summary>Expl6.3 :</summary>

Travailler sur de grands volumes de données dont certaines peuvent être sensibles, utiliser des systèmes automatiques basés sur des modèles dont les règles ont été "apprises" (et non définies et formalisées) interrogent le fonctionnement des organisations et la responsabilité individuelle de chacun, impose d'avoir une réflexion sur l'usage qui en est fait. Il est donc important que l'organisation s'assure que les enjeux éthiques ne soient pas inconnus de son personnel.
Un exemple qui revient : certains systèmes ou services d'IA conçus pour s'adapter au comportement des utilisateurs peuvent influencer ceux-ci (par exemple en cherchant à maximiser leurs temps d'utilisation ou les sommes qu'ils dépensent) et présenter des risques non négligeables de manipulation ou d'addiction.

</details>

<details>
<summary>Ressources6.3 :</summary>

- (Official report) Rapport *[Éthique et responsabilité des algorithmes publics](https://www.etalab.gouv.fr/wp-content/uploads/2020/01/Rapport-ENA-Ethique-et-responsabilit%C3%A9-des-algorithmes-publics.pdf)*, Etalab / ENA, Janvier 2020
- (Public declaration) *[Déclaration de Montréal pour l'IA responsable](https://www.declarationmontreal-iaresponsable.com/la-declaration)*
- (Public declaration) *[Serment Holberton-Turing](https://www.holbertonturingoath.org/accueil)*
- (Public declaration) *[Serment d'Hippocrate pour data scientist](https://hippocrate.tech/)*
- (Public declaration) *[Future of Life's AI principles](https://futureoflife.org/ai-principles/)*
- (Public declaration) *[Charte internationale pour une IA inclusive](https://charteia.arborus.org/)*, Arborus et Orange
- (Course) *[Practical data ethics](https://ethics.fast.ai/)*, fast.ai : un excellent cours en ligne combinant listes de lectures et vidéos didactiques

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
