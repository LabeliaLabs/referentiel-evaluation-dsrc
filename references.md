# Références

## Liste de lecture

- Fairness :

  - [Machine Learning in the wild](https://www.oreilly.com/radar/machine-learning-in-the-wild/) : en particulier sur le sujet _fairness_

  - [Building Fair and Transparent Machine Learning via Operationalized Risk Management](https://aiforsocialgood.github.io/icml2019/accepted/track2/pdfs/32_aisg_icml2019.pdf) de Quantum Black : approche analyse de risque très détaillée, à suivre courant 2020 si publication de leur plateforme de risques

  - [Biased Algorithms are Easier to Fix than Biased People](https://www.nytimes.com/2019/12/06/business/algorithm-bias-fix.html)

  - Word Embedding and gender bias:
    - [Word embeddings quantify 100 years of gender and ethnic stereotypes](https://www.pnas.org/content/pnas/115/16/E3635.full.pdf)
    - [Christine Basta, Marta R. Costa-juss`a, Noe Casas. Evaluating the Underlying Gender Bias in Contextualized Word Embeddings, 2018](https://arxiv.org/pdf/1904.08783.pdf)
    - [Invisible Women: Exposing Data Bias in a World Designed for Men, Caroline Criado Perez](https://www.theguardian.com/books/2019/feb/28/invisible-women-by-caroline-criado-perez-review)

- AI safety:
  
  - [A Roadmap for Robust End-to-End Alignment](https://arxiv.org/pdf/1809.01036.pdf), Lê Nguyên Hoang, EPFL : "_AI alignment problem. This is the problem of aligning an AI’s objective function with human preferences._"

  - [Concrete problems in AI safety](https://arxiv.org/abs/1606.06565). Abstract: _"[...] the problem of accidents in machine learning systems, defined as unintended and harmful behavior that may emerge from poor design of real-world AI systems. We present a list of five practical research problems related to accident risk, categorized according to whether the problem originates from having the wrong objective function ("avoiding side effects" and "avoiding reward hacking"), an objective function that is too expensive to evaluate frequently ("scalable supervision"), or undesirable behavior during the learning process ("safe exploration" and "distributional shift"). [...]"_

- Trust in AI systems, explicabilité et interprétabilité:

  - *[La confiance des utilisateurs dans les systèmes impliquant de l’Intelligence Artificielle](https://blog.octo.com/la-confiance-des-utilisateurs-dans-les-systemes-impliquant-de-lintelligence-artificielle/)*, blog Octo Technologies, octobre 2019

  - *[Interpretable Machine Learning, A Guide for Making Black Box Models Explainable](https://christophm.github.io/interpretable-ml-book/)*, Christoph Molnar

- Protection of data confidentiality:

  - *[The secret-sharer: evaluating and testing unintended memorization in neural networks](https://blog.acolyer.org/2019/09/23/the-secret-sharer/)*, A. Colyer, 2019

  - *[Membership Inference Attacks against Machine Learning Models](https://arxiv.org/abs/1610.05820)*, R. Shokri, M. Stronati, C. Song, V. Shmatikov, 2017 and further analysis *[Demystifying the membership inference attack](https://medium.com/disaitek/demystifying-the-membership-inference-attack-e33e510a0c39)*, Disaitek, 2019. A tool called [ML Privacy Meter](https://github.com/privacytrustlab/ml_privacy_meter) to quantify the privacy risks of machine learning models with respect to inference attacks is also available

  - Outils pour la *differential privacy* : Google [differential privacy library](https://github.com/google/differential-privacy) and its Python wrapper [PyDP](https://github.com/OpenMined/PyDP) by OpenMined

  - La *distillation* d'un modèle, en plus de la compression qu'elle apporte, peut être utilisée comme une mesure de protection du modèle et des données d'entraînement utilisées, voir par exemple *[Knowledge Distillation : Simplified](https://towardsdatascience.com/knowledge-distillation-simplified-dd4973dbc764)*, Towards Data Science, 2019, et *[Distilling the Knowledge in a Neural Network](https://arxiv.org/abs/1503.02531)*, G. Hinton, O. Vinyals, J. Dean, 2015

  - *[The FTC’s new enforcement weapon spells death for algorithms](https://www.protocol.com/policy/ftc-algorithm-destroy-data-privacy)*, Protocol Policy, 2022

- Cycle de vie complet :

  - *[En route vers le cycle de vie des modèles !](https://www.quantmetry.com/blog/premier-etape-cycle-vie-modeles/)*, G. Martinon, Janvier 2020

- "Performance is not outcome", erreurs, crises :

  - *[Google’s medical AI was super accurate in a lab. Real life was a different story](https://www.technologyreview.com/2020/04/27/1000658/google-medical-ai-accurate-lab-real-life-clinic-covid-diabetes-retina-disease/)*, MIT Technology Review

  - *[Hundreds of AI tools have been built to catch covid. None of them helped](https://www.technologyreview.com/2021/07/30/1030329/machine-learning-ai-failed-covid-hospital-diagnosis-pandemic)*, MIT Technology Review, July 2021

- Various scandals and or controversies:

  - [Awful AI](https://github.com/daviddao/awful-ai): a curated list to track current scary usages of AI - hoping to raise awareness to its misuses in society, David Dao
  
  - [South Wales police lose landmark facial recognition case](https://www.theguardian.com/technology/2020/aug/11/south-wales-police-lose-landmark-facial-recognition-case)

  - [An AI hiring firm says it can predict job hopping based on your interviews](https://www.technologyreview.com/2020/07/24/1005602/ai-hiring-promises-bias-free-job-hopping-prediction/): *The idea of “bias-free” hiring, already highly misleading, is being used by companies to shirk greater scrutiny for their tools’ labor issues beyond discrimination*, MIT Technology Review, July 2020

  - [Faulty Facial Recognition Led to His Arrest—Now He’s Suing](https://www.vice.com/en_us/article/bv8k8a/faulty-facial-recognition-led-to-his-arrestnow-hes-suing), Septembre 2020, vice.com

  - [Argentina: Child Suspects’ Private Data Published Online](https://www.hrw.org/news/2020/10/09/argentina-child-suspects-private-data-published-online) - Facial Recognition System Uses Flawed Data, Poses Further Risks to Children

  - [Minneapolis prohibits use of facial recognition software by its police department](https://www.theverge.com/2021/2/13/22281523/minneapolis-prohibits-facial-recognition-software-police-privacy)

## Travaux dans ce domaine

L'*[Institute for Ethical AI & Machine Learning](https://ethical.institute)* maintient un panorama très complet des initiatives réglementaires, rapports, guidelines, frameworks divers et variés en lien avec la pratique et l'usage de l'IA et la data science : voir leur repository [Awesome AI Guidelines](https://github.com/EthicalML/awesome-artificial-intelligence-guidelines#online-courses-and-learning-resources) sur Github.

### Méta-études

- Méta-étude *[The Ethics of AI Ethics: An Evaluation of Guidelines](https://link.springer.com/content/pdf/10.1007/s11023-020-09517-8.pdf)*, T. Hagendorff, Octobre 2019

- Méta-étude *[The global landscape of AI ethics guidelines](https://arxiv.org/ftp/arxiv/papers/1906/1906.11668.pdf)*, A. Jobin, M. Ienca, E. Vayena, Juin 2019

- Méta-étude *[A Unified Framework of Five Principles for AI in Society](https://hdsr.mitpress.mit.edu/pub/l0jsh9d1/release/6)*, F. Floridi, J. Cowls, Juillet 2019

- Méta-étude *[Principled Artificial Intelligence](https://cyber.harvard.edu/publication/2020/principled-ai)*, Berkman Klein Center, Février 2020 

### Guidelines, liste de principes ou de thèmes-clés

- [UNESCO - Recommendation on the ethics of artificial intelligence](https://unesdoc.unesco.org/ark:/48223/pf0000373434_fre):

    > - *La  présente  Recommandation  a  pour  objet  de  formuler  des  valeurs  et  des  principes  éthiques ainsi que des recommandations concrètes concernant la recherche, la conception, le développement, le déploiement et l’utilisation de l’IA, en vue de mettre les systèmes d’IA au service de l’humanité, des individus, des sociétés et de l’environnement.*
    > - Current status is draft, with an open public consultation in progress (as of August 2020)

- [EU Draft Ethics guidelines for trustworthy AI](https://ec.europa.eu/digital-single-market/en/news/draft-ethics-guidelines-trustworthy-ai) and [pilot assessment survey](https://ec.europa.eu/futurium/en/ethics-guidelines-trustworthy-ai/register-piloting-process-0)

    > 7 Key requirements:
    >
    > - Human agency and oversight
    > - Technical robustness and safety
    > - Privacy and data governance
    > - Transparency
    > - Diversity, non-discrimination and fairness
    > - Societal and environmental well-being
    > - Accountability

- [OECD AI Principles](https://www.oecd.org/going-digital/ai/principles/) focused on 'Responsible stewardship of trustworthy AI'

    > The Recommendation identifies five complementary values-based principles for the responsible stewardship of trustworthy AI:
    >
    > - AI should benefit people and the planet by driving inclusive growth, sustainable development and well-being.
    > - AI systems should be designed in a way that respects the rule of law, human rights, democratic values and diversity, and they should include appropriate safeguards – for example, enabling human intervention where necessary – to ensure a fair and just society.
    > - There should be transparency and responsible disclosure around AI systems to ensure that people understand AI-based outcomes and can challenge them.
    > - AI systems must function in a robust, secure and safe way throughout their life cycles and potential risks should be continually assessed and managed.
    > - Organisations and individuals developing, deploying or operating AI systems should be held accountable for their proper functioning in line with the above principles.

- The Institute for Ethical AI & Machine Learning: [Awesome AI guidelines](https://github.com/ethicalml/awesome-artificial-intelligence-guidelines) and [The Responsible ML Principles](https://ethical.institute/principles.html):

    > The Responsible Machine Learning Principles:
    >
    >   1. **Human augmentation**: I commit to assess the impact of incorrect predictions and, when reasonable, design systems with human-in-the-loop review processes
    >   1. **Bias evaluation**: I commit to continuously develop processes that allow me to understand, document and monitor bias in development and production.
    >   1. **Explainability by justification**: I commit to develop tools and processes to continuously improve transparency and explainability of machine learning systems where reasonable.
    >   1. **Reproducible operations**: I commit to develop the infrastructure required to enable for a reasonable level of reproducibility across the operations of ML systems.
    >   1. **Displacement strategy**: I commit to identify and document relevant information so that business change processes can be developed to mitigate the impact towards workers being automated.
    >   1. **Practical accuracy**: I commit to develop processes to ensure my accuracy and cost metric functions are aligned to the domain-specific applications.
    >   1. **Trust by privacy**: I commit to build and communicate processes that protect and handle data with stakeholders that may interact with the system directly and/or indirectly.
    >   1. **Data risk awareness**: I commit to develop and improve reasonable processes and infrastructure to ensure data and model security are being taken into consideration during the development of machine learning systems.

- [PWC IA responsable](https://www.pwc.fr/fr/vos-enjeux/data-intelligence/intelligence-artificielle/intelligence-artificielle-responsable.html):

    > 6 thèmes :
    >
    > - Renforcer la sécurité de l'IA avec validation, surveillance et vérification
    > - Créer des modèles d'IA transparents, extensibles et prouvables
    > - Créer des systèmes éthiques, compréhensibles, légaux
    > - Améliorer la gouvernance avec des modèles d'exploitation et des processus de l'IA
    > - Tester le biais dans les données, les modèles et l'utilisation d'algorithmes par l'homme

- [Google recommended practices for AI: Fairness, Interpretability, Privacy, Security](https://ai.google/education/responsible-ai-practices)

### Déclarations, chartes, serments

- [Déclaration de Montréal pour l'IA responsable](https://www.declarationmontreal-iaresponsable.com/la-declaration)
- [Serment Holberton-Turing](https://www.holbertonturingoath.org/accueil)
- [Serment d'Hippocrate pour data scientist](https://hippocrate.tech/)
- [Future of Life's AI principles](https://futureoflife.org/ai-principles/)
- [Charte internationale pour une IA inclusive](https://charteia.arborus.org/), Arborus
- [Manifeste pour des IA éthiques](http://ai-ethical.com/131-2/), Numeum, 2021

### Assessments et référentiels

- ADEL - [Label éthique pour l'exploitation du big data](http://www.adel-label.com/)
- ALTAI - [The Assessment List on Trustworthy Artificial Intelligence](https://altai.insight-centre.org/)
- Occitanie Data / Ekitia - [Charte éthique de l'usage des données](https://www.occitaniedata.fr/la-charte-ethique/)
- LNE - [Référentiel certification de processus pour l'intelligence artificielle](https://www.lne.fr/fr/service/certification/certification-processus-ia), 2021

### Autres

- [Guide pratique pour des IA éthiques](http://ai-ethical.com/guide-pratique/), Numeum, 2021
- [Livre blanc Data Responsable](http://www.utopies.com/fr/initiatives/groupe-de-travail-data-responsable), Utopies & Imaginable For Good
- [Responsible AI Licenses](https://www.licenses.ai/)
- [FAT ML](https://www.fatml.org/) : _semble inactif depuis fin 2018_
- [AI for social good workshops](https://aiforsocialgood.github.io/neurips2019/) and research papers
- [Building Fair and Transparent Machine Learning via Operationalized Risk
Management: Towards an Open-Access Standard Protocol](https://aiforsocialgood.github.io/icml2019/accepted/track2/pdfs/32_aisg_icml2019.pdf)
- Algorithmes publics :
  - [Guide des algorithmes publics à l'usage des administrations](https://guides.etalab.gouv.fr/algorithmes/guide/), Etalab
  - Rapport [Éthique et responsabilité des algorithmes publics](https://www.etalab.gouv.fr/wp-content/uploads/2020/01/Rapport-ENA-Ethique-et-responsabilit%C3%A9-des-algorithmes-publics.pdf), Etalab / ENA, Janvier 2020
- [ISO](https://blog.iec.ch/2019/11/international-standards-committee-on-ai-ecosystem-achieves-milestone-and-launches-new-areas-of-study/) est en train de définir des normes dans le secteur de l'Intelligence Artificielle. Ces travaux devront être suivis
- Rapport [Ethics and Algorithms toolkit](https://ethicstoolkit.ai/)
- Rapport [AI Now Report 2019](https://ainowinstitute.org/AI_Now_2019_Report.pdf)

## Notes et observations

- Beaucoup de travaux s'intéressent à l'éthique par les usages et par la non-reproduction de discrimination
- On trouve en revanche peu de choses sur le cycle de vie de l'élaboration d'un modèle (voir par exemple le [papier de Quantum Black](https://aiforsocialgood.github.io/icml2019/accepted/track2/pdfs/32_aisg_icml2019.pdf))
- Le plus complet est peut-être le questionnaire d'évaluation de l'UE, mais il est loin d'être actionnable, opérationnel (63 questions dont de nombreuses sont des questions très ouvertes), et son processus d'élaboration et d'évolution est relativement fermé
- Des référentiels de la sécurité des systèmes d'information, bien plus généraux, pourraient être utilisés comme références pour éviter d'être redondant sur certains points. Par exemple le [guide de la sécurité des données personnelles](https://www.cnil.fr/fr/principes-cles/guide-de-la-securite-des-donnees-personnelles) de la CNIL.
