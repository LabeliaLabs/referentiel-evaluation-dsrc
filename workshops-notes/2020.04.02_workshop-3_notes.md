# Atelier du 2 avril 2020

_Présents : @ClementMayer, @bowni, @natct10, @SaboniAmine, @celinejacques, Anne-Sophie Cissey, Timothée Faucon, Cédric Meurée, Jeremie Abiteboul, Raphaelle Bertrand, Augustin Durivault, Anabelle Blangero, Timothé Delion, Grégory Chatel_

_Merci à tous !_

Retrouvez [les slides de la présentation](https://docs.google.com/presentation/d/1C46TOlvJidpKBekw8xjbqVU3q3h7kl85jfCfdb7x0kQ/edit)

## Présentation de la démarche et de Substra Foundation

### Substra Foundation

- [Présentation de l'association](https://frama.link/substrapres)
- [Repos Substra et de ses travaux](https://github.com/SubstraFoundation/)
- [Projet Healthchain](https://www.substra.ai/fr/healthchain-project)
- [Projet Melloddy](https://www.substra.ai/fr/melloddy-project)
- _New_ ! La documentation du [framework Substre](https://substrafoundation.github.io)

### Démarche Data Science Responsable et de Confiance

- [Le dépôt](https://github.com/SubstraFoundation/referentiel-ds-responsable-confiance)
- [Le référentiel](https://github.com/SubstraFoundation/referentiel-ds-responsable-confiance/blob/master/referentiel.md)

## Présentation aiVision et retour d'expérience

Présentation par Cédric Meurée, [aiVision](https://www.aivision.health/)

### Présentation aiVision :

- Plateforme de télémédecine pour ophtalmologistes et orthoptistes
- Solutions basées sur de l'intelligence artificielle pour l'aide au diagnostic (rétinopathie diabétique, DMLA, glaucome)

### Pourquoi rejoindre les ateliers ?

- Domaines d'activité
- Convictions et intérêts personnels
- Croissance de l'équipe aiVision : bon moment pour s'interroger sur bonnes pratiques à mettre en place
- Visibilité et crédibilité pour l'entreprise : atout dans ce secteur d'activité

### Revue des mesures

Revue de deux mesures par thème (afin de ne pas parcourir tout le référentiel) et de l'évaluation de ces données.

L'évaluation est sur une échelle de 0 à 5 - Les niveaux de maturité :

- 0 : Mesure non implémentée / Pratique inexistante ou incomplète
- 1 : Mesure en cours d'implémentation / Pratique informelle
- 2 : Mesure implémentée nécessitant amélioration / Pratique répétable et suivie
- 3 : Mesure implémentée / Processus défini
- 4 : Mesure implémentée et contrôlée / Processus contrôlé
- 5 : Mesure implémentée, contrôlée et optimisée / Processus en amélioration continue

**Question :** Sur l'utilisation de dataset de données publiques : quelles informations sont disponibles ? Manière de prendre les photos, technologies, ... ?

Des informations sont prises sur le dataset, beaucoup sont récents avec de l'information sur comment ils ont été constitués.
Sur des dataset plus anciens, images segmentés à la main : moins d'informations disponibles.  

**Question :** L'âge des patients est-il disponible sur toutes les données ?
Pour les jeux de données publiques, ils viennent souvent d'Amerique du nord et d'Indes : information disponnible sur l'éthnie par exemple mais pas nécessairement l'âge.

L'information est présente sur les dataset d'études cliniques nécessaires pour valider les dispositifs médicaux.
--> l'information est disponible plus facilement sur les datasets de test que d'entrainement.

**Fairness metrics (BIA-03) :**
Certaines mesures ne sont pas pertinentes en fonction du domaine de l'organisation. Certaines mesures sont rédigées de manière trop ambigües et sont difficiles à répondre.

**Question :** DON-3 - évaluation d'aiVision de 4/5 : êtes vous en capacité de déterminer ce qu'il vous faut faire pour passer d'un processus défini à un processus contrôlé ?

Aujourd'hui, l'accompagnement est extérieur pour le projet. Nécessité d'internaliser la compétence / de s'approoprier les outils. Trop de dépendance à l'accompagnement.


**Référence essentielle :** [Continous delivery for machine learning](https://martinfowler.com/articles/cd4ml.html)

Cette référence a été utilisée pour traiter un certain nombre de mesures.

**Processus vs. Formalisation :** Certaines mesures sont bien mises en place mais pas toujours documentées.

**Réutilisation de modèle (exemple : transfer learning) :** nécessité d'avoir la généaologie des modèles qui sont transférés. Forte complexité. Beaucoup de recherche et outil sur le sujet en cours.

**Question :** Avez-vous implémentés une boucle de feedback pour récupérer les retours des médecins/experts sur les prédictions?

En amont : validation de l'outil : besoin d'avoir plusieurs médecins qui notent les mêmes images puis croisement des résultats. Application de l'outil --> rapprochement entre le retour des médecins et l'outil.
Cela est obligatoire pour validation réglementaire du dispositif.

Une fois que le modèle existe et mis en prod : pas de vérification mise en place à ce stade.

**Référence intéressante :** Calcul de l'impact CO2 en fonction de la plateforme, de la région - [ML CO2 impact](https://mlco2.github.io/impact/)

### Intérêt de l'exercie d'auto-évaluation

**Aspect positif :**

- Démarrage dynamique CI/CD en machine learning : s'inscrire dans l'esprit des mesures de type généalogie des modèles
- Mesures les plus avancées : suivi de projets individuels    

**Amélioration :**

- Généraliser la documentation, au niveau de l'entreprise
- Identifier et définir plus clairement les chaînes de responsabilités

=> Bilan très positif


**Question :** Votre modèle principal étant du deep learning, qu'en est-il de l'interprétabilité / explicabilité des décisions ?

Inclure les probabilités de décisions - fournir les probas par classe en plus du diagnostique
Mettre en place l'explication : quelle zone de l'image a aidé à faire le diagnostique.
Travail également sur des analyses d'images plus classiques


## Enseignements

L'outil est déjà utile !
Les points d'amélioration sont détaillés dans la présentation : certaines mesures vont être revues afin de résoudre ces différents problèmes.

## Prochaines étapes et ouverture

_D'autres organisations souhaitent s'auto-évaluer ? Dites-le-nous !_

Retour d'aiVision sur l'auto-évaluation : cela permet de prendre du recul, de voir où on en est.

**Temps pour réaliser l'évaluation :** environ une demi-journée  (vs 140h sur le référentiel de l'initiative de l'Union Européenne!)

La plateforme de self-assessment est en cours de travail !

**Référence :**

- Initiative ["Model Cards"](https://modelcards.withgoogle.com/about)de Google.
Souvenir de toutes les étapes de la création d'un modèle --> à creuser pour les ressources.

- [Dataset Version Control](https://dvc.org)
Versioning de vos performances / datasets
Outil de versioning de dataset pour la data science.
Tagguer certains modèles en fonction des datasets utilisés.


**Question :** Les outils du framework open source Substra permettent-ils "par construction" d'obtenir de bonnes cotations selon le référentiel ? Quelles dimensions en particulier ?

Framework Substra : une des ressources parmis les nombreuses utiles pour les approches responsable et de confiance :
- Tracabilité complète de toutes les opérations dans les projets : généalogie de bout en bout, historique intéressant pour l'audit / certification
- Protection de la confidentialité de la donnée : projet de DS sans que les données ne bougent, uniquement les modèles et les algos. Risque pas zéro mais diminution du risque.
- Performance : cadrage de la performance, nécessité de rentrer sa metric de performance + la séparation training test. Pas de possibilité de hacker la performance.  


**Merci à tou.te.s**


_Inscrivez-vous à notre newsletter pour ne pas manquer la prochaine édition !_
www.substra.ai
