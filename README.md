# Comment définir la data science responsable et de confiance ?

## Motivations et ambition

Un nouvel espace émerge au croisement entre expansion de l'IA dans les organisations et les systèmes automatiques, et inquiétudes du public sur les données privées, la transparence et la robustesse des algorithmes.

Ce sont deux tendances puissantes qui commencent déjà à se percuter. Comment les réconcilier, les conjuguer ensemble ? Des solutions techniques et organisationnelles nouvelles sont indispensables pour cela, pour accorder un cadre de confiance qui manque aujourd’hui, pour rendre possible des collaborations nouvelles, prometteuses et sûres entre les entreprises, les institutions publiques et les citoyens.

De nombreux acteurs s'emparent du sujet et travaillent par exemple déjà à des cadres pour un usage éthique et à impact positif des technologies d'IA, à des outils pour apporter de la traçabilité aux travaux de data science, à des formations pour éviter la reproduction de biais discriminatoires, à des briques techniques pour permettre la mutualisation et renforcer la confidentialité des données, etc.

En s'appuyant sur les travaux, cadres et corpus existants, nous vous proposons de travailler de manière ouverte et collaborative à la définition de ce que serait la **data science responsable et de confiance**. L'objectif ? Établir ensemble un référentiel open source de bonnes pratiques permettant aux organisations intéressées d'évaluer leur niveau de maturité (sur le modèle de l'annexe A de la norme ISO 27001 ou du label B-Corp par exemple).

Ce référentiel devra être actionnable, opérationnel, pour que cela puisse être utile le plus rapidement possible, susciter des réflexions, des échanges, des souhaits d'amélioration. Cela pourra faciliter l'émergence d'offres d'évaluation et de formation dans ce domaine.

### Pourquoi _responsable_ et _de confiance_ ?

_Responsable_ : Qui se préoccupe des conséquences sur ses parties prenantes, cherche à avoir un impact positif, essaie d'éviter d'être _irresponsable_ c'est-à-dire ne pas maîtriser des conséquences préjudiciables pour ses parties prenantes.

_De confiance_ : Dans lequel on peut avoir un niveau de confiance raisonnable car les règles de l'art prévenant une large panoplie de risques typiques sont appliquées.

Les deux notions se recouvrent en partie. Il est cependant difficile de trouver un terme unique satisfaisant. La combinaison des deux apporte une richesse intéressante.

### Inspirations

- Annexe A ISO 27001
- ITIL
- B-Corp
- Don en confiance
- Exemple Apple Card et Goldman Sachs

### Un référentiel de bonnes pratiques

- Référentiel de _bonnes pratiques_. Une bonne pratique est une pratique cible, une mesure qui peut ou non être mise en oeuvre. Par exemple voici une mesure extraite de l'annexe A d'ISO 27001 :
> _Des procédures de gestion des supports amovibles doivent être mises en œuvre conformément au plan de classification adopté par l’organisation._

- Chaque organisation met en oeuvre les mesures cibles à sa façon avec un certain _niveau de maturité_ qui peut évoluer dans le temps :

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

### Disponibilité en ligne des travaux et participation asynchrone

Ce projet en ligne et le dépôt de fichiers associés, hébergés par Substra Foundation sur Github, assurent la disponibilité en ligne de ces travaux et du référentiel de la data science responsable et de confiance. Au-delà des ateliers participatifs bimestriels, il ainsi possible de participer de manière asynchrone.

### Nature évolutive

Par nature cette démarche est en constante évolution. Il nous semble plus utile et plus transparent de mettre à disposition le référentiel dans son état du moment, plutôt qu'attendre que des jalons majeurs soient franchis. Ainsi, chacun est en mesure d'en prendre connaissance et de participer par des questions ou des suggestions d'amélioration.
Une logique de versions ou de jalons sera proposée afin de fournir un repère temporel.

## Périmètres cible et hors-cible

- Un référentiel de pratiques qui s'adresse à qui ?
    - Cible : l'activité data science d'une organisation
    - Hors-cible : un projet spécifique, un produit donné, un modèle en particulier
    - Pourquoi ?
        - Les projets et produits peuvent prendre des formes extrêmement variées et il est donc très difficile d'être pertinent avec un référentiel générique
        - L'effort pour s'évaluer selon un référentiel peut être trop élevé s'il doit être fait projet par projet
        - Les mesures ou pratiques relatives aux collaborateurs (e.g. la formation) correspondent plus naturellement aux pratiques d'une organisation et pas d'un projet déterminé
- Que désigne-t-on par _IA_ et _data science_ ?
    - Cible : l'utilisation de techniques algorithmiques sur des données, les modèles prédictifs et les systèmes automatiques en résultant
    - Hors cible : ...

## Propositions de thèmes, d'un canevas du référentiel

| # | Thème | Description |
|---|---|---|
| 1 | **Protéger les données personnelles ou confidentielles** | L'utilisation de données personnelles ou confidentielles fait porter le risque d'exposition de celles-ci, ce qui peut avoir des conséquences très préjudiciables pour les producteurs, gestionnaires, ou sujets de ces données. Elles doivent donc être protégées, les risques d'exposition doivent être minimisés. |
| 2 | **Prévenir les biais malencontreux** | L'utilisation de modèles prédictifs élaborés à partir de données historiques peut se révéler néfaste lorsque les données historiques décrivent des phénomènes non souhaitables. Il apparaît indispensable de s'interroger sur ce risque et d'étudier la nature des données utilisées et ce qu'elles représentent. |
| 3 | **Evaluer la performance de manière rigoureuse** | Le score de performance d'un modèle prédictif est déterminant pour son adoption dans des produits, systèmes ou processus. L'évaluation de la performance se doit donc d'être rigoureuse. |
| 4 | **Etablir et maintenir une généalogie des modèles** | Un modèle prédictif est un objet informatique complexe qui peut évoluer au fil des apprentissages. Tracer les étapes de son élaboration et de son évolution permet d'en constituer une forme de _généalogie_, pré-requis pour reproduire ou auditer un modèle. |
| 5 | **Garantir la chaîne de responsabilité des modèles** | Un modèle prédictif peut-être utilisé comme un système automatique, dont les règles de fonctionnement ne se prêtent pas ou mal à être explicitées, débattues, ajustées. Des efforts sont nécessaires sur l'interprétation et l'explication des choix réalisés à l'aide de ces systèmes. Il apparaît également indispensable de garantir une chaîne de responsabilité claire, de personnes physiques ou morales, pour chaque modèle. |
| 6 | **Minimiser l'empreinte énergétique de l'activité data science** | Les ressources informatiques peuvent être gourmandes en énergie et avoir une empreinte environnementale significative si elles ne sont pas optimisées. Prendre conscience de ce phénomène est indispensable, chercher à optimiser l'utilisation des ressources est nécessaire. |
