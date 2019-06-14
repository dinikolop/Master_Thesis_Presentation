---?color=white
@title[Introduction]

@snap[west text-white span-80]
@box[bg-blue](Connecting patient groups to biomedical research: a Linked Data approach using ICD10 and PubMed)
@snapend


@snap[south-east byline text-black text-06]
Vrije Universiteit Amsterdam<br/>
Articial Intelligence<br/>2<sup>nd</sup> KIM presentation<br/>
Supervised by Prof. Annette ten Teije
@snapend

---?color=linear-gradient(100deg, #fff1eb 50%, #4487F2 50%)
@title[Outline]

@snap[west text-center text-14 text-bold text-italic text-black  span-50]
Outline
@snapend

@snap[east text-center text-white span-45]
@ol[split-screen-list text-06](false)
- Context & Use Case
- Research Framework
- Some Preliminaries
- Methods
- Analysis
- Discussion

@olend
@snapend


---?color=linear-gradient(135deg, #fff1eb, #ffffff)

@title[Context & Use Case]

## @color[black](Context & Use Case)
@fa[arrow-down text-black]


+++?image=template/img/bg/c1.jpg&position=center&size=100% 65%
@title[Domain and Problem Statement]

@snap[north span-100]
@size[1.5em](Domain and problem area)
@snapend

@snap[west list-content-verbose  span-100]
@ul[list-bullets-blue]
- **Domain:** Health/patient care in combination to biomedical research
- **Problem:** Correlating patient groups to research output of academic hospitals
- A task that requires **knowledge** and **knowledge intensive processes**
@olend
<br><br>
@snapend

+++?color=linear-gradient(90deg, #ffffff 50%, #4487F2 50%)
@title[Text + Image Centered]

@snap[north-west span-40 text-center]
@color[#text-black](@size[1em](<u>Knowledge</u>))
@snapend

@snap[west list-content-verbose span-40]
<br>
@ul[text-black]
- Electronic Health Records (EHRs)
- Medical Classification Systems
- Databases with academic and scientific articles
- Controlled vocabularies
@ulend
@snapend


@snap[midpoint]
@box[bg-white mid-box rounded](@fa[user-injured fa-blue] @fa[sync-alt fa-blue] @fa[newspaper fa-blue])
@snapend

@snap[north-east span-40 text-black text-center]
@size[1em](<u>Knowledge Intensive Procedures</u>)
@snapendf

@snap[east list-content-verbose span-40]
<br>
@ul[text-black]
- Retrieving articles/patient-groups of interest
- Grouping articles or patient-groups
- Linking topics of articles to diagnosis codes
- Getting insights / evaluating
@ulend
@snapend


+++?image=template/img/bg/c1.jpg&position=bottom&size=100% 75%
@title[Use Case]
@snap[north span-100]
@size[1.5em](Use Case)

@snap[fragment]
@snap[span-80]
<br/><br/>
University Medical Centres (UMCs)
@snapend

@snap[east span-20]
<br/><br/><br/><br/>
![NFU](assets/img/nfu.png)
@snapend
@snapend
@snapend


@snap[south-west text-center span-30 fragment]
@size[0.4em](**Bridging three scopes**)
![NFU](assets/img/bridge.png)
@snapend

@snap[south span-30 text-center fragment]
@size[0.4em](**Citation scores above the world average**)
![NFU](assets/img/citation-impact-by-unive.png)
<br/>
@size[0.2em](Source: <a href="https://www.rathenau.nl/en/science-figures/output/publications/citation-impact-score-dutch-universities" >Rathenau Instituut</a>)
@snapend

@snap[south-east text-center span-33 list-content-concise text-04 fragment]
@size[1.1em](**ROBIJN project**)
@ul[]()
- Special patient groups:
  - with role to scientific developments.
  - frequently treated in UMCs.
- Distinguish these groups as **academic**.
- A model using labels.
- **9 labels**, 1 particular of interest: **"Science"**
  - Scientific output should cover developments in these patient groups
  - Objective linking between patients and scientific output.

@ulend
<br><br>
@snapend




+++?image=template/img/bg/c1.jpg&position=center&size=100% 65%
@title[Opportunity]
@snap[north span-100]
@size[1.5em](A.I. Opportunity)
@snapend


@snap[midpoint list-content-verbose span-100]
@ul[list-bullets-black](false)
- Knowledge Representation & Reasoning
- Implementation through **Knowledge Based Systems**
- Representation of domain knowledge: **Ontologies**
- Reasoning with **Semantic Web** tools
@ulend
<br><br>
@snapend


+++
@title[Interoperability]
@snap[north span-100]
@size[1.5em](Interoperability)
@snapend


@snap[west list-content-verbose span-100]
@ul[list-bullets-black](false)
- Various Disease Ontologies
  - Different content, focus, granularity
  - Different purpose, e.g: for statistics, retrieval, patient reports...
@snap[fragment]
- Considering community-based mapping efforts such as:
@snapend
@olend
<br><br>
@snapend


@snap[fragment]
@snap[south-west span-33]
![UMLS](assets/img/umls.jpeg)
@snapend

@snap[south span-33]
![BioPortal](assets/img/logo.png)
@snapend

@snap[south-east span-33]
![snomed](assets/img/SNOMED-CT-5.png)
@snapend


+++?image=template/img/bg/c1.jpg&position=center&size=100% 65%
@title[Knowledge sources]
@snap[north span-100]
@size[1.5em](Knowledge sources)
@snapend

@snap[west text-center span-50 text-07]
<u>ICD10</u> <br/>

@ul[list-content-verbose list-bullets-black text-06](false)

- International Classification of Diseases - 10<sup>th</sup> revision
- Reporting diagnosis codes for patients.
- Monohierarchical Tree Structure
- Statistical classification system:
  - Mutually exclusive nodes
  - Exhaustive
  - Residual categories
@ulend

@snapend

@snap[east text-center text-07 span-50]
<u>MeSH</u><br/>

@ul[list-content-verbose list-bullets-black text-06](false)

- Medical Subject Headings
- Controlled vocabulary created by NLM.
- Hierarchical terminology for indexing biomedical info
- Indexing of citation in MEDLINE Database
- MEDLINE is accessed by **PubMed**:
    - database, search engine for biomedical articles
    - over 29 million citations
@ulend
@snapend

+++
@title[Semantic Web technologies]
@snap[north span-100]
@size[1.5em](Semantic Web technologies)
@snapend


@snap[west text-center text-black span-80]
@ol[split-screen-list text-06](false)
- Ontology representation based on **RDF**.<br/><br/>

- Ontology creation based on **Linked Data** principles.<br/><br/>
- Querying through **SPARQL**.<br/><br/>
@olend
@snapend



@snap[south-west span-10]
![RDF](assets/img/rdf.png)
@snapend

@snap[south span-53]
![sparql](assets/img/linked.jpeg)
@snapend

@snap[south-east span-23]
![sparql](assets/img/sparql.png)
@snapend


---?color=linear-gradient(135deg, #fff1eb, #ffffff)

@title[Research Framework]

## @color[black](Research Framework)
@fa[arrow-down text-black]


+++

@title[Main points]
@snap[north span-100]
@size[1.5em](Main points)
@snapend

@snap[west text-center text-black span-80]
@ol[split-screen-list text-06](false)
- **Problem:** correlation between patient groups and articles.
- **Motivation:** Dutch UMC case.
- **Approach:** Knowledge Engineering using Linked Data methods and tools.

@olend
@snapend

+++?color=linear-gradient(135deg, #ffffff, #4487F2)
@title[Main Research Question]

@snap[midpoint span-100]
@box[bg-white text-center text-09 box-wide-padding](Main Research Question # How can investigation of the correlation between patient groups and academic articles be achieved by following a Knowledge Engineering approach using Semantic Web technologies?)
@snapend


+++?color=linear-gradient(135deg, #ffffff, #4487F2)
@title[First Subquestion]

@snap[midpoint span-100]
@box[bg-white text-center text-09 box-wide-padding](1<sup>st</sup> Sub-question # How the **domain knowledge** about: <br/><br/>(1) health conditions describing patient groups with _ICD10_, <br/> (2) topics about diseases in academic articles of _PubMed_, and <br/> (3) _mappings_ between them, <br/><br/> can be gathered, created if necessary, and be represented?)
@snapend


+++?color=linear-gradient(135deg, #ffffff, #4487F2)
@title[Second Subquestion]

@snap[midpoint text-09 span-100]
@box[bg-white text-center text-09 box-wide-padding](2<sup>nd</sup> Sub-question # What is the quality of the potential mappings between ICD10 and MeSH, in terms of relevance and distribution within the various sources?)
@snapend

+++?color=linear-gradient(135deg, #ffffff, #4487F2)
@title[Second Subquestion]

@snap[midpoint text-09 span-100]
@box[bg-white text-center text-09 box-wide-padding](3<sup>rd</sup> Sub-question # How can the Semantic Web technology of SPARQL be used for obtaining interesting insights about the patient groups and articles of a specific UMC?)
@snapend

@title[Some Preliminaries]

## @color[black](Some preliminaries)
@fa[arrow-down text-black]

---?color=linear-gradient(135deg, #fff1eb, #ffffff)

@title[Methods]

## @color[black](Methods)
@fa[arrow-down text-black]

---?color=linear-gradient(135deg, #fff1eb, #ffffff)

@title[Analysis]

## @color[black](Analysis)
@fa[arrow-down text-black]

---?color=linear-gradient(135deg, #fff1eb, #ffffff)

@title[Discussion]

## @color[black](Discussion)
@fa[arrow-down text-black]

---
@title[Questions #4]

@snap[east span-50]
![QUESTIONS-4](template/img/questions-4.png)
@snapend

@snap[south-west template-note text-gray]
contact: d.nikolopoulos@vu.nl
@snapend



---

![TIP](template/img/tip.png)
<br>
For the best viewing experience, press F for fullscreen.
@css[template-note](We recommend using the *SPACE* key to navigate between slides.)

---?include=template/md/split-screen/PITCHME.md

---?include=template/md/sidebar/PITCHME.md

---?include=template/md/list-content/PITCHME.md

---?include=template/md/boxed-text/PITCHME.md

---?include=template/md/image/PITCHME.md

---?include=template/md/sidebox/PITCHME.md

---?include=template/md/code-presenting/PITCHME.md

---?include=template/md/header-footer/PITCHME.md

---?include=template/md/quotation/PITCHME.md

---?include=template/md/announcement/PITCHME.md

---?include=template/md/about/PITCHME.md

---?include=template/md/wrap-up/PITCHME.md

---?image=template/img/presenter.jpg
@title[The Template Docs]

@snap[west sign-off]
### Now it's your turn.
@snapend

@snap[south docslink text-gold span-100]
For supporting documentation see the [The Template Docs](https://gitpitch.com/docs/the-template)
@snapend
