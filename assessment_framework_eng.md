# Responsible and Trustworthy Data Science - Evaluation framework

The [evaluation framework](#evaluation-framework-to-assess-the-maturity-of-an-organisation) below is the result of the participatory work initiated in the spring of 2019 by Labelia Labs (ex- Substra Foundation) and ongoing since then. It is based on the identification of the risks that we are trying to prevent by aiming for a responsible and trustworthy practice of data science, and best practices to mitigate them. It also brings together for each topic technical resources that can be good entry points for interested organisations.

Last update: 2nd semester 2021.

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

**[Data privacy]**

The use of personal or confidential data carries the risk of exposure of such data, which can have very detrimental consequences for the producers, controllers or subjects of such data. Particularly in data science projects, they must therefore be protected and the risks of their leakage or exposure must be minimised.

[_[⇧ back to the list of sections](#evaluation-framework-to-assess-the-maturity-of-an-organisation)_]  
[_[⇩ next section](#section-2---preventing-bias-developing-non-discriminatory-models)

---

Q1.1 : **Applicable legislation and contractual requirements - Identification**  
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

Q1.2 : **Applicable legislation and contractual requirements - Compliance approach**  
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

Q1.3 : **Applicable legislation and contractual requirements - Regulatory surveillance**  
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

Q1.4 : **Applicable legislation and contractual requirements - Auditing and certification**  
Has the organisation's compliance with personal and confidential data requirements been audited and is it recognised by a certification, label or equivalent?

R1.4 :  
_(Type: single answer)_  
_(Select one answer only, which best corresponds to the level of maturity of the organisation on this topic)_

- [ ] 1.4.a Yes
- [ ] 1.4.b No
- [ ] 1.4.c We are currently preparing an upcoming audit or certification of our organisation's compliance with personal and confidential data requirements
- [ ] 1.4.d Not at the organization level, but it is the case for at least one project

<details>
<summary>Expl1.4 :</summary>

In many sectors there are specific compliance requirements. It is generally possible to formalise an organisation's compliance through certification or a specialised audit, or by obtaining a label (e.g. AFAQ "Protection des données personnelles", ISO 27701).

</details>

---

Q1.5 : **Data minimisation principle**  
In data science projects, the data minimisation principle should guide the collection and use of personal or confidential data. How is it implemented in your organisation?

R1.5 :  
_(Type: single answer)_  
_(Select one answer only, which best corresponds to the level of maturity of the organisation on this topic)_  
_(Specific risk domain: use of personal or confidential data)_

- [ ] 1.5.a We take care not to use any personal or confidential data. We are not concerned by this risk area
- [ ] 1.5.b We need to use personal or confidential data in certain projects and the data minimisation principle is then systematically applied
- [ ] 1.5.c Employees are aware of the data minimisation principle and generally apply it
- [ ] 1.5.d The "who can do the most can do the least" reflex with regard to data still exists here and there within our organisation. In some projects, we keep datasets that are much richer in personal and confidential data than what is strictly useful to the project
- [ ] 1.5.e Employees are aware of the data minimisation principle, but it is not applied as a general standard. However, we give a particular attention to implementing personal data-related risk mitigation measures (i.e. pseudonymising some features by identifiers with a separate correspondence table, split datasets in multiple tables kept apart)

<details>
<summary>Expl1.5 :</summary>

The data minimisation principle is sometimes also referred to as "privacy by design". It is one of the pillars of the RGPD in the European Union.

</details>
  
---

_The following elements within this section apply only to organisations that did not select the first response to R1.5. Organisations not concerned are therefore invited to move on to [Section 2](#section-2---preventing-bias-developing-non-discriminatory-models)._

---

Q1.6 : **Project involving new processing of personal or confidential data**  
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

Q1.7 : **Machine Learning security - Knowledge level**  
_(Condition: R1.5 <> 1.5.a)_  
Machine Learning security (_ML security_) is a constantly evolving field. In some cases, AI models learned from confidential data may reveal elements of that confidential data (see articles cited in resources). Within your organisation, the general level of knowledge of collaborators working on data science projects about vulnerabilities related to ML models and the techniques to mitigate them is:

R1.7 :  
_(Type: single answer)_  
_(Select one answer only, which best corresponds to the level of maturity of the organisation on this topic)_

- [ ] 1.7.a Complete beginner
- [ ] 1.7.b Basic
- [ ] 1.7.c Confirmed
- [ ] 1.7.d Expert

<details>
<summary>Expl1.7 :</summary>

The state of the art in ML security is constantly evolving. If data scientists are now familiar in general with the membership inference attack (see proposed resources), new ones are being published regularly. While it is impossible to guard against all vulnerabilities at all times, it is crucial to be aware of them and to keep a watch on them. The article [Demystifying the Membership Inference Attack](https://medium.com/disaitek/demystifying-the-membership-inference-attack-e33e510a0c39) is for example an interesting entry point in the context of sensitive data.

</details>

<details>
<summary>Ressources1.7 :</summary>

- (Software & Tools) *[AI security risk assessment using Counterfit](https://www.microsoft.com/security/blog/2021/05/03/ai-security-risk-assessment-using-counterfit/)*, Microsoft, May 2021 : Counterfit is an open source tool enabling testing different attacks on ML models to identify their vulnerabilities. [Link](https://github.com/Azure/counterfit/) to GitHub repo
- (Technical guide) *[Privacy Enhancing Technologies Decision Tree (v2)](http://www.private-ai.ca/PETs_Decision_Tree.svg)*, Private AI, 2020
- (Web article) *[The secret-sharer: evaluating and testing unintended memorization in neural networks](https://blog.acolyer.org/2019/09/23/the-secret-sharer/)*, A. Colyer, 2019
- (Academic paper) *[Membership Inference Attacks against Machine Learning Models](https://arxiv.org/abs/1610.05820)*, R. Shokri, M. Stronati, C. Song, V. Shmatikov, 2017
- (Software & Tools) *[ML Privacy Meter](https://github.com/privacytrustlab/ml_privacy_meter): a tool to quantify the privacy risks of machine learning models with respect to inference attacks*.
- (Web article) *[Demystifying the membership inference attack](https://medium.com/disaitek/demystifying-the-membership-inference-attack-e33e510a0c39)*, Disaitek, 2019
- (Academic paper) *[Inverting Gradients - How easy is it to break privacy in federated learning](https://arxiv.org/abs/2003.14053)*, J. Geiping, H. Bauermeister, H. Dröge, M. Moeller, 2020
- (Web article) *[Top Five ML risks](https://github.com/OWASP/Top-5-Machine-Learning-Risks/blob/master/Top%205%20Machine%20Learning%20Risks.md)*, OWASP
- (Software & Tools) Tools for *differential privacy*: Google *[differential privacy library](https://github.com/google/differential-privacy)*, and the Python [PyDP](https://github.com/OpenMined/PyDP) wrapper from OpenMined
- (Software & Tools) *[OpenDP](https://opendp.org)*: *a community effort to build trustworthy, open-source software tools for statistical analysis of sensitive private data. Offers the rigorous protections of differential privacy for the individuals who may be represented in confidential data and statistically valid methods of analysis for researchers who study the data*
- (Software & Tools) *[Opacus](https://opacus.ai/)*: *a Facebook Open Source project, to enable training PyTorch models with Differential Privacy*
- (Web article) The *distillation* of a model, in addition to the compression it provides, can be used as a measure to protect the model and the training data used, see for example *[Knowledge Distillation: Simplified](https://towardsdatascience.com/knowledge-distillation-simplified-dd4973dbc764)*, Towards Data Science, 2019.
- (Academic paper) *[Distilling the Knowledge in a Neural Network](https://arxiv.org/abs/1503.02531)*, G. Hinton, O. Vinyals, J. Dean, 2015
- (Web article) *[Model distillation and privacy](https://www.labelia.org/en/blog/model-distillation)*, Labelia Labs (ex- Substra Foundation) blog post to introduce distillation approaches, Gijs Barmentlo, 2020
- (Web article) *[Never a dill moment: Exploiting machine learning pickle files](https://blog.trailofbits.com/2021/03/15/never-a-dill-moment-exploiting-machine-learning-pickle-files/)*, Trail of Bits, March 2021: exposition of a vulnerability of ML models using pickle for objects storage

</details>

---

Q1.8 : **Machine Learning security - Implementation**  
_(Condition: R1.5 <> 1.5.a)_  
Still on the subject of vulnerabilities related to ML models and techniques to mitigate them:

R1.8 :  
_(Type: multiple responses possible)_  
_(Select all the answer items that correspond to practices in your organisation)_

- [ ] 1.8.a We keep a technical watch on the main attacks and measures to mitigate them
- [ ] 1.8.b Employees receive regular information and training to help them develop their skills in this area
- [ ] 1.8.c In some projects, we implement specific techniques to reduce the risks associated with the models we develop (for example: differential privacy, distillation, etc.)
- [ ] 1.8.d On each project, the vulnerabilities that apply to it and the techniques implemented are documented (e.g. in the lifecycle documentation of each model, see Section 4 and Element 4.1 for more information on this concept)
- [ ] 1.8.e We have not yet set up an organised approach to these subjects

<details>
<summary>Expl1.8 :</summary>

The state of the art in ML security is constantly evolving. If data scientists are now familiar in general with the membership inference attack (see proposed resources), new ones are being published regularly. While it is impossible to guard against all vulnerabilities at all times, it is crucial to be aware of them and to keep a watch on them. The article [Demystifying the Membership Inference Attack](https://medium.com/disaitek/demystifying-the-membership-inference-attack-e33e510a0c39) is for example an interesting entry point in the context of sensitive data.

Depending on the level of risk and sensitivity of the projects, certain technical approaches to guard against them will be selected and implemented. It is important to follow the evolution of research and state-of-the-art practices, and to document the choices made. The notion of "Model lifecycle" is introduced here.

</details>

<details>
<summary>Resources1.8 :</summary>

- (Software & Tools) *[AI security risk assessment using Counterfit](https://www.microsoft.com/security/blog/2021/05/03/ai-security-risk-assessment-using-counterfit/)*, Microsoft, May 2021 : Counterfit is an open source tool enabling testing different attacks on ML models to identify their vulnerabilities. [Link](https://github.com/Azure/counterfit/) to GitHub repo
- (Technical guide) *[Privacy Enhancing Technologies Decision Tree (v2)](http://www.private-ai.ca/PETs_Decision_Tree.svg)*, Private AI, 2020
- (Web article) *[The secret-sharer: evaluating and testing unintended memorization in neural networks](https://blog.acolyer.org/2019/09/23/the-secret-sharer/)*, A. Colyer, 2019
- (Academic paper) *[Membership Inference Attacks against Machine Learning Models](https://arxiv.org/abs/1610.05820)*, R. Shokri, M. Stronati, C. Song, V. Shmatikov, 2017
- (Software & Tools) *[ML Privacy Meter](https://github.com/privacytrustlab/ml_privacy_meter): a tool to quantify the privacy risks of machine learning models with respect to inference attacks*.
- (Web article) *[Demystifying the membership inference attack](https://medium.com/disaitek/demystifying-the-membership-inference-attack-e33e510a0c39)*, Disaitek, 2019
- (Academic paper) *[Inverting Gradients - How easy is it to break privacy in federated learning](https://arxiv.org/abs/2003.14053)*, J. Geiping, H. Bauermeister, H. Dröge, M. Moeller, 2020
- (Web article) *[Top Five ML risks](https://github.com/OWASP/Top-5-Machine-Learning-Risks/blob/master/Top%205%20Machine%20Learning%20Risks.md)*, OWASP
- (Software & Tools) Tools for *differential privacy*: Google *[differential privacy library](https://github.com/google/differential-privacy)*, and the Python [PyDP](https://github.com/OpenMined/PyDP) wrapper from OpenMined
- (Software & Tools) *[OpenDP](https://opendp.org)*: *a community effort to build trustworthy, open-source software tools for statistical analysis of sensitive private data. Offers the rigorous protections of differential privacy for the individuals who may be represented in confidential data and statistically valid methods of analysis for researchers who study the data*
- (Software & Tools) *[Opacus](https://opacus.ai/)*: *a Facebook Open Source project, to enable training PyTorch models with Differential Privacy*
- (Web article) The *distillation* of a model, in addition to the compression it provides, can be used as a measure to protect the model and the training data used, see for example *[Knowledge Distillation: Simplified](https://towardsdatascience.com/knowledge-distillation-simplified-dd4973dbc764)*, Towards Data Science, 2019.
- (Academic paper) *[Distilling the Knowledge in a Neural Network](https://arxiv.org/abs/1503.02531)*, G. Hinton, O. Vinyals, J. Dean, 2015

</details>

---

Q1.9 : **Notification of safety incidents to the regulatory authorities**  
_(Condition: R1.5 <> 1.5.a)_  
In the event that a model that the organisation has developed is used or accessible by one or more external stakeholders, and a new vulnerability is published, there is a risk that it may apply to them and thus create a risk of exposure of personal or confidential data:

R1.9 :  
_(Type: single answer)_  
_(Select one answer only, which best corresponds to the level of maturity of the organisation on this topic)_

- [ ] 1.9.a We have not yet put in place a procedure for such cases
- [ ] 1.9.b We have a process describing the course of action in such cases
- [ ] 1.9.c We have a process describing the course of action in such cases, which references the authorities to whom we must report
- [ ] 1.9.d We have a process describing the course of action in such cases, which references the authorities to whom we must report, and which includes communication to the stakeholders of whom we have contact details

<details>
<summary>Expl1.9 :</summary>

In some sectors there are obligations to report safety incidents to the regulatory authorities (e.g. in France: CNIL, ANSSI, ARS, etc.). An interesting entry point: [Notifications of safety incidents to regulatory authorities: how to organise and who to contact](https://www.cnil.fr/fr/notifications-dincidents-de-securite-aux-autorites-de-regulation-comment-sorganiser-et-qui-sadresser) on the CNIL website.

</details>

---
---

### Section 2 - Preventing bias, developing non-discriminatory models

**[Biases and discrimination]**

The use of AI models learned from historical data can be counterproductive when historical data are contaminated by problematic phenomena (e.g. quality of certain data points, non-comparable data, social phenomena undesirable due to the time period, etc.). A key challenge for responsible and trustworthy data science is to respect the principle of diversity, non-discrimination and equity (described for example in section 1.5 of the EU [Ethics Guidelines for Trustworthy AI](https://ec.europa.eu/newsroom/dae/document.cfm?doc_id=60419)). It is therefore essential to question this risk and to study the nature of the data used, the conditions under which they were produced and collected, and what they represent.
Among other things, in some cases a specification of the equity sought between populations must also be defined. The equity of a model can [be defined in several ways that may be inconsistent with each other](https://papers.nips.cc/paper/6995-counterfactual-fairness), and the interpretation of performance scores must therefore be made within the framework of one of these definitions.

[_[⇧ back to the list of sections](#evaluation-framework-to-assess-the-maturity-of-an-organisation)_]  
[_[⇩ next section](#section-3---assessing-model-performance-rigorously)_]

---

Q2.1 : **Analysis of the training data**  
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
- (Software & Tools) *[Pandas Profiling](https://github.com/pandas-profiling/pandas-profiling)*: Create HTML profiling reports from pandas `DataFrame` objects. The pandas `df.describe()` function is great but a little basic for serious exploratory data analysis. `pandas_profiling` extends the pandas `DataFrame` with `df.profile_report()` for quick data analysis

</details>

---

Q2.2 : **Evaluation of the risk of discrimination against certain social groups**  
In the context of data science projects, the nature of the project, the data used for the project and/or the thematic environment of the project can foster a risk of discrimination against certain social groups (gender, origin, age, etc.). Evaluating first for each project if it is subject or not to such a risk seems key (in which case mitigation measures can be then contemplated). On that topic, your organisation:

R2.2 :  
_(Type: single answer)_  
_(Select one answer only, which best corresponds to the level of maturity of the organisation on this topic)_  
_(Specific risk domain: discrimination against certain social groups)_

- [ ] 2.2.a Operates informally and relies on the practices of each collaborator involved to evaluate if there is a risk
- [ ] 2.2.b Does not have a documented approach to the subject, but the collaborators involved are trained on the risks and best practices on the subject
- [ ] 2.2.c Has a documented approach that is systematically implemented to evaluate this type of risk


<details>
<summary>Expl2.2 :</summary>

Configurations with risks of potential discriminations against social groups are particularly sensitive for the organisation and its counterparts. It requires special attention and the use of specific methodologies.
In certain cases it is obvious if this risk has to be considered or not (e.g. projects on behavioral data on a population of users or customers, vs. projects on oceanographic or astronomical data), whereas in some cases it might be less obvious. It is therefore important to consider the question for each project.

</details>

---

Q2.3 : **Preventing discriminatory bias**  
_(Condition: R2.2 <> 2.2.b)_  
In cases where the AI models your organisation develops are used in thematic environments where there is a risk of discrimination against certain social groups (gender, origin, age, etc.):

R2.3 :  
_(Type: multiple responses possible)_  
_(Select all the answer items that correspond to practices in your organisation)_  
_(Specific risk domain: discrimination against certain social groups)_

- [ ] 2.3.a We are not involved in cases where AI models are used in thematic environments with risks of discrimination against certain social groups (gender, origin, age, etc.) | _(Concerned / Not concerned)_
- [ ] 2.3.b We pay particular attention to the identification of protected attributes and their possible proxies (e.g. studying one by one the variables used as model inputs to identify the correlations they might have with sensitive data)
- [ ] 2.3.c We carry out evaluations on test data from different sub-populations in order to identify possible problematic biases
- [ ] 2.3.d We select and implement one or more justice and equity measure(s) (_fairness metrics_)
- [ ] 2.3.e We use _data augmentation_ or _re-weighting_ approaches to reduce possible biases in the data sets
- [ ] 2.3.f The above practices that we implement are duly documented and integrated into the model lifecycle documentation of the models concerned
- [ ] 2.3.g We have not yet put in place any such measures

<details>
<summary>Expl2.3 :</summary>

It is a question of systematically questioning, for each data science project and according to the objective and target use of the model that one wants to develop, the features that may directly or indirectly be the source of a risk of discriminatory bias. The term "protected attribute" or "protected variable" is used to refer to attributes whose values define sub-populations at risk of discrimination.
Complement on the use of synthetic data and _data augmentation_, _re-weighting_ approaches in order to reduce possible biases in the data sets: when such techniques are used it is important to make them explicit, otherwise there is a risk of losing information on how a model was developed.

</details>

<details>
<summary>Resources2.3 :</summary>

- (Web article) *[Unfair biases in Machine Learning: what, why, where and how to obliterate them](https://www.mlsecurity.ai/post/unfair-biases-in-machine-learning-what-why-where-and-how-to-obliterate-them)*, blog ML Security, P. Irolla, April 2020
- (Web article) [Awful AI](https://github.com/daviddao/awful-ai), a registry of worrying AI services or projects, David Dao
- (Technical guide) *[A Tutorial on Fairness in Machine Learning](https://towardsdatascience.com/a-tutorial-on-fairness-in-machine-learning-3ff8ba1040cb)*, Towards Data Science blog, Z. Zhong, October 2018
- (Web article) *[Measuring fairness](https://pair.withgoogle.com/explorables/measuring-fairness)* explorable, [PAIR](https://pair.withgoogle.com/)
- (Software & Tools) *[AI Fairness 360](https://developer.ibm.com/technologies/artificial-intelligence/projects/ai-fairness-360/): an open source software toolkit that can help detect and remove bias in machine learning models*, IBM
- (Academic paper) *Fairness metrics* : *[counterfactual fairness](https://papers.nips.cc/paper/6995-counterfactual-fairness)*
- (Academic paper) *Fairness metrics* : *[adversarial debiaising](https://arxiv.org/pdf/1801.07593.pdf)*
- (Technical guide) Book *Fair ML* : *[Fairness and machine learning - Limitations and opportunities](https://fairmlbook.org/)*, Solon Barocas, Moritz Hardt, Arvind Narayanan, December 2019
- (Web article) *[Fairness in Machine Learning](https://www.labelia.org/en/blog/fairness-in-machine-learning)*, introduction to Fairness metrics on Labelia Labs (ex- Substra Foundation)'s blog, Mickael Fine, 2020

</details>

---

Q2.4 : **Links between modelisation choices and bias**  
_(Condition : R2.2 <> 2.2.b)_  
Recent work has shown the role that modeling and learning choices can play in the formation of discriminatory bias. Differential privacy, compression, the choice of the learning rate, early stopping mechanisms for example can have disproportionate impacts on certain subgroups. Within your organisation, the general level of knowledge of collaborators working on data science projects on this topic is:

R2.4 :  
_(Type: single answer)_  
_(Select one answer only, which best corresponds to the level of maturity of the organisation on this topic)_  
_(Specific risk domain: discrimination against certain social groups)_

- [ ] 2.4.a We are not involved in cases where AI models are used in thematic environments with risks of discrimination against certain social groups (gender, origin, age, etc.) | _(Concerned / Not concerned)_
- [ ] 2.4.b Complete beginner
- [ ] 2.4.c Basic
- [ ] 2.4.d Confirmed
- [ ] 2.4.e Expert

<details>
<summary>Expl2.4 :</summary>

If datasets used to train and evaluate a model require a particular attention to prevent discriminatory biases, recent work shows that modeling choices have to be taken into account too. The article *"Moving beyond “algorithmic bias is a data problem”"* suggested in resources synthesizes very well how the learning algorithm, the model structure, adding or not differential privacy, compression, etc. can have consequences on the fairness of a model. Extracts:

> - *A key reason why model design choices amplify algorithmic bias is because notions of fairness often coincide with how underrepresented protected features are treated by the model*
> - [...] *design choices to optimize for either privacy guarantees or compression amplify the disparate impact between minority and majority data subgroups*
> - [...] *the impact of popular compression techniques like quantization and pruning on low-frequency protected attributes such as gender and age and finds that these subgroups are systematically and disproportionately impacted in order to preserve performance on the most frequent features*
> - [...] *learning rate and length of training can also disproportionately impact error rates on the long-tail of the dataset. Work on memorization properties of deep neural networks shows that challenging and underrepresented features are learnt later in the training process and that the learning rate impacts what is learnt. Thus, early stopping and similar hyper-parameter choices disproportionately and systematically impact a subset of the data distribution.*

These topics require a strong expertise and few practitioners are familiar with them yet. In the context of this evaluation element, the recommendation is to learn about them and become aware of the complex trade-offs it implies, consider them during concrete projects rather than hiding them away, and follow how the state-of-the-art evolves and what best practices emerge.

</details>

<details>
<summary>Resources2.4 :</summary>

- (Academic paper) *[Moving beyond “algorithmic bias is a data problem”](https://www.cell.com/patterns/fulltext/S2666-3899(21)00061-1)*, Sara Hooker, Opinion, April 2021
- (Academic paper) *[Algorithmic Factors Influencing Bias in Machine Learning](https://arxiv.org/abs/2104.14014)*, W. Blanzeisky, P. Cunningham, April 2021: The authors defines 4 types of algorithmic choices : Data description (for the first version on the model, and feature engineering), Irreductible Errors, Impact of regularization (present in DL or more classical ML), Impact of class & feature imbalance. Those 4 types of choices will generate what they call underestimation bias, opposed to negative latency, bias due to data (that can be due to an under-representative dataset, or other reasons). They also propose some mitigation process.
- (Academic paper) *[Man is to Computer Programmer as Woman is to Homemaker? Debiasing Word Embeddings](https://arxiv.org/abs/1607.06520)*, T. Bolukbasi, K.-W. Chang, J. Zou, V. Saligrama, A. Kalai, 2016

</details>

---
---

### Section 3 - Assessing model performance rigorously

**[Performance evaluation]**

The performance of the models is crucial for their adoption in products, systems or processes. Performance evaluation must therefore be rigorous.

[_[⇧ back to the list of sections](#evaluation-framework-to-assess-the-maturity-of-an-organisation)_]  
[_[⇩ next section](#section-4---ensuring-model-reproducibility-and-establishing-the-chain-of-accountability)_]

---

Q3.1 : **Separation of test datasets**  
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

Q3.2 : **Privacy-preserving distributed learning projects**  
In the case of data science projects based on distributed or federated learning on multiple datasets and whose confidentiality must be preserved:

R3.2 :  
_(Type: single answer)_  
_(Select one answer only, which best corresponds to the level of maturity of the organisation on this topic)_  
_(Specific risk domain: federated leraning on sensitive data)_

- [ ] 3.2.a We do not participate in *privacy-preserving* distributed learning projects | _(Concerned / Not concerned)_
- [ ] 3.2.b We master and implement approaches to develop test datasets in such a way that there is no cross-contamination between training and test data from different partners
- [ ] 3.2.c At this stage we do not master the methods for developing test datasets in such a way that there is no cross-contamination between training and test data from the different partners

<details>
<summary>Expl3.2 :</summary>

In this type of distributed learning project under conditions where the data is kept confidential, the question arises of how to compose a test dataset, making sure that it does not also appear in the training dataset (e.g. at another partner's premises).

</details>

<details>
<summary>Resources3.2 :</summary>

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

The use of AI models that have been validated and tested on historical data can be counterproductive when the historical data in question is contaminated by problematic phenomena. It seems essential to question this risk and to study the nature of the data used, the conditions under which they were produced and assembled, and what they represent.

</details>

---

Q3.4 : **Performance validation**  
Does your organisation implement the following approaches:

R3.4 :  
_(Type: multiple responses possible)_  
_(Select all the answer items that correspond to practices in your organisation)_

- [ ] 3.4.a When developing a model, we choose the performance metric(s) prior to actually training the model, from among the most standard metrics possible
- [ ] 3.4.b The implementation of robustness metrics is considered and evaluated for each modelling project, and applied by default in cases where the input data may be subject to fine-grain alterations (e.g. images, sounds)
- [ ] 3.4.c The above practices that we implement are documented and integrated into the model lifecycle documentation of the models concerned, including the performance metrics chosen
- [ ] 3.4.d We have not yet introduced any such measures

<details>
<summary>Expl3.4 :</summary>

On choosing metrics upstream, see for example the risk of *[p-hacking / data dredging](https://en.wikipedia.org/wiki/Data_dredging)*.
On robustness, an intuitive definition is that a model is robust when its performance is stable when the input data is disturbed. For more information see the technical resources indicated.

</details>

<details>
<summary>Resources3.4 :</summary>

- (Web article) *[The Comprehensive Guide to Model Validation Framework: What is a Robust Machine Learning Model?](https://medium.com/@ODSC/the-comprehensive-guide-to-model-validation-framework-what-is-a-robust-machine-learning-model-7bdbc41c1702)*, Open Data Science, March 2020
- (Web article) *[Testing Robustness Against Unforeseen Adversaries](https://openai.com/blog/testing-robustness/)*, Open AI, August 2019
- (Academic paper) *Robustness metrics* : *[noise sensitivity score](https://arxiv.org/abs/1806.01477)*.
- (Technical guide) *[Adversarial Robustness - Theory and Practice](https://adversarial-ml-tutorial.org/)*, Z. Kolter and A. Madry
- (Technical guide) *[Understand Robustness](https://github.com/Nathanlauga/understand-robustness/blob/main/notebooks/understand_robustness.ipynb)*, Nathan Lauga, 2020

</details>

---

Q3.5 : **Monitoring model performance over time**  
In cases where AI models developed by your organisation are used in production systems:

R3.5 :  
_(Type: multiple responses possible)_  
_(Select all response items that correspond to practices in your organisation. Please note that some combinations would not be coherent)_  
_(Specific risk domain: use of AI models in production systems)_

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
<summary>Resources3.5 :</summary>

- (Technical guide) *[Continuous delivery for machine learning](https://martinfowler.com/articles/cd4ml.html)*, D. Sato, A. Wider, C. Windheuser, September 2019
- (Technical guide) *[Monitoring Machine Learning Models in Production - A comprehensive guide](https://christophergs.com/machine%20learning/2020/03/14/how-to-monitor-machine-learning-models/)*, Christopher Samiullah, March 2020
- (Web article) *[Google's medical AI was super accurate in a lab. Real life was a different story](https://www.technologyreview.com/2020/04/27/1000658/google-medical-ai-accurate-lab-real-life-clinic-covid-diabetes-retina-disease/)*, MIT Technology Review
- (Web article) (In French) *[En route vers le cycle de vie des modèles !](https://www.quantmetry.com/blog/premier-etape-cycle-vie-modeles/)*, G. Martinon, Janvier 2020

</details>

---

Q3.6 : **Decision making and ranges of indecision**  
For the definition of decision thresholds for models or automatic systems based on them, your organisation:

R3.6 :  
_(Type: multiple responses possible)_  
_(Select all response items that correspond to practices in your organisation. Please note that some combinations would not be coherent)_

- [ ] 3.6.a Operates informally on this subject, depending upon the collaborators involved
- [ ] 3.6.b Has a documented approach that is systematically implemented
- [ ] 3.6.c Takes into account the possibility of maintaining ranges of indecision in certain cases
- [ ] 3.6.d The choices made for each model and implemented are documented and integrated into the lifecycle documentation of the models concerned.

<details>
<summary>Expl3.6 :</summary>

The study and selection of relevant decision thresholds for a given data science problem (*threshold selection*) is linked to the metrics selected. As discussed in the resources section of this evaluation issue, in some cases it may be worth considering the possibility of defining ranges of indecision.

</details>

<details>
<summary>Resources3.6 :</summary>

- (Web article) *[Opening the algorithm's black box and understand its outputs](https://medium.com/@asaboni/opening-the-algorithms-black-box-and-understand-its-outputs-e2363b0a887c)*, A. Saboni (Octo Technologies), April 2020

</details>

---

Q3.7 : **Audits by independent third parties and *verifiable claims***
When your organization communicates on the results or performance of an AI system, and makes it a marketing and communication argument to its stakeholders:

R3.7 :  
_(Type: single answer)_  
_(Select one answer only, which best corresponds to the level of maturity of the organisation on this topic)_  
_(Specific risk domain: external communication on the performance of AI systems)_

- [ ] 3.7.a We do not communicate or do not need to communicate on the results or the performance of our AI systems, or do not use the results or performance of our AI systems as an argument to our stakeholders, we are not concerned by this assessment element | _(Concerned / Not concerned)_
- [ ] 3.7.b We communicate on the results or the performance of our AI systems and rely on them for our development without first having our work audited by an independent third party, without making evidence available
- [ ] 3.7.c We have our work audited by an independent third party, or we make evidence available, before communicating our results and using them to communicate and rely on with our stakeholders

<details>
<summary>Expl3.7 :</summary>

Developing an AI model, and determining a meaningful and reliable benchmark performance measure, is a complex challenge. It is therefore often difficult for an organisation to assert that it has achieved excellent results and to claim them with certainty. Where possible, however, it may be even more difficult to make evidence publicly available without revealing valuable information about the organisation's intellectual property and the value of the work carried out. In such cases, it is recommended to have an audit carried out by an independent third party (e.g. security, privacy, fairness, reliability...), in order to secure the results the organisation wishes to claim.

</details>

<details>
<summary>Resources3.7 :</summary>

- (Academic paper) [Toward Trustworthy AI Development: Mechanisms for Supporting Verifiable Claims](https://arxiv.org/pdf/2004.07213.pdf), §2 p.8-20, April 2020

</details>

---
---

### Section 4 - Ensuring model reproducibility and establishing the chain of accountability

**[Model documentation]**

An AI model is a complex object that can evolve over time. Tracing the stages of its development and evolution allows one to create a form of **model lifecycle**, which is a prerequisite for **reproducing or auditing** a model. Furthermore, using automatic systems based on models whose rules have been "learned" (and not defined and formalised) questions the way organisations operate. It seems essential to guarantee a clear chain of responsibility, of natural or legal persons, for each model.

[_[⇧ back to the list of sections](#evaluation-framework-to-assess-the-maturity-of-an-organisation)_]  
[_[⇩ next section](#section-5---using-models-responsibly-and-in-confidence)_]

---

Q4.1 : **"Lifecycle" of ML models**  
Ensuring the traceability of all steps of the development of an AI model enables building up a form of **model lifecycle**. Within your organisation, a lifecycle documentation of models is fed and maintained within the framework of data science projects, throughout the phases of data collection, design, training, validation and exploitation of the predictive models:

R4.1 :  
_(Type: single answer)_  
_(Select one answer only, which best corresponds to the level of maturity of the organisation on this topic)_

- [ ] 4.1.a At this stage we have not implemented any such approach
- [ ] 4.1.b This information exists and is recorded so as not to be lost, but it may be scattered and it is not versioned
- [ ] 4.1.c They are compiled in a single document which systematically accompanies the model
- [ ] 4.1.d They are gathered in a single document that systematically accompanies the model and is versioned

<details>
<summary>Expl4.1 :</summary>

This concept of "model lifecycle" of a learned AI model can take the form, for example, of a reference document containing all the important choices and the entire history of model development (data used, pre-processing carried out, type of learning and model architecture, hyperparameters selected, decision thresholds, test metrics, etc.), and the internal processes organising this activity. In particular, it is interesting to include the trade-offs that have been made and why (e.g. trade-offs precision-specification, performance-privacy, performance-computing cost, etc.).

</details>

<details>
<summary>Ressources4.1 :</summary>

- (Software & Tools) [Substra Framework](http://doc.substra.ai/): *an open source framework offering distributed orchestration of machine learning tasks among partners while guaranteeing secure and trustless traceability of all operations*
- (Software & Tools) [MLflow](https://mlflow.org/): *an open source platform to manage the ML lifecycle, including experimentation, reproducibility, deployment, and a central model registry*
- (Software & Tools) [DVC](https://dvc.org/): *an Open-source Version Control System for Machine Learning Projects*
- (Software & Tools) [DAGsHub](https://dagshub.com/docs/): *a platform for data version control and collaboration, based on DVC* *a platform for data version control and collaboration, based on DVC*
- (Software & Tools) [Model lifecycle template](https://github.com/dataforgoodfr/batch8_substra/blob/master/G%C3%A9n%C3%A9alogie%20de%20bout-en-bout/Genealogie-de-bout-en-bout_template.md): *template for Data Scientists to help collect all the information in order to trace the lifecycle from end to end of a model*, 2020, Joséphine Lecoq-Vallon

</details>

---

Q4.2 : **Conditions and limitations for using a model**  
In the context of data science projects, the "conditions and limits of validity" of a model designed, trained and validated by the organisation:

R4.2 :  
_(Type: multiple responses possible)_  
_(Select all response items that correspond to practices in your organisation. Please note that some combinations would not be coherent)_

- [ ] 4.2.a Are not documented systematically, it relies on the practices of each collaborator involved
- [ ] 4.2.b Are systematically explicited and documented
- [ ] 4.2.c Are versioned
- [ ] 4.2.d Contain a description of the risks involved in using the model outside its "conditions and limits of validity"
- [ ] 4.2.e The documents presenting these "conditions and limits of validity" systematically accompany the models throughout their life cycle

<details>
<summary>Expl4.2 :</summary>

The aim is to make explicit and add to the model the description of the context of use for which it was designed and in which its announced performance is significant. This concept of "conditions and limits of validity" can take the form of a synthetic document or a specific section in the "model lifecycle" documentation.

</details>

<details>
<summary>Ressources4.2 :</summary>

- (Academic paper) [Model Cards for Model Reporting](https://arxiv.org/abs/1810.03993), M. Mitchell, S. Wu, A. Zaldivar, P. Barnes, L. Vasserman, B. Hutchinson, E. Spitzer, I. D. Raji, T. Gebru, January 2019
- (Web article) [Model Cards](https://modelcards.withgoogle.com/about) from Google is an open and scalable framework, and offers 2 examples: *To explore the possibilities of model cards in the real world, we've designed examples for two features of our Cloud Vision API, Face Detection and Object Detection. They provide simple overviews of both models' ideal forms of input, visualize some of their key limitations, and present basic performance metrics.*
- (Web article) *[Model Cards for AI Model Transparency](https://blog.einstein.ai/model-cards-for-ai-model-transparency/)*, Salesforce: examples of *Model Cards* used and published by Salesforce
- (Software & Tools) *[AI FactSheets 360](https://aifs360.mybluemix.net/)*, an IBM Research project to foster trust in AI by increasing transparency and enabling governance: *Increased transparency provides information for AI consumers to better understand how an AI model or service was created. This allows a consumer of the model to determine if it is appropriate for their situation. AI Governance enables an enterprise to specify and enforce policies describing how an AI model or service should be constructed and deployed.*

</details>

---

Q4.3 : **Analysis and publications of incidents reports**  
In data science projects, when unexpected behaviour of a model is observed:

R4.3 :  
_(Type: multiple responses possible)_  
_(Select all response items that correspond to practices in your organisation. Please note that some combinations would not be coherent)_

- [ ] 4.3.a At this stage we do not analyse the incidents or unexpected behaviour observed
- [ ] 4.3.b We analyse incidents or unexpected behaviour encountered, but don't publish or share it
- [ ] 4.3.c We analyse incidents or unexpected behaviour encountered and publish them when relevant (e.g. article, blog)
- [ ] 4.3.d We get involved in clubs, networks or professional associations in the field of data science, and give feedback on incidents of unexpected behaviour that we observe

<details>
<summary>Expl4.3 :</summary>

Understanding or even mastering the behaviour of a learned AI model is a complex challenge. Lots of research is being done to develop methods and tools in this area, but much remains to be done. The sharing by practitioners of the unexpected incidents and behaviours they encounter contributes to the progress of the community.

</details>

<details>
<summary>Ressources4.3 :</summary>

- (Software & Tools) [AI Incident Registry](http://aiid.partnershiponai.org/), Partnership on AI
- (Web article) [Specification gaming examples in AI](https://docs.google.com/spreadsheets/d/e/2PACX-1vRPiprOaC3HsCf5Tuum8bRfzYUiKLRqJmbOoC-32JorNdfyTiRRsR6Ea5eWtvsWzuxo8bjOxCG84dAg/pubhtml), Victoria Krakovna
- (Web article) [Learning from Tay's introduction](https://blogs.microsoft.com/blog/2016/03/25/learning-tays-introduction/): Incident analysis of the Tay chatbot, Microsoft, 2016
- (Academic paper) [Toward Trustworthy AI Development: Mechanisms for Supporting Verifiable Claims](https://arxiv.org/pdf/2004.07213.pdf), §2.4 p.19, April 2020

</details>

---

Q4.4 : **Value chain and chain of accountability**  
In the case of data science projects where several players, including internal to the organisation (teams, departments, subsidiaries), are involved throughout the value and accountability chains:

R4.4 :  
_(Type: multiple responses possible)_  
_(Select all response items that correspond to practices in your organisation. Please note that some combinations would not be coherent)_  
_(Specific risk domain: roles and responsibilities in data science projects are divided up multiple actors)_

- [ ] 4.4.a Within our organisation, data science projects are carried out end-to-end by autonomous teams, including the elaboration of datasets and the exploitation of models for its own account. Consequently, for each project, an autonomous team is solely responsible | _(Concerned / Not concerned)_
- [ ] 4.4.b We systematically identify the risks and responsibilities of each of the internal and external stakeholders with whom we work
- [ ] 4.4.c We systematically enter into contracts with upstream (e.g. data suppliers) and downstream (e.g. customers, model-using partners) players
- [ ] 4.4.d We do not systematically implement this type of measure

<details>
<summary>Expl4.4 :</summary>

It is important to ensure that organisations upstream and downstream the chain identify and take responsibility for their segments of the value chain.

</details>

---

Q4.5 : **Subcontracting of all or part of the data science activities**  
Data science activities subcontracted to a third party organisation(s) are subject to the same requirements your organisation applies to itself:

R4.5 :  
_(Type: single answer)_  
_(Select one answer only, which best corresponds to the level of maturity of the organisation on this topic)_  
_(Specific risk domain: subcontracting of data science activities)_

- [ ] 4.5.a Not concerned, we do not subcontract these activities | _(Concerned / Not concerned)_
- [ ] 4.5.b Yes, our responses to this evaluation take into account the practices of our subcontractors
- [ ] 4.5.c No, our answers to this evaluation do not apply to our subcontractors and on certain points they may be less advanced than us

<details>
<summary>Expl4.5 :</summary>

As in the reference frameworks of IS management (ISO 27001) or GDPR in the European Union, it is important not to dilute responsibilities in uncontrolled subcontracting chains. This should apply, for example, to consultants, freelancers who come to reinforce an internal team on a data science project. For example, it is possible to ask sub-contractors to carry out the same evaluation on their own account and share their results with you.

</details>

---

Q4.6 : **Distribution of the value creation**  
In the case of data science projects where several partners work alongside your organisation to develop a model, and that model is or will be the subject of an economic activity:

R4.6 :  
_(Type: multiple responses possible)_  
_(Select all response items that correspond to practices in your organisation. Please note that some combinations would not be coherent)_  
_(Specific risk domain: roles and responsibilities in data science projects are divided up multiple actors)_

- [ ] 4.6.a Our organisation carries out its data science activities autonomously, including the development of datasets and the exploitation of models for its own account. It is therefore not concerned | _(Concerned / Not concerned)_
- [ ] 4.6.b At this stage we have not structured this aspect of multi-partner data science projects
- [ ] 4.6.c In these cases, we contract the economic aspect of the relationship with the stakeholders involved upstream of the project
- [ ] 4.6.d Our organisation has a policy that responsibly frames the sharing of value with the stakeholders involved

<details>
<summary>Expl4.6 :</summary>

When several partners work together to develop a model, it is important that the distribution of value resulting from an economic activity in which the model plays a role is made explicit and contractualized. In some cases this can be a complex issue, for example when a model is trained in a distributed manner over several datasets.

</details>

<details>
<summary>Ressources4.6 :</summary>

- (Code repository) [Exploration of dataset contributivity to a model in collaborative ML projects](https://github.com/SubstraFoundation/distributed-learning-contributivity), an open source project led by [ Labelia Labs (ex- Substra Foundation)](https://www.labelia.org/)

</details>

---
---

### Section 5 - Using models responsibly and in confidence

**[Using the models]**

An AI model can be used as an automatic system, whose rules or criteria are not written _in extenso_ and are difficult to explain, discuss or adjust. Using automatic systems based on AI models whose rules have been "learned" (and not defined and formalised) therefore questions the way organisations design and operate their products and services. It is important to preserve the responsiveness and resilience of organisations using those AI models, particularly in dealing with situations where AI models have led to an undesirable outcome for the organisation or its stakeholders. In addition, efforts are therefore needed on the interpretation and explanation of the choices made using these systems.

[_[⇧ back to the list of sections](#evaluation-framework-to-assess-the-maturity-of-an-organisation)_]  
[_[⇩ next section](#section-6---anticipating-monitoring-and-minimising-the-negative-externalities-of-data-science-activities)_]

---

Q5.1 : **Exploitation of AI models for one's own account**  
If your organisation uses AI models on its own behalf:

R5.1 :  
_(Type: multiple responses possible)_  
_(Select all response items that correspond to practices in your organisation. Please note that some combinations would not be coherent)_  
_(Specific risk domain: use of AI models, provision or operation of AI model-based applications for customers or third parties)_

- [ ] 5.1.a Our organisation does not use ML models on its own behalf | _(Concerned / Not concerned)_
- [ ] 5.1.b **An AI models register** identifies all the models used by the organisation and is kept up-to-date
- [ ] 5.1.c For each model there is an **owner** defined, identifiable and easily contactable
- [ ] 5.1.d For each model, we systematically carry out a **risk assessment** following any incidents, failures or biases
- [ ] 5.1.e Monitoring tools are put in place to ensure continuous monitoring of systems based on AI models and can trigger alerts directly to the team in charge
- [ ] 5.1.f For each model, we define and test a procedure for suspending the model and a degraded operating mode without the model, in order to prepare for the case where the model is subject to failure or unexpected behaviour
- [ ] 5.1.g For each model, we study its entire lifecycle (all the steps and choices that led to its development and evaluation), as well as its conditions and limits of validity, in order to understand the model before using it
- [ ] 5.1.h We always use the models for **uses in accordance with their conditions and limits of validity**
- [ ] 5.1.i We have not yet put in place such measures

<details>
<summary>Expl5.1 :</summary>

Using automatic systems based on models whose rules have been "learned" (and not defined and formalised) questions the way organisations design and operate their products and services. It is important to assess the consequences and reactions in the event of an incident. Furthermore, it is important that persons in charge is clearly identified so that no stakeholder is left helpless in the face of an unexpected or inappropriate consequence. Finally, it is important to consider the "conditions and limits of validity" of the models used to ensure that the intended use is appropriate.

</details>

---

Q5.2 : **Development of AI models on behalf of third parties**  
If your organisation provides or operates AI model-based applications to customers or third parties:

R5.2 :  
_(Type: multiple responses possible)_  
_(Select all response items that correspond to practices in your organisation. Please note that some combinations would not be coherent)_  
_(Specific risk domain: use of AI models, provision or operation of AI model-based applications for customers or third parties)_

- [ ] 5.2.a Our organisation does not provide its customers or third parties, nor does it operates on behalf of third parties, with applications based on ML models | _(Concerned / Not concerned)_
- [ ] 5.2.b **An AI models register** identifies all models or applications used by its customers and/or by the organisation on behalf of third parties, and is kept up-to-date
- [ ] 5.2.c For each model or application for a customer or a third party we have a defined, identifiable and easily reachable **owner**
- [ ] 5.2.d For each model or application for a customer or a third party, we systematically carry out a **risk assessment** resulting from possible incidents, failures, biases, etc., in order to identify the risks involved
- [ ] 5.2.e Monitoring tools are in place to ensure continuous monitoring of ML systems and can trigger alerts directly to the responsible team
- [ ] 5.2.f For each model or application for a customer or a third party, we define and test a procedure for suspending the model and a degraded operating mode without the model, in order to prepare for the case where the model is subject to failure or unexpected behaviour
- [ ] 5.2.g For each model or application for a client or third party, we study its entire lifecycle and its conditions and limits of validity to understand the model before using it
- [ ] 5.2.h We supply our customers or operate on their behalf with models or applications for **uses in accordance with their conditions and limits of validity**
- [ ] 5.2.i We have not yet put in place such measures

<details>
<summary>Expl5.2 :</summary>

Using automatic systems based on models whose rules have been "learned" (and not defined and formalised) questions the way organisations design and operate their products and services. It is important to assess the consequences and reactions in the event of an incident. Furthermore, it is important that persons in charge is clearly identified so that no stakeholder is left helpless in the face of an unexpected or inappropriate consequence. Finally, it is important to consider the "conditions and limits of validity" of the models used to ensure that the intended use is appropriate.

</details>

---

Q5.3 : **Management of problematic predictions, bypass process, _human agency_**  
Automatic systems, especially when based on AI models, are used in production generally to gain efficiency. By nature, they occasionally generate undesirable results for the organisation and its stakeholders (e.g. wrong prediction), as they will never achieve 100% performance.

R5.3 :  
_(Type: single answer)_  
_(Select one answer only, which best corresponds to the level of maturity of the organisation on this topic)_  
_(Specific risk domain: use of AI models, provision or operation of AI model-based applications for customers or third parties)_

- [ ] 5.3.a Our organisation does not use AI models on its own behalf or on behalf of its clients, and does not provide its clients with applications based on AI models | _(Concerned / Not concerned)_
- [ ] 5.3.b We implement AI models in integrated automatic systems, without mechanisms to overcome or avoid undesirable results due to model predictions
- [ ] 5.3.c We integrate, in automatic systems based on AI models, the functionalities to manage these cases of undesirable results. For such cases, we set up mechanisms allowing a human operator to go against an automatic decision to manage such undesirable results or incidents
- [ ] 5.3.d In addition to incident management mechanisms, in automatic systems based on AI models, when the confidence interval for the automatic decision is not satisfactory a human operator is called upon
- [ ] 5.3.e We systematically apply the principle of "human agency", the outputs of the AI models that we implement are used by human operators, and do not serve as determinants for automatic decisions

<details>
<summary>Expl5.3 :</summary>

Using automatic systems based on models whose rules have been "learned" (and not defined and formalised) questions the way organisations design and operate their products and services. It is important to preserve the responsiveness and resilience of the organisation.

</details>

<details>
<summary>Ressources5.3 :</summary>

- (Technical guide) *[Monitoring Machine Learning Models in Production - A comprehensive guide](https://christophergs.com/machine%20learning/2020/03/14/how-to-monitor-machine-learning-models/)*, Christopher Samiullah, March 2020

</details>

---

Q5.4 : **Explicability and interpretability**  
Within data science projects aiming at developing AI models:

R5.4 :  
_(Type: multiple responses possible)_  
_(Select all response items that correspond to practices in your organisation. Please note that some combinations would not be coherent)_

- [ ] 5.4.a Our organisation is not yet familiar with the methods and tools for explaining and interpreting AI models
- [ ] 5.4.b We are interested in the explicability and interpretability of AI models and are in dialogue with our stakeholders on this subject
- [ ] 5.4.c We ensure that the models we develop provide, when relevant, at least a level of confidence together with each prediction made
- [ ] 5.4.d We determine the best compromises between performance and interpretability for each model we develop, which sometimes leads us to opt for a model that is simpler to explain to the stakeholders
- [ ] 5.4.e We master and implement advanced approaches for the explicability and interpretability of models

<details>
<summary>Expl5.4 :</summary>

Explanability and interpretability are key issues, in line with the growing demands for transparency, impartiality and accountability. In some cases, regulations even impose it.
Technical resources such as SHAP or LIME provide a first-hand introduction to the topic (see resources associated with this assessment element).

</details>

<details>
<summary>Ressources5.4 :</summary>

- (Web article) *[User confidence in systems involving Artificial Intelligence](https://blog.octo.com/la-confiance-des-utilisateurs-dans-les-systemes-impliquant-de-lintelligence-artificielle/)*, Blog Octo Technologies, October 2019
- (Technical guide) *[Interpretable Machine Learning, A Guide for Making Black Box Models Explainable](https://christophm.github.io/interpretable-ml-book/)*, Christoph Molnar
- (Web article) *[Understanding model predictions with LIME](https://towardsdatascience.com/understanding-model-predictions-with-lime-a582fdff3a3b)*, blog L. Hulstaert, 2018
- (Software & Tools) *[SHAP](https://github.com/slundberg/shap): A game theoretic approach to explain the output of any machine learning model*.
- (Software & Tools) *[Shapash](https://github.com/MAIF/shapash)*: a MAIF Datalab project which aims to make machine learning interpretable and understandable by everyone. It provides several types of visualization that display explicit labels that everyone can understand
- (Software & Tools) *[FACET](https://github.com/BCG-Gamma/facet)*: a BCG Gamma project of an open source library for human-explainable AI. It combines sophisticated model inspection and model-based simulation to enable better explanations of supervised machine learning models
- (Web article) In some cases, regulations impose being able to explain how an automated system came to a certain outcome (see for example [article 22 of the GDPR in the European Union](https://www.cnil.fr/fr/reglement-europeen-protection-donnees/chapitre3#Article22), [article 10 of the "Informatique & Libertés" law in France](https://www.legifrance.gouv.fr/affichTexteArticle.do;?idArticle=LEGIARTI000037090394&cidTexte=LEGITEXT000006068624&dateTexte=20180624), cited in particular in the [Hippocratic Oath for data scientist](https://hippocrate.tech/).

</details>

---

Q5.5 : **Transparency towards stakeholders interacting with an AI model**  
Your organisation uses for its own account, provides to its customers or operates on behalf of its customers applications based on AI models with which users can interact. What measure does it implement to inform users?

R5.5 :  
_(Type: multiple responses possible)_  
_(Select all response items that correspond to practices in your organisation. Please note that some combinations would not be coherent)_  
_(Specific risk domain: use of AI models, provision or operation of AI model-based applications for customers or third parties)_

- [ ] 5.5.a Our organisation does not use AI models on its own behalf or on behalf of its clients, and does not provide its clients with applications based on AI models | _(Concerned / Not concerned)_
- [ ] 5.5.b Users are not informed that they are interacting with an AI model developed with machine learning methods
- [ ] 5.5.c An information notice is made available in the terms and conditions of the system or an equivalent document, freely accessible
- [ ] 5.5.d The system or service is explicit to the user that an AI model is being used
- [ ] 5.5.e The system or service provides the user with additional information on the results it would have provided in slightly different scenarios (e.g. "counterfactual explanations" such as the smallest change in input data that would have resulted in a given different output)
- [ ] 5.5.f We are pionneers in using public AI registers, enabling us to provide transparency to our stakeholders and to capture user feedbacks

<details>
<summary>Expl5.5 :</summary>

Using automatic systems based on models whose rules have been "learned" (and not defined and formalised) questions the functioning of organisations but also the relationship of users to digital systems and services. In most cases it is important to inform users that they are not interacting with conventional business rules.

</details>

<details>
<summary>Ressources5.5 :</summary>

- (Academic paper) *[Counterfactual Explanations without Opening the Black Box: Automated Decisions and the GDPR](https://arxiv.org/abs/1711.00399)*, S. Wachter, B. Mittelstadt, C. Russell, 2018
- (Technical guide) *[Interpretable Machine Learning - Counterfactual explanations](https://christophm.github.io/interpretable-ml-book/counterfactual.html)*, C. Molnar, 2020
- (Web article) *[AI registers: finally, a tool to increase transparency in AI/ML](https://towardsdatascience.com/ai-registers-finally-a-tool-to-increase-transparency-in-ai-ml-f5694b1e317d)*, Natalia Modjeska, December 2020
- (Whitepaper) *[Public AI Registers: Realising AI transparency and civic participation in government use of AI](https://uploads-ssl.webflow.com/5c8abedb10ed656ecfb65fd9/5f6f334b49d5444079726a79_AI%20Registers%20-%20White%20paper%201.0.pdf)*, Saidot, Septembre 2020

</details>

---
---

### Section 6 - Anticipating, monitoring and minimising the negative externalities of data science activities

**[Negative externalities]**

The implementation of an automatic system based on an AI model can generate negative social and environmental externalities. Awareness of this is essential, as well as anticipating, monitoring and minimising the various negative impacts.

[_[⇧ back to the list of sections](#evaluation-framework-to-assess-the-maturity-of-an-organisation)_]  

---

Q6.1 : **CO2 impact**  
About the CO2 impact of the data science activity in your organisation:

R6.1 :  
_(Type: multiple responses possible)_  
_(Select all the answer items that correspond to practices in your organisation)_

- [ ] 6.1.a At this stage we have not looked at the CO2 impact of our data science activity or our AI models
- [ ] 6.1.b We have developed indicators that define what we want to measure regarding the CO2 impact of our data science activity or our models
- [ ] 6.1.c We measure our indicators regularly
- [ ] 6.1.d We include their measurements in the model identity cards
- [ ] 6.1.e Monitoring our indicators on a regular basis is a formalised and controlled process, from which we define and drive improvement objectives
- [ ] 6.1.f The CO2 impact of our data science activity or our models is made transparent to our counterparts and the general public

<details>
<summary>Expl6.1 :</summary>

It is important to question and raise awareness of environmental costs. In particular one can: (i) measure the environmental cost of data science projects, (ii) publish transparently their environmental impact, expliciting the split between train and production phases, (iii) improve on these indicators by working on different levers (e.g. infrastructure, model architecture, transfer learning, etc.).

</details>

<details>
<summary>Ressources6.1 :</summary>

- (Software & Tools) *[ML Impact Calculator](https://mlco2.github.io/impact/)*
- (Software & Tools) *[Code Carbon](https://codecarbon.io/)*: python library for evaluation the carbon cost of executing a script
- (Web article) (In French) *[IA durable : ce que les professionnels de la donnée peuvent faire](https://medium.com/quantmetry/ia-durable-et-sobri%C3%A9t%C3%A9-num%C3%A9rique-ce-que-les-professionnels-de-la-donn%C3%A9e-peuvent-faire-5782289b73cc)*, Geoffray Brerelut and Grégoire Martinon, May 2021
- (Web article) *[The carbon impact of artificial intelligence](https://www.nature.com/articles/s42256-020-0219-9)*, Payal Dhar, 2020
- (Web article) *[AI and Compute](https://openai.com/blog/ai-and-compute/)*, OpenAI, 2018
- (Academic paper) *[Green AI](https://cacm.acm.org/magazines/2020/12/248800-green-ai/fulltext)*, R. Schwart et al. 2020
- (Academic paper) *[Energy and Policy Considerations for Deep Learning in NLP](https://aclanthology.org/P19-1355/)*, E. Strubell et al. 2019
- (Public declaration) (In French) *[DÉPLOYER LA SOBRIÉTÉ NUMÉRIQUE](https://theshiftproject.org/article/deployer-la-sobriete-numerique-rapport-shift/)*, The Shift Project, 2020
- (Web article) *[How to stop data centres from gobbling up the world’s electricity](https://www.nature.com/articles/d41586-018-06610-y)*, Nicolas Jones, 2018
- (Web article) *[AI and Climate Change: How they’re connected, and what we can do about it](https://medium.com/@AINowInstitute/ai-and-climate-change-how-theyre-connected-and-what-we-can-do-about-it-6aa8d0f5b32c)*, AI Now Institute, 2019
- (Academic paper) *[The role of artificial intelligence in achieving the Sustainable Development Goals](https://www.nature.com/articles/s41467-019-14108-y)*, S. Vinuesa et al. 2020

</details>

---

Q6.2 : **Social impact**
In some cases, the implementation of an automatic system based on an AI model can generate negative externalities on upstream stakeholders (e.g. annotation of data), and on downstream stakeholders (e.g. automation of certain positions). Whenever you plan to develop or use an AI model, your organisation:

R6.2 :  
_(Type: single answer)_  
_(Select one answer only, which best corresponds to the level of maturity of the organisation on this topic)_

- [ ] 6.2.a At this stage we are not looking at the social impact of our data science activity or our AI models
- [ ] 6.2.b In some cases we study the social impact
- [ ] 6.2.c We study the social impact in each project
- [ ] 6.2.d We study the social impact in each project and it is documented in the end-to-end genealogy of each model
- [ ] 6.2.e We study the social impact in each project, it is documented in the end-to-end genealogy of each model, and we systematically engage in a dialogue with the relevant stakeholders upstream and downstream the value chain.

<details>
<summary>Expl6.2 :</summary>

It is important for an organisation to question and exchange with its stakeholders. This applies both downstream (e.g. automation of certain jobs) and upstream (e.g. data annotation tasks that can be very violent) the value chain.

</details>

---

Q6.3 : **Ethics and non-maleficence**  
Within your organisation:

R6.3 :  
_(Type: multiple responses possible)_  
_(Select all response items that correspond to practices in your organisation. Please note that some combinations would not be coherent)_

- [ ] 6.3.a At this stage we have not yet addressed the ethical dimension of our data science projects and activities
- [ ] 6.3.b We are studying the ethical dimension of our data science projects and activities, it is work in progress
- [ ] 6.3.c Employees involved in data science activities receive training in ethics
- [ ] 6.3.d Our organisation has adopted an ethics policy
- [ ] 6.3.e For projects justifying it, we set up an independent ethics committee or ask for the evaluation of an organisation validating the ethics of the projects

<details>
<summary>Expl6.3 :</summary>

Working with large volumes of data, some of which may be sensitive, using automatic systems based on models whose rules have been "learned" (and not defined and formalised) raises questions about the way organisations function and the individual responsibility of each contributor. It requires considering carefully the uses of such sytems. It is therefore important for the organisation to ensure that ethical issues are not unknown to its collaborators.
A recurring example is that some AI systems or services designed to adapt to user behaviour may influence users (e.g. by seeking to maximise their time of use or the money they spend) and present significant risks of manipulation or addiction.

</details>

<details>
<summary>Ressources6.3 :</summary>

- (Official report) Rapport *[Ethics and Responsibility of Public Algorithms](https://www.etalab.gouv.fr/wp-content/uploads/2020/01/Rapport-ENA-Ethique-et-responsabilit%C3%A9-des-algorithmes-publics.pdf)*, Etalab / ENA, January 2020, in French
- (Public declaration) *[Montreal Declaration for Responsible RNs](https://www.declarationmontreal-iaresponsable.com/la-declaration)*
- (Public declaration) *[Holberton-Turing Oath](https://www.holbertonturingoath.org/accueil)*
- (Public declaration) *[Hippocratic Oath for data scientist](https://hippocrate.tech/)*
- (Public declaration) *[Future of Life's AI principles](https://futureoflife.org/ai-principles/)*
- (Public declaration) *[International Charter for Inclusive AI](https://charteia.arborus.org/)*, Arborus and Orange
- (Course) *[Practical data ethics](https://ethics.fast.ai/)*, fast.ai: an excellent online course combining reading lists and instructional videos

</details>

---
---
