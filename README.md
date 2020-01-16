# Comment définir la data science responsable et de confiance ?

**Navigation** :

`/`  
`├── README.md`
- [Contexte, motivations et ambition](#contexte-motivations-et-ambition)
- [Approche participative](#approche-participative)
- [Périmètres](#périmètres-cible-et-hors-cible)
- [Travaux dans ce domaine](#travaux-dans-ce-domaine)

`├── referentiel.md`
- [Risques](./referentiel.md#risques)
- [Propositions de thèmes, d'un canevas du référentiel](./referentiel.md#propositions-de-thèmes-dun-canevas-du-référentiel)

`├── methode.md`
- [Approche](./methode.md#approche-et-méthode-de-consensus)
- [Consensus au sein du groupe de travail](./methode.md#consensus-au-sein-du-groupe-de-travail)
- [Travaux asynchrones](./methode.md#travaux-asynchrones)
- [License](./methode.md#license)

## Contexte, motivations et ambition

Un nouvel espace émerge au croisement entre expansion de l'IA dans les organisations et les systèmes automatiques, et inquiétudes du public sur les données privées, la transparence et la robustesse des algorithmes.

Ce sont deux tendances puissantes qui commencent déjà à se percuter (voir par exemple [le cas Apple Card](https://twitter.com/dhh/status/1192540900393705474)). Comment les réconcilier, les conjuguer ensemble ? Des solutions techniques et organisationnelles nouvelles sont indispensables pour cela, pour accorder un cadre de confiance qui manque aujourd’hui, pour rendre possible des collaborations nouvelles, prometteuses et sûres entre les entreprises, les institutions publiques et les citoyens.

De nombreux acteurs s'emparent du sujet et travaillent par exemple déjà à des cadres pour un usage éthique et à impact positif des technologies d'IA, à des outils pour apporter de la traçabilité aux travaux de data science, à des formations pour éviter la reproduction de biais discriminatoires, à des briques techniques pour permettre la mutualisation et renforcer la confidentialité des données, etc.

En s'appuyant sur les travaux, cadres et corpus existants, nous proposons de travailler de manière ouverte et collaborative à la définition de ce que serait la **data science responsable et de confiance**. L'objectif ? Établir ensemble un référentiel open source de bonnes pratiques permettant aux organisations intéressées d'évaluer leur niveau de maturité

### Une initiative de plus ?

Pourquoi cette initiative, dans un univers qui voit déjà émerger un certain nombre de travaux ? Nous listons [ci-dessous](#travaux-dans-ce-domaine) les travaux que nous avons identifiés. Ils sont tous intéressants, inspirants, utiles. Beaucoup proposent des _guidelines_, des engagements à prendre, traitent de l'éthique de l'usage de technologies d'IA. Certains explorent des voies nouvelles : licences spécifiques à l'IA, plateforme d'analyse de risque... Mais à ce stade aucun ne nous a semblé couvrir complètement les points suivants :
- s'intéresser à l'activité data science d'une organisation (comme ensemble de pratiques, de processus, de méthodes...), au cycle de vie complet d'un modèle
- être fait pour être utilisé comme un outil concret d'évaluation de la maturité de l'organisation

Nous imaginons un référentiel qui soit actionnable, opérationnel, pour que cela puisse être utile le plus rapidement possible et, à l'usage, susciter des réflexions, des échanges, des souhaits d'amélioration. Qu'il puisse faciliter l'émergence d'offres d'évaluation, audit, formation dans ce domaine (sur le modèle de l'annexe A de la [norme ISO 27001](https://fr.wikipedia.org/wiki/ISO/CEI_27001) ou du label [B-Corp](https://bimpactassessment.net/) par exemple).  
Nous pensons que la communauté data science responsable et de confiance en France (et en Europe et au-delà) pourrait bénéficier d'un tel cadre commun. L'enjeu est de fournir des repères pour augmenter la lisibilité du sujet et de le faire connaître le plus largement possible, de faciliter la montée en maturité des organisations, les nouvelles collaborations entre prestataires spécialisés et grandes organisations... Il est aussi d'animer une dynamique d'échanges au sein de la communauté et d'amélioration continue du référentiel lui-même.

### Pourquoi _responsable_ et _de confiance_ ?

_Responsable_ : Qui se préoccupe des conséquences sur ses parties prenantes, cherche à avoir un impact positif, essaie d'éviter d'être _irresponsable_ c'est-à-dire ne pas maîtriser des conséquences préjudiciables pour ses parties prenantes.

_De confiance_ : Dans lequel on peut avoir un niveau de confiance raisonnable car les règles de l'art prévenant une large panoplie de risques typiques sont appliquées.

Les deux notions se recouvrent en partie. Il est cependant difficile de trouver un terme unique satisfaisant. La combinaison des deux apporte une richesse utile.

### Inspirations

- [Annexe A ISO 27001](https://fr.wikipedia.org/wiki/ISO/CEI_27001) : 114 mesures de sécurité classées en 14 catégories, dans le domaine des systèmes d'information
- [ITIL](https://fr.wikipedia.org/wiki/Information_Technology_Infrastructure_Library) : référentiel méthodologique sur l'organisation, l'efficacité, la réduction des risques, l'amélioration de la qualité des systèmes d'information
- B-Corp '[B Impact Assessment](https://bimpactassessment.net/)' : questionnaire gratuit et confidentiel d'évaluation de l'impact social et environnemental d'une organisation
- [Don en confiance](www.donenconfiance.org) : charte de déontologie et label dans le domaine du financement des associations et de l'appel public à la générosité

### Un référentiel de bonnes pratiques

- Référentiel de _bonnes pratiques_. Une bonne pratique est une pratique cible, une mesure qui peut ou non être mise en oeuvre. Par exemple voici une mesure dans le domaine des systèmes d'information et de l'évaluation ISO 27001 :
> _Des procédures de gestion des supports amovibles doivent être mises en œuvre conformément au plan de classification adopté par l’organisation._

- Chaque organisation met en oeuvre les mesures cibles à sa façon avec un certain _niveau de maturité_, qui peut évoluer dans le temps au fur et à mesure des progrès de l'organisation :

| Niveau d'implémentation | Note de maturité | Point de vue processus |
|---|:---:|---|
| Mesure non implémentée | 0 | Pratique inexistante ou incomplète |
| Mesure en cours d'implémentation | 1 | Pratique informelle |
| Mesure implémentée nécessitant amélioration | 2 | Pratique répétable et suivie |
| Mesure implémentée | 3 | Processus défini |
| Mesure implémentée et contrôlée | 4 | Processus contrôlé |
| Mesure implémentée, contrôlée et optimisée | 5 | Processus en amélioration continue |

## Approche participative

### Cycle d'ateliers de co-construction

Nous proposons de travailler de manière ouverte et collaborative et organisons un cycle d'ateliers de co-construction :

- Atelier #1 : mercredi 18 décembre 2019 à Paris
- Atelier #2 : jeudi 6 février 2020 à Paris
- Atelier #3 : jeudi 2 avril 2020 à Paris
- Atelier #4 : mardi 23 juin 2020
- Atelier #5 : mardi 8 septembre 2020
- Atelier #6 : mardi 10 novembre 2020
- Atelier #7 : mardi 15 décembre 2020

Curieux ? Enthousiaste ? Sceptique ? Essayons ensemble, avec toutes les bonnes énergies de celles et ceux qui sont intéressés par le sujet et la démarche, avec l’esprit ouvert à la possibilité que cette démarche puisse muter, rencontrer d’autres initiatives, peut-être ne pas aboutir… avec la certitude en revanche de débattre et d’apprendre sur des sujets passionnants.

### Responsabilité éditoriale, disponibilité en ligne des travaux et participation asynchrone

Ce travail est élaboré sous la responsabilité éditoriale de l'association à but non lucratif Substra Foundation, qui s'engage à le mettre à disposition de manière à ce qu'il puisse être librement reproduit et partagé.

Ainsi, le projet en ligne et le dépôt de fichiers associés, hébergés par Substra Foundation sur Github, assurent la disponibilité en ligne de ces travaux et du référentiel de la data science responsable et de confiance. Au-delà des ateliers participatifs bimestriels, il donc également possible de participer de manière asynchrone.

### Nature évolutive

Par nature cette démarche est en constante évolution. Il nous semble plus utile et plus transparent de mettre à disposition le référentiel dans son état du moment, plutôt que d'attendre le franchissement de jalons majeurs. Ainsi, chacun est en mesure d'en prendre connaissance et de participer par des questions ou des suggestions d'amélioration.
Une logique de versions ou de jalons sera proposée afin de fournir un repère temporel aux organisations utilisatrices.

### Mise à disposition

<a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-nd/4.0/88x31.png" /></a><br />Ce(tte) œuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/4.0/">Licence Creative Commons Attribution - Pas d&#39;Utilisation Commerciale - Pas de Modification 4.0 International</a>.

## Périmètres

- Un référentiel de pratiques qui s'adresse à qui ?
    - Cible principale : l'activité data science d'une organisation
    - Hors-cible : un projet donné, un produit donné, un modèle prédictif donné
    - Pourquoi ?
        - Les projets et produits peuvent prendre des formes extrêmement variées et il est donc très difficile d'être pertinent avec un référentiel générique
        - L'effort pour s'évaluer selon un référentiel peut être trop élevé s'il doit être fait projet par projet
        - Les mesures ou pratiques relatives aux collaborateurs (e.g. les formations) correspondent plus naturellement aux pratiques d'une organisation qu'à celle d'un projet donné
    - Idées d'élargissements possibles : des mesures plus ciblées visant un projet en particulier pourraient être étudiées.
- Que désigne-t-on par _IA_ et _data science_ ?
    - Cible : l'utilisation de techniques algorithmiques sur des données, ainsi que les modèles prédictifs et les systèmes automatiques en résultant. On prend ici une acception large des termes _IA_ et _data science_ (e.g on y inclut les systèmes experts).
    - Hors cible : les systèmes informatiques, la sécurité informatique, la gestion des bases de données en général (même si toutefois, en se concentrant sur l'activité data science d'une organisation, des sujets de sécurité et de gestion des données émergeront naturellement).

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
