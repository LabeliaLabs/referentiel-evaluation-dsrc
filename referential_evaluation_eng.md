# Responsible and trustworthy data science - Evaluation framework

The [Assessment Framework](#framework-for-assessing-the-maturity-of-an-organization) below is under development. It proceeds from the identification of the [risks](#risks) that we want to prevent in the responsible and trustworthy practice of data science. It is structured into several complementary [themes](#themes-of-the-evaluation-framework).

## Framework for assessing the maturity of an organization

The evaluation consists of the following 7 sections:

- [Section 1 - Protecting personal or confidential Data](#section-1---protecting-personal-or-confidential-data)
- [Section 2- preventing unintended bias](#section-2---preventing-unintended-bias)
- [Section 3 - Rigorously Assessing Performance](#section-3---assessing-performance-rigorously)
- [Section 4 - Establishing and Maintaining a model genealogy](#section-4---establishing-and-maintaining-a-model-genealogy)
- [Section 5 - Ensuring chain of responsibility](#section-5---ensuring-chain-of-responsibility)
- [Section 6 - Using learned predictive models](#section-6---using-learned-predictive-models)
- [Section 7 - Anticipating, Monitoring and Minimizing Externalities of Data Science Activity](#section-7---anticipate-monitoring-and-minimizing-the-externalities-of-data-science-activity)

---

### Section 1 - Protecting personal or confidential data

The use of personal or confidential data brings the risk of exposure of such data, which can have very hamrful consequences for the producers, users, or subjects of such data. Particularly in data science projects, they must therefore be protected and the risks of their leakage or exposure must be minimised.

[_[⇧ back to list of sections](#framework-for-assessing-the-maturity-of-an-organization)_]  
[-[⇩ next section](#section-2---preventing-unintended-bias)_]

---

Q1.1: **Applicable legislation and contractual requirements - Identification**.  
With regard to personal and/or confidential data, the legal, statutory, regulatory and contractual requirements in force and concerning your organization are:

R1.1:  
_(Type: single response)_  
_(Select only one answer, best suited to the organization's level of maturity on this topic)_

- [ ] 1.1.a not yet identified
- [ ] 1.1.b partially identified or in the process of being identified
- [ ] 1.1.c identified
- [ ] 1.1.d identified and controlled by collaborators
- [ ] 1.1.e identified, documented and mastered by collaborators

<details>
<summary>Expl1.1:</summary>

Set up processes to know and follow the evolution of applicable regulations (very specific in some sectors), as well as to document the approaches and choices made to comply with each data science project. Example(s) of interest: [Welfare surveillance system violates human rights, Dutch court rules](https://www.theguardian.com/technology/2020/feb/05/welfare-surveillance-system-violates-human-rights-dutch-court-rules).

</details>

---

Q1.2: **Applicable legislation and contractual requirements - methodology**.    
To meet these requirements, your organization's approach is:

R1.2:  
_(Type: single response)_  
_(Select only one answer, best suited to the organization's level of maturity on this topic)_

- [ ] 1.2.a informal, based on individual responsibility and competence
- [ ] 1.2.b formalized and accessible to all collaborators
- [ ] 1.2.c formalised and controlled by the collaborators
- [ ] 1.2.d formalized, controlled by collaborators, documented for each processing of personal or confidential data

<details>
<summary>Expl1.2:</summary>

It is a question of questioning the management of personal or confidential data (storage, access, transfer, protection, responsibilities...), and documenting the choices made.

</details>

---

Q1.3: **Regulatory watch**  
Is a regulatory wattch monitoring process in place, either internally or through a specialised service provider, to find out about applicable changes that have an impact on your organisation?

R1.3:  
_(Type: single response)_  
_(Select only one answer, best suited to the organization's level of maturity on this topic)_

- [ ] 1.3.a We don't really do regulatory monitoring.
- [ ] 1.3.b We keep an informal watch, with each coollaboratoor reporting information on a dedicated means of communication.
- [ ] 1.3.c We have a formal monitoring system, those responsible are identified and the process is documented.

<details>
<summary> Expl1.3: </summary>

Set up processes to know and follow the evolution of applicable regulations (very specific in some sectors), as well as to document the approaches and choices made to comply with each data science project. Example(s) of interest: [Welfare surveillance system violates human rights, Dutch court rules](https://www.theguardian.com/technology/2020/feb/05/welfare-surveillance-system-violates-human-rights-dutch-court-rules).

</details>

Q1.4: **Applicable legislation and contractual requirements - Auditing and certification** 
Has the organization's compliance with personal and confidential data requirements been audited and is it recognized by a certification, third party body or equivalent?

R1.4:  
_(Type: single response)_  
_(Select only one answer, best suited to the organization's level of maturity on this topic)_

- [ ] 1.4.a Yes
- [ ] 1.4.b No

<details>
<summary> Expl1.4: </summary>

In many sectors there are specific compliance requirements. It is generally possible to formalise an organisation's compliance through certification or a specialised audit, or by obtaining a label.

</details>

---

Q1.5: **Principle of minimization**
In data science projects, the principle of minimization should guide the collection and use of personal or confidential data. How is it implemented in your organization?

R1.5:  
_(Type: single response)_  
_(Select only one answer, best suited to the organization's level of maturity on this topic)_

- [ ] 1.5.a We ensure that we do not use any personal or confidential data. We are not concerned by this kind of risk.
- [ ] 1.5.b We need to use them in certain projects and the minimisation principle is then systematically applied.
- [ ] 1.5.c The principle of minimisation is known to collaborators, who generally apply it.
- [ ] 1.5.d The "who can do the most can do the least" reflex with regard to data still exists here and there within our organization. In some projects, we keep datasets that are much richer in personal and confidential data than what is strictly useful to the project.
  
---

The following elements within this section apply only to organizations that did not select the first response to R1.5. Organizations not involved are therefore invited to proceed to [Section 2](#section-2---preventing-unintended-bias).

---

Q1.6: **Project involving new processing of personal or confidential data**  
_(Condition: R1.5 <> 1st answer)_  
For each processing of personal or confidential data required in the context of a data science project within your organisation:

R1.6:  
_(Type: multiple responses possible)_  
_(Select all response items that correspond to practices in your organization)_

- [ ] 1.6.a we develop a _Privacy Impact Assessment_ (PIA)
- [ ] 1.6.b we implement protection measures (in particular concerning the transfer, storage and access to the data concerned).
- [ ] 1.6.c we document APIs and measures implemented and keep them within projects.
- [ ] 1.6.d we contract the relationships with suppliers and customers and the responsibilities that arise from this.

---

Q1.7: **Safety of machine learning and _PETs_ - Knowledge level**  
_(Condition: R1.5 <> 1st answer)_  
Machine learning security (_ML security_) is a rapidly developing field. In some cases, predictive models learned from confidential data may reveal elements of the confidential data. Within your organization, regarding vulnerabilities related to ML models and Privacy Enhancing Technologies (PETs), the general level of knowledge of collaborators involved in data science projects is:

R1.7:  
_(Type: single response)_  
_(Select only one answer, best suited to the organization's level of maturity on this topic)_

- [ ] 1.7.a Beginner
- [ ] 1.7.b Intermediate
- [ ] 1.7.c Confirmed
- [ ] 1.7.d Expert

<details>
<summary> Expl1.7: </summary>

The state of the art in ML security is constantly evolving. While it is impossible to guard against all vulnerabilities at all times, it is crucial to be aware of them and keep yourself informed. The [OWASP Top Five ML risks](https://github.com/OWASP/Top-5-Machine-Learning-Risks/blob/master/Top%205%20Machine%20Learning%20Risks.md) is for example an interesting entry point.

</details>

<details>
<summary>Resources1.7:</summary>

- [Top Five ML risks](https://github.com/OWASP/Top-5-Machine-Learning-Risks/blob/master/Top%205%20Machine%20Learning%20Risks.md), OWASP
- The secret-sharer: evaluating and testing unintended memorization in neural networks](https://blog.acolyer.org/2019/09/23/the-secret-sharer/)*, A. Colyer, 2019.
- *[Membership Inference Attacks against Machine Learning Models](https://arxiv.org/abs/1610.05820)*, R. Shokri, M. Stronati, C. Song, V. Shmatikov, 2017 and further analysis *[Demystifying the membership inference attack](https://medium.com/disaitek/demystifying-the-membership-inference-attack-e33e510a0c39)*, Disaitek, 2019. A tool called [ML Privacy Meter](https://github.com/privacytrustlab/ml_privacy_meter) to quantify the privacy risks of machine learning models with respect to inference attacks is also available
- *[Inverting Gradients - How easy is it to break privacy in federated learning?](https://arxiv.org/abs/2003.14053)*, J. Geiping, H. Bauermeister, H. Dröge, M. Moeller, 2020
- Tools for *differential privacy*: Google [differential privacy library](https://github.com/google/differential-privacy) and its Python wrapper [PyDP](https://github.com/OpenMined/PyDP) by OpenMined
- The *distillation* of a model, in addition to the compression it provides, can be used as a measure to protect the model and the training data used, see for example *[Knowledge Distillation: Simplified](https://towardsdatascience.com/knowledge-distillation-simplified-dd4973dbc764)*, Towards Data Science, 2019, and *[Distilling the Knowledge in a Neural Network](https://arxiv.org/abs/1503.02531)*, G. Hinton, O. Vinyals, J. Dean, 2015

</details>

---

Q1.8: **Safety of Machine Learning and _PETs_ - Implementation**
_(Condition: R1.5 <> 1st answer)_  
Still on the subject of vulnerabilities related to ML models and _(PETs)_:

R1.8:  
_(Type: multiple responses possible)_
_(Select all response items that correspond to practices in your organization)_

- [ ] 1.8.a A technical watch and monitoring is implemented
- [ ] 1.8.b Collaborators receive regular information/training to enable them to improve their skills.
- [ ] 1.8.c In some projects, we implement _PETs_ to reduce the risks associated with the models we develop.
- [ ] 1.8.d On each project, the vulnerabilities that apply to it and the _PETs_ implemented are documented in the End-to-End Genealogy (G2B) of each model.

<details>
<summary>Expl1.8:</summary>

The state of the art in ML security is constantly evolving. While it is impossible to guard against all vulnerabilities at all times, it is crucial to be aware of them and to keep a watch. The [OWASP Top Five ML risks](https://github.com/OWASP/Top-5-Machine-Learning-Risks/blob/master/Top%205%20Machine%20Learning%20Risks.md) is for example an interesting entry point.

Depending on the level of risk and sensitivity of the projects, certain _PETs_ approaches will be selected and implemented. It is important to follow the evolution of the state of the art and practices, and to document the choices made. We introduce here the notion of ["end-to-end genealogy"] (#section-4---establishing-and-maintaining-a-model-genealogy).

</details>

<details>
<summary>Resources1.8:</summary>

- [Top Five ML risks](https://github.com/OWASP/Top-5-Machine-Learning-Risks/blob/master/Top%205%20Machine%20Learning%20Risks.md), OWASP
- The secret-sharer: evaluating and testing unintended memorization in neural networks](https://blog.acolyer.org/2019/09/23/the-secret-sharer/)*, A. Colyer, 2019.
- *[Membership Inference Attacks against Machine Learning Models](https://arxiv.org/abs/1610.05820)*, R. Shokri, M. Stronati, C. Song, V. Shmatikov, 2017 and further analysis *[Demystifying the membership inference attack](https://medium.com/disaitek/demystifying-the-membership-inference-attack-e33e510a0c39)*, Disaitek, 2019. A tool called [ML Privacy Meter](https://github.com/privacytrustlab/ml_privacy_meter) to quantify the privacy risks of machine learning models with respect to inference attacks is also available
- *[Inverting Gradients - How easy is it to break privacy in federated learning?](https://arxiv.org/abs/2003.14053)*, J. Geiping, H. Bauermeister, H. Dröge, M. Moeller, 2020
- Tools for *differential privacy*: Google [differential privacy library](https://github.com/google/differential-privacy) and its Python wrapper [PyDP](https://github.com/OpenMined/PyDP) by OpenMined
- The *distillation* of a model, in addition to the compression it provides, can be used as a measure to protect the model and the training data used, see for example *[Knowledge Distillation: Simplified](https://towardsdatascience.com/knowledge-distillation-simplified-dd4973dbc764)*, Towards Data Science, 2019, and *[Distilling the Knowledge in a Neural Network](https://arxiv.org/abs/1503.02531)*, G. Hinton, O. Vinyals, J. Dean, 2015

</details>

---

Q1.9: ** Notification of safety incidents to regulatory authorities**  
_(Condition: R1.5 <> 1st answer)_  
In the event that a model developed by the organization is used or accessible by an external stakeholder(s), and a new vulnerability is published, there is a risk that it may apply to the model and create a risk of exposure of personal or confidential data:

R1.9:  
_(Type: multiple responses possible)_  
_(Select all response items that correspond to practices in your organization)_

- [ ] 1.9.a We have a procedure outlining how to proceed.
- [ ] 1.9.b Our procedure includes communication to the stakeholders in question.
- [ ] 1.9.c Our procedure refers to the authorities to whom we must report.

<details>
<summary>Expl1.9:</summary>

In some sectors there are obligations to report safety incidents to regulatory authorities (e.g. CNIL, ANSSI, ARS, etc.). An interesting entry point: [Notifications of security incidents to regulatory authorities: how to organize and who to contact](https://www.cnil.fr/fr/notifications-dincidents-de-securite-aux-autorites-de-regulation-comment-sorganiser-et-qui-sadresser) on the CNIL website.

</details>

---
---

### Section 2 - Preventing Unintended Bias

The use of predictive models developed from historical data can be counterproductive when historical data are contaminated by problematic phenomena (e.g. quality of certain data points, non-comparable data, social phenomena undesirable due to the time period, etc.). It is essential to question this risk and to study the nature of the data used, the conditions under which they were produced and collected, and what they represent.
In some cases, a specification of the equity sought between populations must also be defined. The fairness of a model can [be defined in several ways that may be inconsistent with each other](https://papers.nips.cc/paper/6995-counterfactual-fairness), and the interpretation of performance scores must therefore be done within the framework of one of these definitions.

[_[⇧ back to list of sections](#framework-for-assessing-the-maturity-of-an-organization)_]  
[_[⇩ next section](#section-3---assessing-performance-rigorously)_]

---

Q2.1: **Analysis of training data used**
Within data science projects and when developing training datasets, thinking about and searching for unintended or parasitic phenomena due to time, context, recording tools or processes can be crucial to prevent unfortunate biases. Your organization:

R2.1:  
_(Type: single response)_  
_(Select one answer only, best suited to the organization's level of maturity on this topic)_

- [ ] 2.1.a operates informally in this respect and relies on the competence and responsibility of the collaborators involved.
- [ ] 2.1.b has a documented approach that is systematically implemented.

<details>
<summary> Expl2.1: </summary>

It is a question of forcing to ask oneself about these subjects and therefore to think about the data used, the way in which they were produced, and so on.

</details>

<details>
<summary>Resources2.1:</summary>

- *[Tour of Data Sampling Methods for Imbalanced Classification](https://machinelearningmastery.com/data-sampling-methods-for-imbalanced-classification/)*
- *[Hidden Bias](https://pair.withgoogle.com/explorables/hidden-bias/)* explorable from [PAIR](https://pair.withgoogle.com/)

</details>

---

Q2.2: **Risks of discrimination against certain social groups**  
Is your organisation concerned with cases where predictive models are used in thematic environments where there are risks of discrimination against certain social groups (gender, origin, age, etc.)?

R2.2:  
_(Type: single response)_  
_(Select only one answer, best suited to the organization's level of maturity on this topic)_

- [ ] 2.2.a Concerned
- [ ] 2.2.b Not concerned

---

The following elements within this section apply only to organizations that have selected the "Concerned" response in R2.2. Organizations not involved are therefore invited to move on to [Section 3](#section-3---assessing-performance-rigorously).

---

Q2.3: **Preventing discriminatory biases**  
_(Condition: R2.2 = Concerned)_  
In cases where the predictive models your organisation develops are used in thematic environments where there is a risk of discrimination against certain social groups (gender, origin, age, etc.):

R2.3:  
_(Type: multiple responses possible)_  
_(Select all response items that correspond to practices in your organization)_

- [ ] 2.3.a We pay particular attention to the identification of protected variables and their possible proxies.
- [ ] 2.3.b We evaluate test data from different sub-populations to identify potential problem biases.
- [ ] 2.3.c We select and implement one or more measures of fairness and equity (_fairness metric_).
- [ ] 2.3.d We use _data augmentation_ or _re-weighting_ approaches.
- [ ] 2.3.e The above practices that we implement are duly documented as part of the G2B of the models concerned.

<details>
<summary>Expl2.3:</summary>

It is a question of systematically questioning, for each data science project and according to the objective and target use of the model that one wants to develop, the features that may directly or indirectly be at the origin of a risk of discriminatory bias.
Complement on the use of synthetic data and _data augmentation_, _re-weighting_ approaches: when such techniques are used it is important to make them explicit, otherwise we risk losing information on how a model was developed.

</details>

<details>
<summary>Resources2.3:</summary>

- *[Measuring fairness](https://pair.withgoogle.com/explorables/measuring-fairness)* exploreable, [PAIR](https://pair.withgoogle.com/)
- _[AI Fairness 360](https://developer.ibm.com/technologies/artificial-intelligence/projects/ai-fairness-360/): an open source software toolkit that can help detect and remove bias in machine learning models_, IBM
- Fairness metrics: _[counterfactual fairness](https://papers.nips.cc/paper/6995-counterfactual-fairness)_, _[adversarial debiaising](https://arxiv.org/pdf/1801.07593.pdf)_

</details>

---
---

### Section 3 - Rigorously Evaluating Performance

The performance score of a predictive model is critical for its adoption in products, systems or processes. Performance evaluation must therefore be rigorous. On the other hand, a predictive model can be used as an automatic system, whose rules of operation are not written _in extenso_ and do not lend themselves or badly to be explained, debated, adjusted. Efforts are therefore needed to interpret and explain the choices made using these systems.

[_[⇧ back to list of sections](#framework-for-assessing-the-maturity-of-an-organization)_]  
[_[⇩ next section](#section-4---establishing-and-maintaining-a-model-genealogy)_]

---

Q3.1: **Separation of test datasets**  
In data science projects and when developing test datasets, it is of utmost importance to ensure non-contamination by training data. Your organization:

R3.1:  
_(Type: combined)_  
_(Select all response items that correspond to practices in your organization. Caution, some combinations would not be consistent)_

- [ ] 3.1.a operates informally in this respect and relies on the competence and responsibility of the collaborators involved.
- [ ] 3.1.b has a documented and systematically implemented approach to test set isolation.
- [ ] 3.1.c uses a versioning and traceability tool for the training and test datasets used, thus enabling the non-contamination of test data to be checked or audited at a later date.
- [ ] 3.1.d systematically provides for the development of two or more testsets to increase resilience.

---

Q3.2: **Distributed learning projects that maintain confidentiality**
In the case of data science projects based on distributed learning or federated learning on multiple datasets and whose confidentiality must be preserved with respect to others (_privacy-preserving_):

R3.2:  
_(Type: single response)_  
_(Select only one answer, best suited to the organization's level of maturity on this topic)

- [ ] 3.2.a We do not participate in _privacy-preserving distributed learning_ projects.
- [ ] 3.2.b We master and implement approaches to develop test data sets in such a way that there is no cross-contamination between training and test data from different partners.
- [ ] 3.2.c At this stage we do not master the methods for developing test datasets so that there is no cross-contamination between training and test data from the different partners.

---

Q3.3: **Analysis of test data**
Within data science projects and when developing test datasets, thinking about and searching for unintended or parasitic phenomena due to time, context, recording tools or processes can be crucial for the meaning of performance scores. Your organization:

R3.3:  
_(Type: single response)_  
_(Select one answer only, best suited to the organization's level of maturity on this topic)_

- [ ] 3.3.a operates informally in this respect and relies on the competence and responsibility of the collaboroators involved.
- [ ] 3.3.b has a documented approach that is systematically implemented.

<details>
<summary>Expl3.3:</summary>

The use of predictive models tested on historical data can be counterproductive when the historical data in question are contaminated by problematic phenomena (e.g. quality of certain data points, non-comparable data, social phenomena undesirable due to the time period, etc.). It is essential to question this risk and to study the nature of the data used, the conditions under which they were produced and collected, and what they represent.

</details>

---

Q3.4: **Performance Validation**
Does your organization implement the following approaches?

R3.4:  
_(Type: multiple responses possible)_  
_(Select all response items that correspond to practices in your organization)_

- [ ] 3.4.a Choice of a performance metric before machine learning training, among the most standard metrics possible.
- [ ] 3.4.b The implementation of robustness metrics is considered and evaluated for each model development project, and systematically implemented in projects where input data may be subject to fine perturbations (e.g. images, sounds).
- [ ] 3.4.c The above practices that we implement are duly documented and incorporated into the [G2B](#section-4---establish-and-maintain-a-model-genealogy) of the models concerned, including the performance metrics.

<details>
<summary>Expl3.4:/summary>

See for example the _[p-hacking / data dredging](https://fr.wikipedia.org/wiki/Data_dredging)_.

</details>

<details>
<summary>Resources3.4:</summary>

- Robustness metrics: _[noise sensitivity score](https://arxiv.org/abs/1806.01477)_.

</details>

---

Q3.5: **Monitoring of performance over time** 
In cases where predictive models developed by your organization are used in production systems:

R3.5:  
_(Type: combined)_  
(Select all response items that correspond to practices in your organization. Caution, some combinations would not be consistent)_

- [ ] 3.5.a The models we are developing are not currently in use | _(When this answer is selected, the others cannot be selected)_
- [ ] 3.5.b Performance is systematically reassessed when the model is updated.
- [ ] 3.5.c Performance is systematically re-evaluated when the context in which the model is used evolves, which can create a risk on the performance of the model due to the evolution of the input data space.
- [ ] 3.5.d Performance is regularly re-evaluated on updated test data, as input data may change.
- [ ] 3.5.e Random checks are carried out on predictions in order to check their consistency.

<details>
<summary>Expl3.5:</summary>

Even on a stable model, there is a risk that the input data will no longer be in the domain after a certain time (population & distribution), for example: a variable that would no longer be filled in at the same frequency as before by users in an IS. It is therefore necessary to regularly monitor the performance of a model used in its context of use.

</details>

<details>
<summary>Resources3.5:</summary>

- [Continuous delivery for machine learning](https://martinfowler.com/articles/cd4ml.html)
- [Monitoring Machine Learning Models in Production - A comprehensive guide](https://christophergs.com/machine%20learning/2020/03/14/how-to-monitor-machine-learning-models/), ChristopherGS, March 2020
- Google's medical AI was super accurate in a lab. Real life was a different story](https://www.technologyreview.com/2020/04/27/1000658/google-medical-ai-accurate-lab-real-life-clinic-covid-diabetes-retina-disease/)_, MIT Technology Review

</details>

---

Q3.6: **Classification thresholds and ranges of indecision** ** 
When developing a classification model, for the definition of classification thresholds, your organization:

R3.6:  
_(Type: combined)_  
_(Select all response items that correspond to practices in your organization. Caution, some combinations would not be consistent)_

- [ ] 3.6.a operates informally in this respect and relies on the competence and responsibility of the collaborators involved.
- [ ] 3.6.b has a documented approach that is systematically implemented.
- [ ] 3.6.c has a documented and systematically implemented approach, which includes the possibility of maintaining ranges of indecision.
- [ ] 3.6.d the choices made for each model and implemented are duly documented in the G2B of the models concerned.

<details>
<summary>Resources3.6:</summary>

- *[Opening the algorithm's black box and understand its outputs](https://medium.com/@asaboni/opening-the-algorithms-black-box-and-understand-its-outputs-e2363b0a887c)*, A. Saboni (Octo Technologies), April 2020

</details>

---

Q3.7: **Explicability and interpretability** 
Within data science projects that aim to develop predictive models for use in inference:

R3.7:  
_(Type: combined)_  
_(Select all response items that correspond to practices in your organization. Caution, some combinations would not be consistent)_

- [ ] 3.7.a Our organization is not yet familiar with the methods and tools for the explicability and interpretability of the models.
- [ ] 3.7.b We are interested in the explicability and interpretability of the models and are in dialogue with our stakeholders on this subject.
- [ ] 3.7.c We ensure that the models we develop provide, where relevant, at least a level of confidence with each prediction made.
- [ ] 3.7.d We determine the best compromise between performance and interpretability for each model we develop, which sometimes leads us to opt for a model that is simpler to explain to the people concerned (a high-performance model will reduce the risk of error, while an interpretable model will make it easier to justify the results of the model).
- [ ] 3.7.e We master and implement advanced approaches for the explicability and interpretability of the models.

<details>
<summary>Resources3.7:</summary>

- *[User Confidence in Systems Involving Artificial Intelligence](https://blog.octo.com/la-confiance-des-utilisateurs-dans-les-systemes-impliquant-de-lintelligence-artificielle/)*, Octo Technologies Blog, October 2019
- *[Interpretable Machine Learning, A Guide for Making Black Box Models Explainable](https://christophm.github.io/interpretable-ml-book/)*, Christoph Molnar
- In some cases, regulations require that the data subjects be able to explain to them how an algorithm works (see for example [Article 22 of the RGPD](https://www.cnil.fr/fr/reglement-europeen-protection-donnees/chapitre3#Article22), [Article 10 of the French Data Protection Act](https://www.legifrance.gouv.fr/affichTexteArticle.do;?idArticle=LEGIARTI000037090394&cidTexte=LEGITEXT000006068624&dateTexte=20180624), cited in particular in the [Hippocratic Oath for data scientist](https://hippocrate.tech/).

</details>

---

### Section 4 - Establishing and Maintaining a Model Genealogy

A predictive model is a complex computer object that can evolve over time. Tracing the stages of its elaboration and its evolution makes it possible to constitute a form of **genealogy**, a prerequisite for **reproducing or auditing** a model.

[_[⇧ back to list of sections](#framework-for-assessing-the-maturity-of-an-organization)_]  
[_[⇩ next section](#section-5---ensuring-chain-of-responsibility)_]

---

Q4.1: **"End-to-End Genealogy" of models**  
An end-to-end genealogy (G2B) of the models is fed and maintained as part of data science projects throughout the data collection, design, training, validation and operation phases:

R4.1:  
_(Type: single response)_  
_(Select one answer only, best suited to the organization's level of maturity on this topic)_

- [ ] 4.1.a At this stage we have not implemented such an approach.
- [ ] 4.1.b This information exists and is recorded so as not to be lost, but it can be lost in a disordered way and is not versioned.
- [ ] 4.1.c They are gathered in a single document that systematically accompanies the model.
- [ ] 4.1.d They are gathered in a single document that systematically accompanies the model and are versioned.

<details>
<summary>Expl4.1:</summary>

This concept of the "end-to-end genealogy" of a model can take the form, for example, of a reference document containing all the important choices and the entire history of the development of the model, and of the internal processes organizing this activity.

</details>

<details>
<summary>Resources4.1:<summary>

- [Substra Framework](http://doc.substra.ai/): an open source framework offering distributed orchestration of machine learning tasks among partners while guaranteeing secure and trustless traceability of all operations.
- [MLflow](https://mlflow.org/): an open source platform to manage the ML lifecycle, including experimentation, reproducibility, deployment, and a central model registry.
- [DVC](https://dvc.org/) _an Open-source Version Control System for Machine Learning Projects_, and [DAGsHub](https://dagshub.com/docs/) _a platform for data version control and collaboration_ [DVC](https://dvc.org/) _an Open-source Version Control System for Machine Learning Projects_, and [DAGsHub](https://dagshub.com/docs/) _a platform for data version control and collaboration_.

</details>

---

Q4.2: **Conditions and limitations on the use of a model**  
In data science projects, the "conditions and limits of validity" of a model designed, trained and validated by the organization:

R4.2:  
_(Type: combined)_  
_(Select all response items that correspond to practices in your organization. Caution, some combinations would not be consistent)_

- [ ] 4.2.a are not documented | _(When this answer is selected, the others cannot be selected)_
- [ ] 4.2.b are explained and documented
- [ ] 4.2.c are versioned
- [ ] 4.2.d documents presenting these "conditions and limits of validity" shall systematically accompany models throughout their life cycle.

<details>
<summary>Expl4.2:</summary>

The aim is to make explicit and add to the model the description of the context of use for which it was designed and in which its announced performance is significant. This concept of "conditions and limits of validity" can take the form of a synthetic document or a specific section in the "end-to-end genealogy".

</details>

---
---

### Section 5 - Ensuring Model Chain of responsibility

Using automatic systems based on models whose rules have been "learned" (and not defined and formalised) questions the way organisations operate. It seems essential to ensure a clear chain of responsibility, of natural or legal persons, for each model.

[_[⇧ back to list of sections](#framework-for-assessing-the-maturity-of-an-organization)_]  
[_[⇩ next section](#section-6---using-learned-predictive-models)_]

—

Q5.1: **Value and responsibility chain**  
In the case of data science projects where several players, including internal to the organisation (teams, departments, subsidiaries), are involved throughout the value and responsibility chain:

R5.1:  
_(Type: combined)_  
_(Select all response items that correspond to practices in your organization. Caution, some combinations would not be consistent)_

- [ ] 5.1.a Within our organization, data science projects are carried out end-to-end by autonomous teams, including the development of datasets and the exploitation of models for its own account. Consequently, for each project an autonomous team is solely responsible | _(When this answer is selected, the others cannot be selected)_
- [ ] 5.1.b We systematically identify the risks and responsibilities of each of the internal and external stakeholders with whom we work.
- [ ] 5.1.c We systematically contract with upstream (e.g. data suppliers) and downstream (e.g. customers, model-using partners) players.

<details>
<summary> Expl5.1: </summary>

It is important to ensure that organizations up and down the chain identify and take responsibility for their segments of the value chain.

</details>

---
Q5.2: **Distribution of the created value**  
In the case of data science projects where several partners work alongside your organisation to develop a model, and that model is or will be the subject of an economic activity:

R5.2:  
_(Type: combined)_  
_(Select all response items that correspond to practices in your organization. Caution, some combinations would not be consistent)_

- [ ] 5.2.a Our organization conducts its data science activities independently, including the development of data sets and the operation of models on its own behalf. It is therefore not concerned | _(When this answer is selected, the others cannot be selected)_
- [ ] 5.2.b At this stage we have not structured this aspect of multi-partner data science projects _(When this answer is selected, the others cannot be selected)._
- [ ] 5.2.c In these cases, we contract the economic aspect of the relationship with the stakeholders involved upstream of the project.
- [ ] 5.2.d Our organization has a policy that responsibly frames value sharing with the stakeholders involved.

<details>
<summary> Expl5.2: </summary>

When several partners work together to develop a model, it is important that the distribution of value resulting from an economic activity in which the model plays a role is made explicit and contractualized. In some cases this can be a complex issue, for example when a model is trained in a distributed manner across multiple datasets.

</details>

<details>
<summary>Resource5.2:</summary>

- [Exploration of dataset contributivity to a model in collaborative ML projects](https://github.com/SubstraFoundation/distributed-learning-contributivity), an open source project animated by Substra Foundation

</details>

---

Q5.3: **Subcontracting**.  
Activities subcontracted to or in partnership with a third party organization are subject to the same requirements as those that apply to your organization:

R5.3:  
_(Type: single response)_  
_(Select one answer only, best suited to the organization's level of maturity on this topic)_

- [ ] 5.3.a Yes
- [ ] 5.3.b No

<details>
<summary> Expl5.3: </summary>

As in the known frameworks of IS management (ISO 27001) or RGPD, it is important not to dilute responsibilities in uncontrolled subcontracting chains.

</details>

---

### Section 6 - Using Learned Predictive Models

Using automatic systems based on models whose rules have been "learned" (and not defined and formalised) questions the way organisations operate. It is important to preserve the responsiveness and resilience of the user organization, particularly in dealing with situations where predictive models have led to an undesirable outcome for the organization and its stakeholders.

[_[⇧ back to list of sections](#framework-for-assessing-the-maturity-of-an-organization)_]  
[_[⇩ next section](#section-7---anticipate-monitoring-and-minimizing-the-externalities-of-data-science-activity)_]

---

Q6.1: **Use predictive models for own account**  
If your organization uses predictive models on its own behalf:

R6.1:  
_(Type: combined)_  
_(Select all response items that correspond to practices in your organization. Caution, some combinations would not be consistent)_

- [ ] 6.1.a Our organization does not use predictive models developed by machine learning on its own behalf | _(When this answer is selected, the others cannot be selected)_
- [ ] 6.1.b **A predictive models register** identifies all the models used by the organization, we keep it up to date.
- [ ] 6.1.c For each model we have a **responsible contact point** defined, identifiable and easily contactable.
- [ ] 6.1.d For each model, we systematically carry out a **risk assessment** following possible incidents, failures, biases, etc., in order to identify the risks associated with each model.
- [ ] 6.1.e. Monitoring tools are in place to ensure continuous monitoring of ML systems and can trigger alerts directly to the responsible team.
- [ ] 6.1.f For each model, we define and test a procedure for suspending the model and a degraded operating mode without the model, in case the model fails or behaves abnormally.
- [ ] 6.1.g For each template, we study its [end-to-end genealogy](#section-4---establishing-and-maintaining-a-model-genealogy) and its conditions and limitations of use to understand the template before using it.
- [ ] 6.1.h We always use the models for **uses in accordance with their conditions and limits of use**

<details>
<summary>Expl6.1:</summary>

Using automatic systems based on models whose rules have been "learned" (and not defined and formalised) questions the way organisations operate. It is important to assess the consequences and reactions to an incident. Furthermore, it is important that a responsible person is clearly identified so that no stakeholder is left helpless in the face of an unexpected or inappropriate consequence. Finally, it is important to consider the "conditions and limits of validity" of the models used to ensure that the intended use is appropriate.

</details>

---

Q6.2: **Use of predictive models on behalf of third parties**
If your organization provides or operates predictive model-based applications to customers or third parties:

R6.2:  
_(Type: combined)_  
_(Select all response items that correspond to practices in your organization. Caution, some combinations would not be consistent)_

- [ ] 6.2.a Our organization does not provide to its customers or third parties, and does not operate on behalf of third parties, applications based on predictive models developed by machine learning | _(When this answer is selected, others cannot be selected)_
- 6.2.b **A predictive models register** identifies all models or applications used by its customers and/or by the organization on behalf of third parties, we keep it up to date.
- [ ] 6.2.c For each model or application for a customer or a third party we have a defined, identifiable and easily contactable **contact point**
- [ ] 6.2.d For each model or application for a customer or a third party, we systematically carry out a **risk assessment** resulting from possible incidents, failures, biases, etc., in order to identify the risks that may arise.
- [ ] 6.2.e. Monitoring tools are in place to ensure continuous monitoring of ML systems and may trigger alerts directly to the responsible team.
- [ ] 6.2.fe For each model or application for a customer or a third party, we define and test a procedure for suspending the model and a degraded operating mode without the model, in case the model is subject to failure or abnormal behaviour.
- [ ] 6.2.g For each model or application for a client or a third party, we study its [end-to-end genealogy](#section-4---establishing-and-maintaining-a-model-genealogy) and its conditions and limitations of use to understand the model before using it.
- [ ] 6.2.h We provide our customers or operate on their behalf models or applications for **uses in accordance with their conditions and limits of use**

<details>
<summary>Expl6.2:</summary>

Using automatic systems based on models whose rules have been "learned" (and not defined and formalised) questions the way organisations operate. It is important to assess the consequences and reactions to an incident. Furthermore, it is important that a responsible person is clearly identified so that no stakeholder is left helpless in the face of an unexpected or inappropriate consequence. Finally, it is important to consider the "conditions and limits of validity" of the models used to ensure that the intended use is appropriate.

</details>

---

Q6.3: **Managing problematic predictions, workarounds, _human agency_**  
Automatic systems, especially when based on learned predictive models, are used in production generally to gain efficiency. It turns out that by their nature, they occasionally generate undesirable results for the organization and its stakeholders (e.g. wrong prediction), as they will never achieve 100% performance.

R6.3:  
_(Type: combined)_  
-(Select all response items that correspond to practices in your organization. Caution, some combinations would not be consistent)_

- [ ] 6.3.a Our organization does not use predictive models developed by machine learning for its own account or that of its clients, and does not provide its clients with applications based on predictive models [ ] 
- [ ] 6.3.b We integrate into automatic systems based on learned predictive models the functionalities to manage these cases of undesirable outcomes. This is done according to an incident management method, i.e. correcting _ex post_ the undesirable result.
- [ ] 6.3.c We integrate into automatic systems based on learned predictive models the functionalities to manage these cases of undesirable outcomes. This is done _ex ante_, by soliciting a human operator in a number of cases where the confidence interval for the automatic decision is not satisfactory.
- [ ] 6.3.d We set up mechanisms allowing a human operator, under certain defined conditions, to go against a decision of a model if he identifies that the model commits an error.

<details>
<summary> Expl6.3: </summary>

Using automatic systems based on models whose rules have been "learned" (and not defined and formalised) questions the way organisations operate. It is important to preserve the responsiveness and resilience of the organization.

</details>

<details>
<summary>Resources6.3:</summary>

- *[Monitoring Machine Learning Models in Production - A comprehensive guide](https://christophergs.com/machine%20learning/2020/03/14/how-to-monitor-machine-learning-models/)*, ChristopherGS, March 2020

</details>

---


Q6.4: **Transparency to stakeholders interacting with a learned predictive model**  
If your organization uses for its own account, provides to its customers or operates on behalf of its customers applications based on predictive models, with which users can interact, what does your organization put in place to inform users about them?

R6.4:  
_(Type: combined)_  
_(Select all response items that correspond to practices in your organization. Caution, some combinations would not be consistent)_

- [ ] 6.4.a Our organization does not use predictive models developed by machine learning for its own account or that of its clients, and does not provide its clients with applications based on predictive models
- [ ] 6.4.b Users are not informed | _(When this answer is selected, the others cannot be selected)_ _(When this answer is selected, the others cannot be selected)_
- [ ] 6.4.c An information notice is made available in the general conditions of use of the system or an equivalent document, in free access.
- [ ] 6.4.d The use of the system or service is explicit to the user that a learned predictive model is being used.
- [ ] 6.4.e The system or service provides the user with additional information on the results that would have been provided by the system or service in slightly different situations.

<details>
<summary> Expl6.4: <summary>

Using automatic systems based on models whose rules have been "learned" (and not defined and formalised) questions the functioning of organisations but also the relationship of users to digital systems and services. In most cases it is important to inform users that they do not face conventional business rules.

</details>

<details>
<summary>Resources6.4:</summary>

- Counterfactual Explanations without Opening the Black Box: Automated Decisions and the GDPR](https://arxiv.org/abs/1711.00399)*, S. Wachter, B. Mittelstadt, C. Russell, 2018.
- *[Interpretable Machine Learning](https://christophm.github.io/interpretable-ml-book/counterfactual.html)*, C. Molnar, 2020

</details>

---


### Section 7 - Anticipating, Monitoring and Minimizing Externalities of Data Science Activity

The implementation of an automatic system based on a predictive model can generate negative social and environmental externalities. It is essential to be aware of this, as well as to anticipate, seek to monitor and minimise the various negative impacts.

[_[⇧ back to list of sections](#framework-for-assessing-the-maturity-of-an-organization)_]

---

Q7.1: **Impact CO2** 
About the CO2 impact of its data science activity, within your organization:

R7.1:  
_(Type: single response)_  
)_(Select one answer only, best suited to the organization's level of maturity on this topic)_

- [ ] 7.1.a At this stage we have not looked at the CO2 impact of our data science activity or our predictive models.
- [ ] 7.1.b We have defined indicators to know what exactly to measure.
- [ ] 7.1.c We have defined indicators and include their measures in the G2Bs of the models.
- [ ] 7.1.d We have defined indicators and we monitor them regularly.
- [ ] 7.1.e We have defined indicators, we monitor them regularly, and we have set improvement targets.

<details>
<summary> Expl7.1: <summary>

It is important to question and raise awareness of environmental costs.

</details>

<details>
<summary>Resources7.1:</summary>

- [ML Impact Calculator](https://mlco2.github.io/impact/)

</details>

---

Q7.2: **Social impact**
In some cases, the implementation of an automatic system based on a predictive model can generate negative externalities on upstream stakeholders (e.g. annotation of data), and on downstream stakeholders (e.g. automation of certain stations). Whenever you develop or use a predictive model, your organization:

R7.2:  
_(Type: single response)_  
_(Select one answer only, best suited to the organization's level of maturity on this topic)_

- [ ] 7.2.a At this stage we are not looking at the social impact of our data science activity or our predictive models.
- [ ] 7.2.b In some cases we wonder about the social impact
- [ ] 7.2.c We carry out this work of reflection on the social impact of each project.
- [ ] 7.2.d We carry out this social impact analysis for each project and the social impact is documented in the G2B of each model.
- [ ] 7.2.e We carry out this social impact analysis for each project, the social impact is documented in the G2B of each model, and we systematically initiate a dialogue with the relevant stakeholders upstream and downstream.

<details>
<summary> Expl7.2: </summary>

It is important to question and exchange with its stakeholders. This applies both downstream (e.g. automation of certain jobs) and upstream (e.g. data annotation tasks that can sometimes be very violent).

</details>


Q7.3: **Ethical and non-maleficence** 
Within your organization:

R7.3:  
_(Type: combined)_  
_(Select all response items that correspond to practices in your organization. Caution, some combinations would not be consistent)_

- [ ] 7.3.a At this stage we have not yet addressed the ethical dimension.
- [ ] 7.3.b Employees involved in data science activities receive ethics training.
- [ ] 7.3.c Our organization has an ethics policy.

<details>
<summary> Expl7.3:</summary>

Working with large volumes of data, some of which may be sensitive, using automatic systems based on models whose rules have been "learned" (and not defined and formalised) raises questions about how organisations function and the individual responsibility of each person. It is important for the organization to ensure that ethical issues are not unknown to its staff.

</details>

<details>
<summary>Resources7.3:</summary>

- Report *[Ethics and Responsibility of Public Algorithms](https://www.etalab.gouv.fr/wp-content/uploads/2020/01/Rapport-ENA-Ethique-et-responsabilit%C3%A9-des-algorithmes-publics.pdf)*, Etalab / ENA, January 2020
- *[Montreal Declaration for Responsible RN](https://www.declarationmontreal-iaresponsable.com/la-declaration)*
- *[Holberton-Turing Oath](https://www.holbertonturingoath.org/accueil)*
- *[Hippocratic Oath for Data Scientist](https://hippocrate.tech/)*
- *[Future of Life's AI principles](https://futureoflife.org/ai-principles/)*
- *[International Charter for an Inclusive AI](https://charteia.arborus.org/)*, Arborus and Orange

</details>

---
---

## Risks ##

What are the risks that one wishes to prevent in order to be able to talk about _responsible_ data science and _trust_?

Divided into themes:

- EDP: Exposure of Personal or Confidential Data
- PDI: Inappropriate Decision Making by Automatic Systems
- RC: not accountable to its stakeholders in a responsible manner
- SEA: having an irresponsible Social and Environmental Footprint
- TR: transverse
- to be categorized.

| # | Risks | Actual examples or comments |
|:---:|:---|:---|
| | | |
| **EDP** | **Exposure of Personal or Confidential Data** (e.g. personal data or private data of an organization) | |
| EDP-01 | datasets containing personal or confidential data are exposed | [re-identification of anonymized datasets](https://www.wired.com/2007/12/why-anonymous-data-sometimes-isnt/); [Nature article](https://www.nature.com/articles/s41467-019-10933-3/): "Using our model, we find that 99.98% of Americans would be correctly re-identified in any dataset using 15 demographic attributes."|
| EDP-02 | a machine learning algorithm is maliciously used to extract or expose personal or confidential data from a training or test dataset | |
| EDP-03 | malicious exploitation of a predictive model exposes personal or confidential data | [retro-engineering of algorithm results](https://www.abc.net.au/news/2019-03-01/abs-census-vulnerability/10857236) |
| EDP-04 | regulatory provisions pose risks, or a regulatory change increases the risk of exposure of personal or confidential data | Cloud Act; [FATCA](https://www.cnil.fr/fr/cnil-direct/question/loi-fatca-que-faire) in contradiction with European law; [NBC - HDH Warning](https://www.cnb.avocat.fr/sites/default/files/11.cnb-mo2020-01-11_ldh_health_data_hubfinal-p.pdf) |
| | | |
| **PDI** | **Inappropriate Decision Making by Automatic Systems** that would be prejudicial to individuals or organizations. Inappropriate means unfounded, unjust or illegitimate. |
| PDI-01 | inappropriate decision making due to discriminatory biases in training or test data | [Apple Card case](https://twitter.com/dhh/status/1192540900393705474); [Amazon HR algorithm](https://www.lefigaro.fr/social/2018/10/11/20011-20181011ARTFIG00096-le-logiciel-de-recrutement-d-amazon-n-aimait-pas-les-femmes.php); [facial recognition](https://www.thesun.co.uk/news/5182512/chinese-users-claim-iphonex-face-recognition-cant-tell-them-apart/); [bias in visual recognition systems](https://arxiv.org/pdf/1902.11097.pdf) | [bias in visual recognition systems](https://arxiv.org/pdf/1902.11097.pdf)
| PDI-02 | inappropriate decision making due to poisoned data (maliciously, or due to diffuse, poorly understood phenomena) | the example of [social cooling](https://usbeketrica.com/article/le-social-cooling-symptome-numerique-de-la-surveillance-de-masse) |
| PDI-03 | inappropriate decision making due to the use of synthetic data | _# this risk is poorly identified/defined at this stage #_ |
| PDI-04 | inappropriate decision making due to discriminatory biases due to the architecture or design of the learning algorithm and/or model itself [word embedding templates](https://arxiv.org/abs/1607.06520), [doc2vec](https://www.pnas.org/content/115/16/E3635); use of directly protected variables |
| PDI-05 | the use of predictive models in contexts for which they do not perform sufficiently well, are not relevant or even dangerous, are not predicted and validated (where their actual performance is insufficient compared to what is stated or expected) | [example of Google Flu Trends in health](https://science.sciencemag.org/content/343/6176/1203); [bias and limited performance of the COMPAS model for predicting recidivism](https://advances.sciencemag.org/content/4/1/eaao5580) |
| PDI-06 | the use of models that have degenerated or _drifted_ over time (for example, in cases of continuous learning, when the new input data comes, even indirectly, from situations in which the model has been used) | cases to be identified (problems with measurement sensors in predictive maintenance, trading...) |
| PDI-07 | Adversarial use of a predictive model in a manner detrimental to individuals or organizations | [Three Small Stickers in Intersection Can Cause Tesla Autopilot to Swerve Into Wrong Lane](https://spectrum.ieee.org/cars-that-think/transportation/self-driving/three-small-stickers-on-road-can-steer-tesla-autopilot-into-oncoming-lane) |
| | | |
| **RC** | **Does not Account responsibly to its stakeholders** for the consequences of using predictive models | |
| RC-01 | in the case of an incident with or caused by a predictive model, not having an identified individual or legal entity to whom to hold accountable | [Steve Wozniak's case with the Apple Card](https://twitter.com/stevewoz/status/1193330241478901760) |
| RC-02 | in the case of an incident with or due to a predictive model: for the actor implementing and operating the model, not knowing how to react to a request to interpret and explain a challenged prediction | [Facebook's automatic censoring algorithms were less effective in the Christchurch attack than with the EI videos: what exactly do they detect](https://techcrunch.com/2019/03/21/facebooks-ai-couldnt-spot-mass-murder/); [An Algorithm that grants Freedom, or Takes it away](https://www.nytimes.com/2020/02/06/technology/predictive-algorithms-crime.html) |
| RC-03 | in the case of an incident with or due to a predictive model: for the actor who implements and operates the model, no longer being able to provide a critical service | case to be identified |
| RC-04 | within an organization that uses automatic systems based on predictive models, not knowing or not being able to easily identify who is responsible for these systems | |
| | | |
| **ESE** | **have an irresponsible Social and Environmental Footprint** | | |
| ESE-01 | not knowing or being concerned about the energy or environmental cost of developing and using a model, or that it is disproportionate to the target use of the model | [AlphaGo in kW vs. 20W for a human](https://deepmind.com/blog/article/alphago-zero-starting-scratch) ; [ML Impact Calculator](https://mlco2.github.io/impact/) | [AlphaGo in kW vs. 20W for a human](https://deepmind.com/blog/article/alphago-zero-starting-scratch) ; [ML Impact Calculator](https://mlco2.github.io/impact/) | 
| ESE-02 | not anticipating the social impacts of the development or implementation of an automatic system based on a predictive model | upstream for the production of annotated data, for example, downstream for the evolution of impacted activities |
| ESE-03 | not anticipating negative/hazardous effects or misuses of a model at the design stage | [Implication analysis and release strategy of gpt2 by OpenAI](https://openai.com/blog/better-language-models/) |
| | | |
| **TR** | **Transverse** | |
| TR-01 | not mastering the negative consequences of using a given model due to the lack of "global governance" throughout the end-to-end value chain (data, design, training, validation, operation) | |
| TR-02 | not being able to control the consequences of using a model due to lack of knowledge of its genealogy and lack of control over its nominal conditions of use | models that become references and/or supplied by third parties | |
| | | |
| | **various - to be categorized** | |
| | getting "stolen" a model by multiple inferences | |
| | getting "stolen" from the computation time by _adversarial reprogramming_ | |
| | | placement of job offers on the flows of users selected by a predictive model: does it make sense to ask about a risk of discrimination, or is it analogous to a headhunter who decides to call candidates who interest him in a discretionary way? |

## Themes of the evaluation framework

Proposals of themes to structure the good practices and risk prevention measures that make up the evaluation reference framework:

| # | Themes | Descriptions |
|:---:|:---|:---|
| T1 | **Protecting personal or confidential data** | The use of personal or confidential data carries with it the risk of exposure of such data, which can have very detrimental consequences for the producers, managers, or subjects of such data. Therefore, they must be protected, the risk of exposure must be minimized. |
| Q2 | **Preventing undesirable biases** | The use of predictive models developed from historical data can be detrimental when historical data describe undesirable phenomena. It seems essential to question this risk and to study the nature of the data used and what they represent. | The risk of a risk of a loss of data is a major concern. |
| Q3 | **Reviews performance rigorously** | The performance score of a predictive model is critical to its adoption in products, systems or processes. Performance evaluation must therefore be rigorous. A specification of the equity sought between populations must also be defined. Indeed, the fairness of a model can [be defined in several ways that may be incompatible with each other](https://papers.nips.cc/paper/6995-counterfactual-fairness), and the interpretation of performance scores must therefore be done within the framework of one of these definitions. |
| T4 | **Establish and maintain a genealogy of models** | A predictive model is a complex computer object that can evolve over time. Tracing the stages of its elaboration and its evolution makes it possible to constitute a form of **genealogy**, a prerequisite for **reproducing or auditing** a model. |
| T5 | **Guaranteeing the chain of responsibility of models** | A predictive model can be used as an automatic system, whose rules of operation are not written _in extenso_ and do not lend themselves or badly to be explained, debated, adjusted. Efforts are needed on **interpretation and explanation** of the choices made using these systems. It also appears essential to ensure a clear chain of responsibility, of natural or legal persons, for each model. |
| T6 | **Anticipate, monitor and minimise the negative externalities of the data science activity** | The implementation of an automatic system based on a predictive model can generate negative social and environmental externalities. It is essential to be aware of this, as well as to anticipate, seek to monitor and minimise the various negative impacts.|
