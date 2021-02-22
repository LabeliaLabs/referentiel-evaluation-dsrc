# Data science responsable et de confiance - Référentiel d'évaluation

*Note: although kickstarted in French, this work has been translated in English and will be updated in both languages from January 2021 onwards. Follow [this link](./assessment_framework_eng.md) to access the assessment in English.*

## Navigation dans le repository

`/`  
[`├── README.md`](#contexte-motivations-et-ambition) : [Contexte, motivations et ambition](#contexte-motivations-et-ambition) | [Périmètre du référentiel d'évaluation](#périmètre-du-référentiel-dévaluation) | [Approche participative](#approche-participative)  
**[`├── referentiel_evaluation.md`](./referentiel_evaluation.md)** : **[Référentiel d'évaluation](./referentiel_evaluation.md#référentiel-dévaluation-de-la-maturité-dune-organisation)** | [Risques](./referentiel_evaluation.md#risques)  
[`├── methode.md`](./methode.md) : [Approche](./methode.md#approche-et-méthode-de-consensus) | [Consensus au sein du groupe de travail](./methode.md#consensus-au-sein-du-groupe-de-travail) | [Travaux asynchrones](./methode.md#travaux-asynchrones) | [License](./methode.md#license)  
[`├── references.md`](./references.md) : [Liste de lectures](./references.md#liste-de-lecture) | [Travaux dans ce domaine](./references.md#travaux-dans-ce-domaine)  

## Contexte, motivations et ambition

Un nouvel espace émerge au croisement entre expansion de l'IA dans les organisations et les systèmes automatiques, et inquiétudes du public sur les données privées, la transparence et la robustesse des algorithmes.

Ce sont deux tendances puissantes qui commencent déjà à se percuter (voir par exemple [le cas Apple Card](https://twitter.com/dhh/status/1192540900393705474) en novembre 2019 ou le formidable article du New York Times en février 2020, [An Algorithm that grants Freedom, or Takes it away](https://www.nytimes.com/2020/02/06/technology/predictive-algorithms-crime.html)). Comment les réconcilier, les conjuguer ensemble ? Des solutions techniques et organisationnelles nouvelles sont indispensables pour cela, pour accorder un cadre de confiance qui manque aujourd’hui, pour rendre possible des collaborations nouvelles, prometteuses et sûres entre les entreprises, les institutions publiques et les citoyens.

De nombreux acteurs s'emparent du sujet et travaillent par exemple déjà à des cadres pour un usage à impact positif des technologies d'IA, à des outils pour apporter de la traçabilité aux travaux de data science, à des formations pour éviter la reproduction de biais discriminatoires, à des briques techniques pour permettre la mutualisation et renforcer la confidentialité des données, etc.

En s'appuyant sur les travaux, cadres et corpus existants, **nous proposons de travailler de manière ouverte et collaborative** à la définition de ce que serait la **data science responsable et de confiance**. L'objectif ? **Établir ensemble un référentiel open source** de bonnes pratiques permettant aux organisations intéressées d'évaluer leur niveau de maturité.

### Une initiative de plus ?

Pourquoi cette initiative, dans un univers qui voit déjà émerger un certain nombre de travaux ? Nous tenons à jour [la liste des travaux](./references.md#travaux-dans-ce-domaine) que nous avons identifiés. Ils sont tous intéressants, inspirants, utiles. Beaucoup proposent des _guidelines_, des engagements à prendre, traitent de l'éthique de l'usage de technologies d'IA. Certains explorent des voies nouvelles : licences spécifiques aux modèles prédictifs, plateforme d'analyse de risque... Mais à ce stade aucun ne nous a semblé couvrir complètement les points suivants :

1. s'intéresser à **l'activité data science d'une organisation** (comme ensemble de pratiques, de processus, de méthodes...), au cycle de vie complet d'un modèle ;

1. être fait **pour être utilisé comme un outil concret d'évaluation** de la maturité de l'organisation.

Nous imaginons un référentiel qui soit actionnable, opérationnel, pour que cela puisse être utile le plus rapidement possible et, à l'usage, susciter des réflexions, des échanges, des souhaits d'amélioration. Qu'il puisse faciliter l'émergence d'offres d'évaluation, audit, formation dans ce domaine.  
Nous pensons que la communauté data science responsable et de confiance en France et en Europe pourrait bénéficier d'un tel cadre commun. L'enjeu est de fournir des repères pour augmenter la lisibilité du sujet et de le faire connaître le plus largement possible, de faciliter la montée en maturité des organisations, les nouvelles collaborations entre prestataires spécialisés et grandes organisations... L'enjeu est aussi d'animer une dynamique d'échanges au sein de la communauté et d'amélioration continue du référentiel lui-même.

### Pourquoi _responsable_ et _de confiance_, et pourquoi pas _éthique_ ?

Nous utilisons ici ces termes comme suit :

_Responsable_ : Qui se préoccupe des conséquences sur ses parties prenantes, cherche à avoir un impact positif, essaie d'éviter d'être _irresponsable_ c'est-à-dire ne pas maîtriser des conséquences préjudiciables pour ses parties prenantes.

_De confiance_ : Dans lequel on peut avoir un niveau de confiance raisonnable car les règles de l'art prévenant une large panoplie de risques typiques sont appliquées.

Les deux notions se recouvrent en partie. Il est cependant difficile de trouver un terme unique satisfaisant. La combinaison des deux apporte une richesse qui nous semble utile.

On considère ici la _data science_ comme une combinaison de techniques et d'outils. Dans ce contexte l'_éthique_ de la data science ou de l'intelligence artificielle ne nous semble pas être le meilleur angle pour aborder et étudier les questions et défis inhérents à la data science dans le but d'élaborer un référentiel opérationnel. L'angle éthique polarise la réflexion sur les usages de l'IA, et la fond dans celle de l'éthique de l'usage des technologies ou des capacités techniques de manière plus générale (voir par exemple [cet article de Tom Chatfield sur OneZero](https://onezero.medium.com/theres-no-such-thing-as-ethical-a-i-38891899261d)). Il s'agit cependant d'un excellent sujet de discussion et débat, la conversation est donc très ouverte en ce moment dans la communauté.

Par ailleurs, une [discussion est ouverte](https://github.com/SubstraFoundation/referentiel-ds-responsable-confiance/issues/23) sur ce sujet pour prolonger la réflexion.

## Périmètre du référentiel d'évaluation

### Un référentiel d'évaluation qui s'adresse à qui ?

- Cible principale : **l'activité data science d'une organisation**
- Hors-cible : un projet donné, un produit donné, un modèle prédictif donné
- Pourquoi ?
  - Les projets et produits peuvent prendre des formes extrêmement variées et il est donc très difficile d'être pertinent avec un référentiel générique
  - L'effort pour s'évaluer selon un référentiel peut être trop élevé s'il doit être fait projet par projet
  - Les mesures ou pratiques relatives aux collaborateurs (e.g. les formations) correspondent plus naturellement aux pratiques d'une organisation qu'à celle d'un projet donné
- Idées d'élargissements possibles : des mesures plus ciblées visant un projet en particulier pourraient être étudiées.

### Que désigne-t-on par _IA_ et _data science_ ?

- Cible : **les modèles prédictifs et les systèmes automatiques résultant de l'utilisation de techniques algorithmiques sur des données**. On prend ici une acception large des termes _IA_ et _data science_ (e.g on y inclut les systèmes experts).
- Hors cible : les systèmes informatiques, la sécurité informatique, la gestion des bases de données en général (même si toutefois, en se concentrant sur l'activité data science d'une organisation, des sujets de sécurité et de gestion des données émergeront naturellement).

## Approche participative

### Cycle d'ateliers d'échange et de co-construction

Nous proposons de travailler de manière ouverte et collaborative et organisons pour cela des ateliers d'échange et de co-construction :

#### Saison 1

- Atelier #1 : mercredi 18 décembre 2019 à la Maison du Libre et des Communs (Paris) - [notes de l'atelier](./workshops-notes/2019.12.18_workshop-1_notes.md)
- Atelier #2 : jeudi 6 février 2020 à la Maison du Libre et des Communs (Paris) - [notes de l'atelier](./workshops-notes/2020.02.06_workshop-2_notes.md)
- Atelier #3 : jeudi 2 avril 2020 par téléconférence - [notes de l'atelier](./workshops-notes/2020.04.02_workshop-3_notes.md)
- Atelier #4 : mardi 23 juin 2020 par téléconférence - [notes de l'atelier](./workshops-notes/2020.06.23_workshop-4_notes.md)
- Atelier #5 : mardi 8 septembre 2020 par téléconférence - [notes de l'atelier](./workshops-notes/2020.09.08_workshop-5_notes.md)
- Atelier #6 : mardi 10 novembre 2020 par téléconférence - [notes de l'atelier](./workshops-notes/2020.11.10_workshop-6_notes.md)
- Atelier #7 : mardi 15 décembre 2020 par téléconférence - [notes de l'atelier](./workshops-notes/2020.12.16_workshop-7_notes.md)

#### Saison 2

- Atelier #1 : lundi 22 février 2021
- Atelier #2 : lundi 26 avril 2021
- Atelier #3 : lundi 21 juin 2021
- Atelier #4 : lundi 20 septembre 2021
- Atelier #5 : lundi 22 novembre 2021
- Atelier #6, suivi d'un temps de convivialité : jeudi 9 décembre 2021

Curieux ? Enthousiaste ? Sceptique ? Essayons ensemble, avec toutes les bonnes énergies de celles et ceux qui sont intéressés par le sujet et la démarche, avec l’esprit ouvert à la possibilité que cette démarche puisse muter, rencontrer d’autres initiatives, peut-être ne pas aboutir… avec la certitude en revanche de débattre et d’apprendre sur des sujets passionnants.

### Responsabilité éditoriale, disponibilité en ligne des travaux et participation asynchrone

Ce travail est élaboré sous la responsabilité éditoriale de l'association à but non lucratif Substra Foundation, qui s'engage à le mettre à disposition de manière à ce qu'il puisse être librement reproduit et partagé.

Ainsi, le projet en ligne et le dépôt de fichiers associés, hébergés par Substra Foundation sur GitHub, assurent la disponibilité en ligne de ces travaux et du référentiel de la data science responsable et de confiance. Au-delà des ateliers participatifs bimestriels, il est donc également possible de participer de manière asynchrone.

### Nature évolutive

Par nature cette démarche est en constante évolution. Il nous semble plus utile et plus transparent de mettre à disposition le référentiel dans son état du moment, plutôt que d'attendre le franchissement de jalons majeurs. Ainsi, chacun est en mesure d'en prendre connaissance et de participer par des questions ou des suggestions d'amélioration.
Une logique de versions ou de jalons sera proposée afin de fournir un repère temporel aux organisations utilisatrices.

### Mise à disposition

<a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-nd/4.0/88x31.png" /></a><br />Ce(tte) œuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/4.0/">Licence Creative Commons Attribution - Pas d&#39;Utilisation Commerciale - Pas de Modification 4.0 International</a>.
