# Using the `push` command, [spaCy-huggingface-hub](https://github.com/explosion/spacy-huggingface-hub) will generate a model card using your model's `meta.json` file.
# [Example](https://huggingface.co/spacy/en_core_web_sm)
---
tags:
- spacy
- new-languages-for-nlp
language:
- kli
license: mit
model-index:
- name: klingon_sub_sm
  results:
  - task:
      name: NER
      type: token-classification
    metrics:
    - name: NER Precision
      type: precision
      value: 0.8463095057
    - name: NER Recall
      type: recall
      value: 0.8377904647
    - name: NER F Score
      type: f_score
      value: 0.8420284384
  - task:
      name: POS
      type: token-classification
    metrics:
    - name: POS Accuracy
      type: accuracy
      value: 0.9725066923
  - task:
      name: SENTER
      type: token-classification
    metrics:
    - name: SENTER Precision
      type: precision
      value: 0.9205049471
    - name: SENTER Recall
      type: recall
      value: 0.8899003892
    - name: SENTER F Score
      type: f_score
      value: 0.904943986
  - task:
      name: UNLABELED_DEPENDENCIES
      type: token-classification
    metrics:
    - name: Unlabeled Dependencies Accuracy
      type: accuracy
      value: 0.9166876131
  - task:
      name: LABELED_DEPENDENCIES
      type: token-classification
    metrics:
    - name: Labeled Dependencies Accuracy
      type: accuracy
      value: 0.9166876131
---
### Details: https://spacy.io/models/en#en_core_web_sm
Klingon pipeline optimized for CPU. Components: tok2vec, tagger, parser, senter, ner, lemmatizer.
| Feature | Description |
| --- | --- |
| **Name** | `klingon_sub_sm` |
| **Version** | `3.2.0` |
| **spaCy** | `>=3.2.0,<3.3.0` |
| **Default Pipeline** | `tok2vec`, `tagger`, `parser`, `lemmatizer`, `ner` |
| **Components** | `tok2vec`, `tagger`, `parser`, `senter`, `lemmatizer`, `ner` |
| **Vectors** | 0 keys, 0 unique vectors (0 dimensions) |
| **Sources** | [OntoNotes 5](https://catalog.ldc.upenn.edu/LDC2013T19) (Ralph Weischedel, Martha Palmer, Mitchell Marcus, Eduard Hovy, Sameer Pradhan, Lance Ramshaw, Nianwen Xue, Ann Taylor, Jeff Kaufman, Michelle Franchini, Mohammed El-Bachouti, Robert Belvin, Ann Houston)<br />[ClearNLP Constituent-to-Dependency Conversion](https://github.com/clir/clearnlp-guidelines/blob/master/md/components/dependency_conversion.md) (Emory University)<br />[WordNet 3.0](https://wordnet.princeton.edu/) (Princeton University) |
| **License** | `MIT` |
| **Author** | [New Languages for NLP](https://newnlp.princeton.edu) |

### Label Scheme

<details>

<summary>View label scheme (114 labels for 4 components)</summary>

| Component | Labels |
| --- | --- |
| **`tagger`** | `$`, `''`, `,`, `-LRB-`, `-RRB-`, `.`, `:`, `ADD`, `AFX`, `CC`, `CD`, `DT`, `EX`, `FW`, `HYPH`, `IN`, `JJ`, `JJR`, `JJS`, `LS`, `MD`, `NFP`, `NN`, `NNP`, `NNPS`, `NNS`, `PDT`, `POS`, `PRP`, `PRP$`, `RB`, `RBR`, `RBS`, `RP`, `SYM`, `TO`, `UH`, `VB`, `VBD`, `VBG`, `VBN`, `VBP`, `VBZ`, `WDT`, `WP`, `WP$`, `WRB`, `XX`, ```` |
| **`parser`** | `ROOT`, `acl`, `acomp`, `advcl`, `advmod`, `agent`, `amod`, `appos`, `attr`, `aux`, `auxpass`, `case`, `cc`, `ccomp`, `compound`, `conj`, `csubj`, `csubjpass`, `dative`, `dep`, `det`, `dobj`, `expl`, `intj`, `mark`, `meta`, `neg`, `nmod`, `npadvmod`, `nsubj`, `nsubjpass`, `nummod`, `oprd`, `parataxis`, `pcomp`, `pobj`, `poss`, `preconj`, `predet`, `prep`, `prt`, `punct`, `quantmod`, `relcl`, `xcomp` |
| **`senter`** | `I`, `S` |
| **`ner`** | `CARDINAL`, `DATE`, `EVENT`, `FAC`, `GPE`, `LANGUAGE`, `LAW`, `LOC`, `MONEY`, `NORP`, `ORDINAL`, `ORG`, `PERCENT`, `PERSON`, `PRODUCT`, `QUANTITY`, `TIME`, `WORK_OF_ART` |
</details>
### Accuracy
| Type | Score |
| --- | --- |
| `TOKEN_ACC` | 99.93 |
| `TOKEN_P` | 99.57 |
| `TOKEN_R` | 99.58 |
| `TOKEN_F` | 99.57 |
| `TAG_ACC` | 97.25 |
| `SENTS_P` | 92.05 |
| `SENTS_R` | 88.99 |
| `SENTS_F` | 90.49 |
| `DEP_UAS` | 91.67 |
| `DEP_LAS` | 89.80 |
| `ENTS_P` | 84.63 |
| `ENTS_R` | 83.78 |
| `ENTS_F` | 84.20 |
