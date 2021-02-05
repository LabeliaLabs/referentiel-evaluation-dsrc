# Responsible and Trustworthy Data Science - Evaluation framework

The [evaluation framework](#evaluation-framework-to-assess-the-maturity-of-an-organisation) below is the result of the participatory work initiated in the spring of 2019 by Substra Foundation and ongoing since then. It is based on the identification of the [risks](#risks) that we are trying to prevent by aiming for a responsible and trustworthy practice of data science, and best practices to mitigate them. It also brings together for each topic technical resources that can be good entry points for interested organisations.

## Evaluation framework to assess the maturity of an organisation

The evaluation is composed of the following 6 sections:

- [Section 1 - Protecting personal or confidential data](#section-1---protecting-personal-or-confidential-data)
- [Section 2 - Preventing bias, developing non-discriminatory models](#section-2---preventing-bias-developing-non-discriminatory-models)
- [Section 3 - Assessing model performance rigorously](#section-3---assessing-model-performance-rigorously)
- [Section 4 - Ensuring model reproducibility and establishing the chain of accountability](#section-4---ensuring-model-reproducibility-and-establishing-the-chain-of-accountability)
- [Section 5 - Using models responsibly and in confidence](#section-5---using-models-responsibly-and-in-confidence)
- [Section 6 - Anticipating, monitoring and minimising the negative externalities of data science activities](#section-6---anticipating-monitoring-and-minimising-the-negative-externalities-of-data-science-activities)

---

### Section 1 - Protecting personal or confidential data

The use of personal or confidential data carries the risk of exposure of such data, which can have very detrimental consequences for the producers, controllers or subjects of such data. Particularly in data science projects, they must therefore be protected and the risks of their leakage or exposure must be minimised.

[_[⇧ back to the list of sections](#evaluation-framework-to-assess-the-maturity-of-an-organisation)_]  
[_[⇩ next section](#section-2---preventing-bias-developing-non-discriminatory-models)

---

Q1.1: **Applicable legislation and contractual requirements - Identification**  
With regard to personal or confidential data, the legal, statutory, regulatory and contractual requirements in force and concerning your organisation are:

R1.1 :  
_(Type: single answer)_  
_(Select one answer only, which best corresponds to the level of maturity of the organisation on this topic)_

- [ ] 1.1.a Not yet identified
- [ ] 1.1.b Partially identified or in the process of identification
- [ ] 1.1.c Identified
- [ ] 1.1.d Identified and known by our collaborators
- [ ] 1.1.e Identified, documented and known by our collaborators

<details>
<summary>Expl1.1 :</summary>

It is crucial to put in place processes to know and follow the evolution of applicable regulations (very specific in certain fields, for example in the banking sector), as well as to document the approaches and choices made to comply with each data science project. Interesting example(s) : [Welfare surveillance system violates human rights, Dutch court rules](https://www.theguardian.com/technology/2020/feb/05/welfare-surveillance-system-violates-human-rights-dutch-court-rules).

</details>

<details>
<summary>Resources1.1 :</summary>

- (Official report) [Big data, artificial intelligence, machine learning and data protection](https://ico.org.uk/media/for-organisations/documents/2013559/big-data-ai-ml-and-data-protection.pdf), EU Information Commissioner's Office, 2017
- (Web article) [Artificial Intelligence and the GDPR: how do they interact](https://www.avocats-mathias.com/technologies-avancees/artificial-intelligence-gdpr), Mathias Avocats, November 2017
- (Web article) [How to develop Artificial Intelligence that is GDPR-friendly](https://techgdpr.com/blog/develop-artificial-intelligence-ai-gdpr-friendly/), Tech GDRP blog, February 2019
- (Video) [What is the impact of GDPR on AI and Machine Learning](https://www.youtube.com/watch?v=RLEtyfmsfs4&app=desktop), SwissAI Machine Learning Meetup, September 2018
- (Technical guide) [L'Atelier RGPD](https://atelier-rgpd.cnil.fr/), online training offered by the CNIL (French data protection authority), in French

</details>

---

Q1.2: **Applicable legislation and contractual requirements - Compliance approach**  
In order to meet these requirements, the approach adopted by your organisation is:

R1.2 :  
_(Type: single answer)_  
_(Select one answer only, which best corresponds to the level of maturity of the organisation on this topic)_

- [ ] 1.2.a Informal, based on individual responsibility and competence
- [ ] 1.2.b Formalized and accessible to all collaborators
- [ ] 1.2.c Formalized and known by collaborators
- [ ] 1.2.d Formalized, known by employees, documented for each processing of personal or confidential data

<details>
<summary>Expl1.2 :</summary>

It is a question of questioning the management of personal or confidential data (storage, access, transfer, protection, responsibilities...), and documenting the choices made.

</details>

---

Q1.3: **Applicable legislation and contractual requirements - Regulatory surveillance**  
Is a regulatory surveillance process in place, either internally or via a specialised service provider, to find out about applicable changes that have an impact on your organisation?

R1.3 :  
_(Type: single answer)_  
_(Select one answer only, which best corresponds to the level of maturity of the organisation on this topic)_

- [ ] 1.3.a We do not really monitor the regulatory environment
- [ ] 1.3.b We keep an informal watch, each employee sends back information via internal communication channels
- [ ] 1.3.c We have a formal surveillance, with identified collaborators in charge and a documented process

<details>
<summary>Expl1.3 :</summary>

In addition to identifying regulations and compliance approaches, it is important to set up a surveillance processe to know and follow **the evolution** of applicable regulations (which can be very specific in certain sectors). Interesting example(s) : [Welfare surveillance system violates human rights, Dutch court rules](https://www.theguardian.com/technology/2020/feb/05/welfare-surveillance-system-violates-human-rights-dutch-court-rules).

</details>

---

Q1.4: **Applicable legislation and contractual requirements - Auditing and certification**  
Has the organisation's compliance with personal and confidential data requirements been audited and is it recognised by a certification, label or equivalent?

R1.4 :  
_(Type: single answer)_  
_(Select one answer only, which best corresponds to the level of maturity of the organisation on this topic)_

- [ ] 1.4.a Yes
- [ ] 1.4.b No

<details>
<summary>Expl1.4 :</summary>

In many sectors there are specific compliance requirements. It is generally possible to formalise an organisation's compliance through certification or a specialised audit, or by obtaining a label.

</details>

---

Q1.5: **Data minimisation principle**  
In data science projects, the data minimisation principle should guide the collection and use of personal or confidential data. How is it implemented in your organisation?

R1.5 :  
_(Type: single answer)_  
_(Select one answer only, which best corresponds to the level of maturity of the organisation on this topic)_

- [ ] 1.5.a We take care not to use any personal or confidential data. We are not concerned by this risk area
- [ ] 1.5.b We need to use personal or confidential data in certain projects and the data minimisation principle is then systematically applied
- [ ] 1.5.c Employees are aware of the data minimisation principle and generally apply it
- [ ] 1.5.d The "who can do the most can do the least" reflex with regard to data still exists here and there within our organisation. In some projects, we keep datasets that are much richer in personal and confidential data than what is strictly useful to the project

<details>
<summary>Expl1.5 :</summary>

The data minimisation principle is sometimes also referred to as "privacy by design". It is one of the pillars of the RGPD in the European Union.

</details>
  
---

_The following elements within this section apply only to organisations that did not select the first response to R1.5. Organisations not concerned are therefore invited to move on to [Section 2](#section-2---preventing-bias-developing-non-discriminatory-models)._

---

Q1.6: **Project involving new processing of personal or confidential data**  
_(Condition: R1.5 <> 1.5.a)_  
For each processing of personal or confidential data required in the framework of a data science project within your organisation:

R1.6 :  
_(Type: multiple responses possible)_  
_(Select all the answer items that correspond to practices in your organisation)_

- [ ] 1.6.a We elaborate a Privacy Impact Assessment (PIA)
- [ ] 1.6.b We implement data protection measures (in particular concerning the transfer, storage and access to the data concerned)
- [ ] 1.6.c We contractualise relations with suppliers and customers and the responsibilities that arise from them
- [ ] 1.6.d We have not yet set up an organised approach to these subjects

<details>
<summary>Expl1.6 :</summary>

The *Privacy Impact Assessment* (PIA) is a method for assessing the impact of a data processing, similar to traditional risk assessment methods. In certain cases, for example where a processing operation presents high risks to the rights and freedoms of natural persons, the GDPR makes it obligatory to carry out an PIA before the processing operation is carried out.

</details>

---

Q1.7: **Machine Learning security - Knowledge level**  
_(Condition: R1.5 <> 1.5.a)_  
Machine Learning security (_ML security_) is a constantly evolving field. In some cases, predictive models learned from confidential data may reveal elements of that confidential data (see articles cited in resources). Within your organisation, the general level of knowledge of collaborators working on data science projects about vulnerabilities related to ML models and the techniques to mitigate them is:

R1.7 :  
_(Type: single answer)_  
_(Select one answer only, which best corresponds to the level of maturity of the organisation on this topic)_

- [ ] 1.7.a Complete beginner
- [ ] 1.7.b Basic
- [ ] 1.7.c Confirmed
- [ ] 1.7.d Expert

<details>
<summary>Expl1.7 :</summary>

The state of the art in ML security is constantly evolving. While it is impossible to guard against all vulnerabilities at all times, it is crucial to be aware of them and to keep a watch on them. The article [Demystifying the Membership Inference Attack](https://medium.com/disaitek/demystifying-the-membership-inference-attack-e33e510a0c39) is for example an interesting entry point in the context of sensitive data.

</details>

<details>
<Summary>Ressources1.7 :</summary>

- (Technical guide) *[Privacy Enhancing Technologies Decision Tree (v2)](https://www.private-ai.ca/PETs_Decision_Tree.png)*, Private AI, 2020
- (Web article) *[The secret-sharer: evaluating and testing unintended memorization in neural networks](https://blog.acolyer.org/2019/09/23/the-secret-sharer/)*, A. Colyer, 2019
- (Academic paper) *[Membership Inference Attacks against Machine Learning Models](https://arxiv.org/abs/1610.05820)*, R. Shokri, M. Stronati, C. Song, V. Shmatikov, 2017
- (Software & Tools) *[ML Privacy Meter](https://github.com/privacytrustlab/ml_privacy_meter): a tool to quantify the privacy risks of machine learning models with respect to inference attacks*.
- (Web article) *[Demystifying the membership inference attack](https://medium.com/disaitek/demystifying-the-membership-inference-attack-e33e510a0c39)*, Disaitek, 2019
- (Academic paper) *[Inverting Gradients - How easy is it to break privacy in federated learning](https://arxiv.org/abs/2003.14053)*, J. Geiping, H. Bauermeister, H. Dröge, M. Moeller, 2020
- (Web article) *[Top Five ML risks](https://github.com/OWASP/Top-5-Machine-Learning-Risks/blob/master/Top%205%20Machine%20Learning%20Risks.md)*, OWASP
- (Software & Tools) Tools for *differential privacy*: Google *[differential privacy library](https://github.com/google/differential-privacy)*, and the Python [PyDP](https://github.com/OpenMined/PyDP) wrapper from OpenMined
- (Web article) The *distillation* of a model, in addition to the compression it provides, can be used as a measure to protect the model and the training data used, see for example *[Knowledge Distillation: Simplified](https://towardsdatascience.com/knowledge-distillation-simplified-dd4973dbc764)*, Towards Data Science, 2019.
- (Academic paper) *[Distilling the Knowledge in a Neural Network](https://arxiv.org/abs/1503.02531)*, G. Hinton, O. Vinyals, J. Dean, 2015

</details>

---

Q1.8: **Machine Learning security - Implementation**  
_(Condition: R1.5 <> 1.5.a)_  
Still on the subject of vulnerabilities related to ML models and techniques to mitigate them:

R1.8 :  
_(Type: multiple responses possible)_  
_(Select all the answer items that correspond to practices in your organisation)_

- [ ] 1.8.a We keep a technical watch on the main attacks and measures to mitigate them
- [ ] 1.8.b Employees receive regular information and training to help them develop their skills in this area
- [ ] 1.8.c In some projects, we implement specific techniques to reduce the risks associated with the models we develop (for example: differential privacy, distillation, etc.)
- [ ] 1.8.d On each project, the vulnerabilities that apply to it and the techniques implemented are documented (e.g. in the end-to-end genealogy of each model, see Section 4 and Element 4.1 for more information on this concept)
- [ ] 1.8.e We have not yet set up an organised approach to these subjects

<details>
<summary>Expl1.8 :</summary>

The state of the art in ML security is constantly evolving. While it is impossible to guard against all vulnerabilities at all times, it is crucial to be aware of them and to keep a watch on them. The article [Demystifying the Membership Inference Attack](https://medium.com/disaitek/demystifying-the-membership-inference-attack-e33e510a0c39) is for example an interesting entry point in the context of sensitive data.

Depending on the level of risk and sensitivity of the projects, certain technical approaches to guard against them will be selected and implemented. It is important to follow the evolution of research and state-of-the-art practices, and to document the choices made. The notion of "end-to-end genealogy" is introduced here.

</details>

<details>
<summary>Resources1.8 :</summary>

- (Technical guide) *[Privacy Enhancing Technologies Decision Tree (v2)](https://www.private-ai.ca/PETs_Decision_Tree.png)*, Private AI, 2020
- (Web article) *[The secret-sharer: evaluating and testing unintended memorization in neural networks](https://blog.acolyer.org/2019/09/23/the-secret-sharer/)*, A. Colyer, 2019
- (Academic paper) *[Membership Inference Attacks against Machine Learning Models](https://arxiv.org/abs/1610.05820)*, R. Shokri, M. Stronati, C. Song, V. Shmatikov, 2017
- (Software & Tools) *[ML Privacy Meter](https://github.com/privacytrustlab/ml_privacy_meter): a tool to quantify the privacy risks of machine learning models with respect to inference attacks*.
- (Web article) *[Demystifying the membership inference attack](https://medium.com/disaitek/demystifying-the-membership-inference-attack-e33e510a0c39)*, Disaitek, 2019
- (Academic paper) *[Inverting Gradients - How easy is it to break privacy in federated learning](https://arxiv.org/abs/2003.14053)*, J. Geiping, H. Bauermeister, H. Dröge, M. Moeller, 2020
- (Web article) *[Top Five ML risks](https://github.com/OWASP/Top-5-Machine-Learning-Risks/blob/master/Top%205%20Machine%20Learning%20Risks.md)*, OWASP
- (Software & Tools) Tools for *differential privacy*: Google *[differential privacy library](https://github.com/google/differential-privacy)*, and the Python [PyDP](https://github.com/OpenMined/PyDP) wrapper from OpenMined
- (Web article) The *distillation* of a model, in addition to the compression it provides, can be used as a measure to protect the model and the training data used, see for example *[Knowledge Distillation: Simplified](https://towardsdatascience.com/knowledge-distillation-simplified-dd4973dbc764)*, Towards Data Science, 2019.
- (Academic paper) *[Distilling the Knowledge in a Neural Network](https://arxiv.org/abs/1503.02531)*, G. Hinton, O. Vinyals, J. Dean, 2015

</details>

---

Q1.9: **Notification of safety incidents to the regulatory authorities**  
_(Condition: R1.5 <> 1.5.a)_  
In the event that a model that the organisation has developed is used or accessible by one or more external stakeholders, and a new vulnerability is published, there is a risk that it may apply to them and thus create a risk of exposure of personal or confidential data:

R1.9 :  
_(Type: multiple responses possible)_  
_(Select all the answer items that correspond to practices in your organisation)_

- [ ] 1.9.a We have a process describing the course of action in such cases
- [ ] 1.9.b Our process includes communication to the stakeholders in question
- [ ] 1.9.c Our process references the authorities to whom we must report
- [ ] 1.9.d We have not yet put in place a procedure for such cases

<details>
<summary>Expl1.9 :</summary>

In some sectors there are obligations to report safety incidents to the regulatory authorities (e.g. in France: CNIL, ANSSI, ARS, etc.). An interesting entry point: [Notifications of safety incidents to regulatory authorities: how to organise and who to contact](https://www.cnil.fr/fr/notifications-dincidents-de-securite-aux-autorites-de-regulation-comment-sorganiser-et-qui-sadresser) on the CNIL website.

</details>

---
---

### Section 2 - Preventing bias, developing non-discriminatory models

The use of predictive models learned from historical data can be counterproductive when historical data are contaminated by problematic phenomena (e.g. quality of certain data points, non-comparable data, social phenomena undesirable due to the time period, etc.). A key challenge for responsible and trustworthy data science is to respect the principle of diversity, non-discrimination and equity (described for example in section 1.5 of the EU [Ethics Guidelines for Trustworthy AI](https://ec.europa.eu/newsroom/dae/document.cfm?doc_id=60419)). It is therefore essential to question this risk and to study the nature of the data used, the conditions under which they were produced and collected, and what they represent.
Among other things, in some cases a specification of the equity sought between populations must also be defined. The equity of a model can [be defined in several ways that may be inconsistent with each other](https://papers.nips.cc/paper/6995-counterfactual-fairness), and the interpretation of performance scores must therefore be made within the framework of one of these definitions.

[_[⇧ back to the list of sections](#evaluation-framework-to-assess-the-maturity-of-an-organisation)_]  
[_[⇩ next section](#section-3---assessing-model-performance-rigorously)_]

---

Q2.1: **Analysis of the training data**  
Within data science projects and when developing training datasets, reflection and research on problematic phenomena (e.g. quality of certain data points, data that are not comparable due to recording tools or processes, social phenomena that are undesirable due to time, context, etc.) can be crucial to prevent bias that undermines the principle of non-discrimination, diversity and equity. Your organisation:

R2.1 :  
_(Type: single answer)_  
_(Select one answer only, which best corresponds to the level of maturity of the organisation on this topic)_

- [ ] 2.1.a Operates informally on this subject and relies on the practices of each collaborator involved
- [ ] 2.1.b Does not have a documented approach to the subject, but the collaborators involved are trained on the risks and best practices on the subject
- [ ] 2.1.c Has a documented approach that is systematically implemented

<details>
<summary>Expl2.1 :</summary>

It is a question of ensuring that oneself considers these subjects and therefore questions the training data, the way in which it was produced, etc.

</details>

<details>
<summary>Ressources2.1 :</summary>

- (Web article) *[Hidden Bias](https://pair.withgoogle.com/explorables/hidden-bias/)* explorable from [PAIR](https://pair.withgoogle.com/)
- (Technical guide) *[Tour of Data Sampling Methods for Imbalanced Classification](https://machinelearningmastery.com/data-sampling-methods-for-imbalanced-classification/)*

</details>

---

Q2.2: **Risk of discrimination against certain social groups**  
Is your organisation involved in cases where predictive models are used in thematic environments where there are risks of discrimination against certain social groups (gender, origin, age, etc.)? (The next assessment element is dedicated to these cases):

R2.2 :  
_(Type: single answer)_  
_(Select one answer only, which best corresponds to the level of maturity of the organisation on this topic)_

- [ ] 2.2.a Concerned
- [ ] 2.2.b Not concerned

---

_The following items within this section apply only to organisations that have selected the "Concerned" response in R2.2. Organisations not involved are therefore invited to move on to [Section 3](#section-3---assessing-model-performance-rigorously)._

---

Q2.3 : **Preventing discriminatory bias**  
_(Condition: R2.2 <> 2.2.b)_  
In cases where the predictive models your organisation develops are used in thematic environments where there is a risk of discrimination against certain social groups (gender, origin, age, etc.):

R2.3 :  
_(Type: multiple responses possible)_  
_(Select all the answer items that correspond to practices in your organisation)_

- [ ] 2.3.a We pay particular attention to the identification of protected attributes and their possible proxies (e.g. studying one by one the variables used as model inputs to identify the correlations they might have with sensitive data)
- [ ] 2.3.b We carry out evaluations on test data from different sub-populations in order to identify possible problematic biases
- [ ] 2.3.c We select and implement one or more justice and equity measure(s) (_fairness metrics_)
- [ ] 2.3.d We use _data augmentation_ or _re-weighting_ approaches to reduce possible biases in the data sets
- [ ] 2.3.e The above practices that we implement are duly documented and integrated into the end-to-end genealogy of the models concerned
- [ ] 2.3.f We have not yet put in place any such measures

<details>
<summary>Expl2.3 :</summary>

It is a question of systematically questioning, for each data science project and according to the objective and target use of the model that one wants to develop, the features that may directly or indirectly be the source of a risk of discriminatory bias. The term "protected attribute" or "protected variable" is used to refer to attributes whose values define sub-populations at risk of discrimination.
Complement on the use of synthetic data and _data augmentation_, _re-weighting_ approaches in order to reduce possible biases in the data sets: when such techniques are used it is important to make them explicit, otherwise there is a risk of losing information on how a model was developed.

</details>

<details>
<Summary>Resources2.3 :/Summary>

- (Web article) *[Unfair biases in Machine Learning: what, why, where and how to obliterate them](https://www.mlsecurity.ai/post/unfair-biases-in-machine-learning-what-why-where-and-how-to-obliterate-them)*, blog ML Security, P. Irolla, April 2020
- (Web article) [Awful AI](https://github.com/daviddao/awful-ai), a registry of worrying AI services or projects, David Dao
- (Technical guide) *[A Tutorial on Fairness in Machine Learning](https://towardsdatascience.com/a-tutorial-on-fairness-in-machine-learning-3ff8ba1040cb)*, Towards Data Science blog, Z. Zhong, October 2018
- (Web article) *[Measuring fairness](https://pair.withgoogle.com/explorables/measuring-fairness)* explorable, [PAIR](https://pair.withgoogle.com/)
- (Software & Tools) *[AI Fairness 360](https://developer.ibm.com/technologies/artificial-intelligence/projects/ai-fairness-360/): an open source software toolkit that can help detect and remove bias in machine learning models*, IBM
- (Academic paper) *Fairness metrics* : *[counterfactual fairness](https://papers.nips.cc/paper/6995-counterfactual-fairness)*
- (Academic paper) *Fairness metrics* : *[adversarial debiaising](https://arxiv.org/pdf/1801.07593.pdf)*
- (Technical guide) Book *Fair ML* : *[Fairness and machine learning - Limitations and opportunities](https://fairmlbook.org/)*, Solon Barocas, Moritz Hardt, Arvind Narayanan, December 2019

</details>

---
---

### Section 3 - Assessing model performance rigorously

The performance of the models is crucial for their adoption in products, systems or processes. Performance evaluation must therefore be rigorous.

[_[⇧ back to the list of sections](#evaluation-framework-to-assess-the-maturity-of-an-organisation)_]  
[_[⇩ next section](#section-4---ensuring-model-reproducibility-and-establishing-the-chain-of-accountability)_]

---

Q3.1: **Separation of test datasets**  
In data science projects and when developing test datasets, it is of utmost importance to ensure non-contamination by training data. Your organisation:

R3.1 :  
_(Type: multiple responses possible)_  
_(Select all response items that correspond to practices in your organisation. Please note that some combinations would not be coherent)_

- [ ] 3.1.a Operates informally on this subject and relies on the competence and responsibility of the collaborators involved
- [ ] 3.1.b Has a documented and systematically implemented approach to isolating test datasets
- [ ] 3.1.c Uses a tool for versioning and tracing the training and test datasets used, thus enabling the non-contamination of test data to be checked or audited at a later stage
- [ ] 3.1.d Systematically plans two or more sets of test data to increase resilience

<details>
<summary>Expl3.1 :</summary>

Ensuring that training and test datasets are kept separated is a principle known and mastered by most organisations. It can however be tricky in some particular configurations (e.g. continuous learning, distributed learning *privacy-preserving*...).

</details>

---

Q3.2: **Privacy-preserving distributed learning projects**  
In the case of data science projects based on distributed or federated learning on multiple datasets and whose confidentiality must be preserved:

R3.2 :  
_(Type: single answer)_  
_(Select one answer only, which best corresponds to the level of maturity of the organisation on this topic)_

- [ ] 3.2.a We do not participate in *privacy-preserving* distributed learning projects | _(Concerned / Not concerned)_
- [ ] 3.2.b We master and implement approaches to develop test datasets in such a way that there is no cross-contamination between training and test data from different partners
- [ ] 3.2.c At this stage we do not master the methods for developing test datasets in such a way that there is no cross-contamination between training and test data from the different partners

<details>
<summary>Expl3.2 :</summary>

In this type of distributed learning project under conditions where the data is kept confidential, the question arises of how to compose a test dataset, making sure that it does not also appear in the training dataset (e.g. at another partner's premises).

</details>

<details>
<Summary>Resources3.2 :</summary>

- (Academic paper) [Stratified cross-validation for unbiased and privacy-preserving federated learning](https://arxiv.org/abs/2001.08090), R. Bey, R. Goussault, M. Benchoufi, R. Porcher, January 2020

</details>

---

Q3.3 : **Analysis of validation and test data**  
Within data science projects and when developing validation or test datasets, reflection and research on problematic phenomena (e.g. quality of certain data points, data that are not comparable due to recording tools or processes, social phenomena that are undesirable due to time, context, etc.) can be crucial for the meaning of performance scores. Your organisation:

R3.3 :  
_(Type: single answer)_  
_(Select one answer only, which best corresponds to the level of maturity of the organisation on this topic)_

- [ ] 3.3.a Operates informally on this subject and relies on the practice of each collaborator member involved
- [ ] 3.3.b Does not have a documented approach to the subject, but the collaborators involved are trained on the risks and best practices on the subject
- [ ] 3.3.c Has a documented approach that is systematically implemented

<details>
<summary>Expl3.3 :</summary>

The use of predictive models that have been validated and tested on historical data can be counterproductive when the historical data in question is contaminated by problematic phenomena. It seems essential to question this risk and to study the nature of the data used, the conditions under which they were produced and assembled, and what they represent.

</details>

---


Q3.4: **Performance validation**  
Does your organisation implement the following approaches:

R3.4 :  
_(Type: multiple responses possible)_
_(Select all the answer items that correspond to practices in your organisation)_

- [ ] 3.4.a When developing a model, we choose the performance metric(s) prior to actually training the model, from among the most standard metrics possible
- [ ] 3.4.b The implementation of robustness metrics is considered and evaluated for each modelling project, and applied by default in cases where the input data may be subject to fine-grain alterations (e.g. images, sounds)
- 3.4.c The above practices that we implement are documented and integrated into the end-to-end genealogy of the models concerned, including the performance metrics chosen
- 3.4.d We have not yet introduced any such measures

<details>
<summary>Expl3.4 :</summary>

On choosing metrics upstream, see for example the risk of *[p-hacking / data dredging](https://en.wikipedia.org/wiki/Data_dredging)*.
On robustness, an intuitive definition is that a model is robust when its performance is stable when the input data is disturbed. For more information see the technical resources indicated.

</details>

<details>
<Summary>Resources3.4 :/Summary>

- (Web article) *[The Comprehensive Guide to Model Validation Framework: What is a Robust Machine Learning Model?](https://medium.com/@ODSC/the-comprehensive-guide-to-model-validation-framework-what-is-a-robust-machine-learning-model-7bdbc41c1702)*, Open Data Science, March 2020
- (Web article) *[Testing Robustness Against Unforeseen Adversaries](https://openai.com/blog/testing-robustness/)*, Open AI, August 2019
- (Academic paper) *Robustness metrics* : *[noise sensitivity score](https://arxiv.org/abs/1806.01477)*.
- (Technical guide) *[Adversarial Robustness - Theory and Practice](https://adversarial-ml-tutorial.org/)*, Z. Kolter and A. Madry

</details>

---

Q3.5: **Monitoring model performance over time**  
In cases where predictive models developed by your organisation are used in production systems:

R3.5 :  
_(Type: multiple responses possible)_
_(Select all response items that correspond to practices in your organisation. Please note that some combinations would not be coherent)_

- [ ] 3.5.a The models we develop are not used in production systems | _(Concerned / Not concerned)_
- [ ] 3.5.b Performance is systematically re-evaluated when the model is updated
- [ ] 3.5.c Performance is systematically re-evaluated when the context in which the model is used evolves, which may create a risk on the performance of the model due to the evolution of the input data space
- [ ] 3.5.d The distribution of input data is monitored, and performance is regularly re-evaluated on the basis of updated test data
- [ ] 3.5.e Random checks are carried out on predictions to check their consistency
- [ ] 3.5.f We do not systematically set up this type of measure

<details>
<summary>Expl3.5 :</summary>

Even on a stable model, there is a risk that the input data will no longer remain in the target distribution after a certain time (population & distribution), for example, a variable that would no longer be filled in at the same frequency as before by users in an IS. It is therefore necessary to regularly re-evaluate the performance of a model used in its context of use.
Monitoring the performance of models over time is also particularly important in cases of continuous learning, where there is a risk of model degeneration.

</details>

<details>
<Summary>Resources3.5 :/Summary>

- (Technical guide) *[Continuous delivery for machine learning](https://martinfowler.com/articles/cd4ml.html)*, D. Sato, A. Wider, C. Windheuser, September 2019
- (Technical guide) *[Monitoring Machine Learning Models in Production - A comprehensive guide](https://christophergs.com/machine%20learning/2020/03/14/how-to-monitor-machine-learning-models/)*, Christopher Samiullah, March 2020
- (Web article) *[Google's medical AI was super accurate in a lab. Real life was a different story](https://www.technologyreview.com/2020/04/27/1000658/google-medical-ai-accurate-lab-real-life-clinic-covid-diabetes-retina-disease/)*, MIT Technology Review

</details>

---


---

Q3.6: **Decision making and ranges of indecision**  
For the definition of decision thresholds for models or automatic systems based on them, your organisation:

R3.6 :  
_(Type: multiple responses possible)_
_(Select all response items that correspond to practices in your organisation. Please note that some combinations would not be coherent)_

- [ ] 3.6.a Operates informally on this subject and relies on the competence and responsibility of the collaborators involved
- [ ] 3.6.b Has a documented approach that is systematically implemented
- [ ] 3.6.c Takes into account the possibility of maintaining ranges of indecision in certain cases
- [ ] 3.6.d The choices made for each model and implemented are documented and integrated into the end-to-end genealogy of the models concerned.

<details>
<summary>Expl3.6 :</summary>

The study and selection of relevant decision thresholds for a given data science problem (*threshold selection*) is linked to the metrics selected. As discussed in the resources section of this evaluation issue, in some cases it may be worth considering the possibility of defining ranges of indecision.

</details>

<details>
<Summary>Resources3.6 :</summary>

- (Web article) *[Opening the algorithm's black box and understand its outputs](https://medium.com/@asaboni/opening-the-algorithms-black-box-and-understand-its-outputs-e2363b0a887c)*, A. Saboni (Octo Technologies), April 2020

</details>

---

Q3.7: **Audits by independent third parties and *verifiable claims***
When your organization communicates on the results or performance of an AI system, and relies on such communications for its development and to its stakeholders:

R3.7 :  
_(Type: single answer)_  
_(Select one answer only, which best corresponds to the level of maturity of the organisation on this topic)_

- [ ] 3.7.a We do not communicate or use the results or performance of our AI systems as an argument to our stakeholders, we are not concerned by this assessment element | _(Concerned / Not concerned)_
- [ ] 3.7.b We communicate on our results and rely on them for our development without first having our work audited by an independent third party, without making available any evidence
-[ ]  3.7.c We have our work audited by an independent third party, or we make evidence available, before communicating our results and using them to communicate and rely on with our stakeholders

<details>
<summary>Expl3.7 :</summary>

Developing a predictive model, and determining a meaningful and reliable benchmark performance measure, is a complex challenge. It is therefore often difficult for an organisation to assert that it has achieved excellent results and to claim them with certainty. Where possible, however, it may be even more difficult to make evidence publicly available without revealing valuable information about the organisation's intellectual property and the value of the work carried out. In such cases, it is recommended to have an audit carried out by an independent third party (e.g. security, privacy, fairness, reliability...), in order to secure the results the organisation wishes to claim.

</details>

<details>
<Summary>Resources3.7 :</summary>

- (Academic paper) [Toward Trustworthy AI Development: Mechanisms for Supporting Verifiable Claims](https://arxiv.org/pdf/2004.07213.pdf), §2 p.8-20, April 2020

</details>

---
---

### Section 4 - Ensuring model reproducibility and establishing the chain of accountability

A predictive model is a complex object that can evolve over time. Tracing the stages of its development and evolution allows one to create a form of **genalogy**, which is a prerequisite for **reproducing or auditing** a model. Furthermore, using automatic systems based on models whose rules have been "learned" (and not defined and formalised) questions the way organisations operate. It seems essential to guarantee a clear chain of responsibility, of natural or legal persons, for each model.

[_[⇧ back to the list of sections](#evaluation-framework-to-assess-the-maturity-of-an-organisation)_]  
[_[⇩ next section](#section-5---using-models-responsibly-and-in-confidence)_]

---

