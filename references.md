# Liste de lecture, références, travaux dans ce domaine

## Références

- Fairness :

    - [Machine Learning in the wild](https://www.oreilly.com/radar/machine-learning-in-the-wild/) : en particulier sur le sujet _fairness_

    - [Building Fair and Transparent Machine Learning via Operationalized Risk Management](https://aiforsocialgood.github.io/icml2019/accepted/track2/pdfs/32_aisg_icml2019.pdf) de Quantum Black : approche analyse de risque très détaillée, à suivre courant 2020 si publication de leur plateforme de risques

    - [Biased Algorithms are Easier to Fix than Biased People](https://www.nytimes.com/2019/12/06/business/algorithm-bias-fix.html)

- [A Roadmap for Robust End-to-End Alignment](https://arxiv.org/pdf/1809.01036.pdf), Lê Nguyên Hoang, EPFL : "_AI alignment problem. This
is the problem of aligning an AI’s objective function with human preferences._"

- Protection of data confidentiality:

    - [The secret-sharer: evaluating and testing unintended memorization in neural networks](https://blog.acolyer.org/2019/09/23/the-secret-sharer/)


- Word Embedding and gender bias:

    - [Word embeddings quantify 100 years of gender and ethnic stereotypes](https://www.pnas.org/content/pnas/115/16/E3635.full.pdf)

    - [Christine Basta, Marta R. Costa-juss`a, Noe Casas. Evaluating the Underlying Gender Bias in Contextualized Word Embeddings, 2018](https://arxiv.org/pdf/1904.08783.pdf)

- Algorithmes publics :

    - [Guide des algorithmes publics à l'usage des administrations](https://guides.etalab.gouv.fr/algorithmes/guide/), Etalab

    - Rapport [Éthique et responsabilité des algorithmes publics](https://www.etalab.gouv.fr/wp-content/uploads/2020/01/Rapport-ENA-Ethique-et-responsabilit%C3%A9-des-algorithmes-publics.pdf), Etalab / ENA, Janvier 2020

## Travaux dans ce domaine

- [EU Draft Ethics guidelines for trustworthy AI](https://ec.europa.eu/digital-single-market/en/news/draft-ethics-guidelines-trustworthy-ai) and [pilot assessment survey](https://ec.europa.eu/futurium/en/ethics-guidelines-trustworthy-ai/register-piloting-process-0)

    > 7 Key requirements:
    > - Human agency and oversight
    > - Technical robustness and safety
    > - Privacy and data governance
    > - Transparency
    > - Diversity, non-discrimination and fairness
    > - Societal and environmental well-being
    > - Accountability

- [OECD AI Principles](https://www.oecd.org/going-digital/ai/principles/) focused on 'Responsible stewardship of trustworthy AI'

    > The Recommendation identifies five complementary values-based principles for the responsible stewardship of trustworthy AI:
    > - AI should benefit people and the planet by driving inclusive growth, sustainable development and well-being.
    > - AI systems should be designed in a way that respects the rule of law, human rights, democratic values and diversity, and they should include appropriate safeguards – for example, enabling human intervention where necessary – to ensure a fair and just society.
    > - There should be transparency and responsible disclosure around AI systems to ensure that people understand AI-based outcomes and can challenge them.
    > - AI systems must function in a robust, secure and safe way throughout their life cycles and potential risks should be continually assessed and managed.
    > - Organisations and individuals developing, deploying or operating AI systems should be held accountable for their proper functioning in line with the above principles.

-  The Institute for Ethical AI & Machine Learning: [Awesome AI guidelines](https://github.com/ethicalml/awesome-artificial-intelligence-guidelines) and [The Responsible ML Principles](https://ethical.institute/principles.html):

    > The Responsible Machine Learning Principles:
    > 1. **Human augmentation**: I commit to assess the impact of incorrect predictions and, when reasonable, design systems with human-in-the-loop review processes
    > 1. **Bias evaluation**: I commit to continuously develop processes that allow me to understand, document and monitor bias in development and production.
    > 1. **Explainability by justification**: I commit to develop tools and processes to continuously improve transparency and explainability of machine learning systems where reasonable.
    > 1. **Reproducible operations**: I commit to develop the infrastructure required to enable for a reasonable level of reproducibility across the operations of ML systems.
    > 1. **Displacement strategy**: I commit to identify and document relevant information so that business change processes can be developed to mitigate the impact towards workers being automated.
    > 1. **Practical accuracy**: I commit to develop processes to ensure my accuracy and cost metric functions are aligned to the domain-specific applications.
    > 1. **Trust by privacy**: I commit to build and communicate processes that protect and handle data with stakeholders that may interact with the system directly and/or indirectly.
    > 1. **Data risk awareness**: I commit to develop and improve reasonable processes and infrastructure to ensure data and model security are being taken into consideration during the development of machine learning systems.

- [PWC IA responsable](https://www.pwc.fr/fr/vos-enjeux/data-intelligence/intelligence-artificielle/intelligence-artificielle-responsable.html):

    > 6 thèmes :
    > - Renforcer la sécurité de l'IA avec validation, surveillance et vérification
    > - Créer des modèles d'IA transparents, extensibles et prouvables
    > - Créer des systèmes éthiques, compréhensibles, légaux
    > - Améliorer la gouvernance avec des modèles d'exploitation et des processus de l'IA
    > - Tester le biais dans les données, les modèles et l'utilisation d'algorithmes par l'homme

- [Future of Life's AI principles](https://futureoflife.org/ai-principles/)
- [Google recommended practices for AI: Fairness, Interpretability, Privacy, Security](https://ai.google/education/responsible-ai-practices)
- [Déclaration de Montréal pour l'IA responsable](https://www.declarationmontreal-iaresponsable.com/la-declaration)
- [Serment Holberton-Turing](https://www.holbertonturingoath.org/accueil)
- [Serment d'Hippocrate pour data scientist](https://dataforgood.fr/projects/4_serment-hippocrate.html)
- [Livre blanc Data Responsable](http://www.utopies.com/fr/initiatives/groupe-de-travail-data-responsable)
- [Responsible AI Licenses](https://www.licenses.ai/)
- [Méta-étude 'The global landscape of AI ethics guidelines'](https://arxiv.org/ftp/arxiv/papers/1906/1906.11668.pdf)
- [FAT ML](https://www.fatml.org/) : _semble inactif depuis fin 2018_
- [AI for social good workshops](https://aiforsocialgood.github.io/neurips2019/) and research papers
- [Building Fair and Transparent Machine Learning via Operationalized Risk
Management: Towards an Open-Access Standard Protocol](https://aiforsocialgood.github.io/icml2019/accepted/track2/pdfs/32_aisg_icml2019.pdf)

Quelques observations :

- Beaucoup de travaux s'intéressent à l'éthique par les usages et par la non-reproduction de discrimination
- Il y a cependant très peu de choses sur comment un modèle est élaboré (voir le [papier de Quantum Black](https://aiforsocialgood.github.io/icml2019/accepted/track2/pdfs/32_aisg_icml2019.pdf))
- Le plus complet est peut-être le questionnaire d'évaluation de l'UE, mais il est loin d'être actionnable, opérationnel (63 questions dont de nombreuses sont des questions très ouvertes), et son processus d'élaboration et d'évolution est relativement fermé
- Des référentiels de la sécurité des systèmes d'information, bien plus généraux, pourraient être utilisés comme références pour éviter d'être redondant sur certains points. Par exemple le [guide de la sécurité des données personnelles](https://www.cnil.fr/fr/principes-cles/guide-de-la-securite-des-donnees-personnelles) de la CNIL.