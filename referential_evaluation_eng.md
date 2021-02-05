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

- 1.1.a Not yet identified
- 1.1.b Partially identified or in the process of identification
- 1.1.c Identified
- 1.1.d Identified and known by our collaborators
- 1.1.e Identified, documented and known by our collaborators

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

- 1.2.a Informal, based on individual responsibility and competence
- 1.2.b Formalized and accessible to all collaborators
- 1.2.c Formalized and known by collaborators
- 1.2.d Formalized, known by employees, documented for each processing of personal or confidential data

<details>
<summary>Expl1.2 :</summary>

It is a question of questioning the management of personal or confidential data (storage, access, transfer, protection, responsibilities...), and documenting the choices made.

</details>

---

Q1.3: **Regulatory surveillance**  
Is a regulatory surveillance process in place, either internally or via a specialised service provider, to find out about applicable changes that have an impact on your organisation?

R1.3 :  
_(Type: single answer)_  
_(Select one answer only, which best corresponds to the level of maturity of the organisation on this topic)_

- 1.3.a We do not really monitor the regulatory environment
- 1.3.b We keep an informal watch, each employee sends back information via internal communication channels
- 1.3.c We have a formal surveillance, with identified collaborators in charge and a documented process

<details>
<summary>Expl1.3 :</summary>

In addition to identifying regulations and compliance approaches, it is important to set up a surveillance processe to know and follow **the evolution** of applicable regulations (which can be very specific in certain sectors). Interesting example(s) : [Welfare surveillance system violates human rights, Dutch court rules](https://www.theguardian.com/technology/2020/feb/05/welfare-surveillance-system-violates-human-rights-dutch-court-rules).

</details>