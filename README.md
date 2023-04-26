# Summary
**UD_French-Sequoia** is an automatic conversion of the [SUD_French-Sequoia](https://github.com/surfacesyntacticud/SUD_French-Sequoia) treebank, which comes from the former corpus [French Sequoia corpus](http://deep-sequoia.inria.fr).

# Introduction
**UD_French-Sequoia** is an automatic conversion of the [SUD_French-Sequoia](https://github.com/surfacesyntacticud/SUD_French-Sequoia) treebank, which comes from the former corpus [French Sequoia corpus](http://deep-sequoia.inria.fr).
The French Sequoia corpus was converted in April 2023 to SUD with the Grew rewriting system [described here](https://gitlab.inria.fr/grew/DSQ_SUD).
Since this date, the corpus is maintained in SUD and converted to UD.

## Origin
The first version of the Sequoia Corpus was presented in [(Candito & Seddah, 2012)](https://hal-univ-diderot.archives-ouvertes.fr/hal-00698938/).

## Splitting
The whole corpus contains 70,546 tokens in 3,099 sentences.

In **UD_French-Sequoia**, data were randomly split into:

 * `fr_sequoia-ud-test.conllu`: 10,044 tokens in 456 sentences
 * `fr_sequoia-ud-dev.conllu`: 9,999 tokens in 412 sentences
 * `fr_sequoia-ud-train.conllu`: 50,503 tokens in 2,231 sentences

## Genres
The original sentences of the corpus are taken from:

 * French Europarl (`sent_id` prefix: `Europar.550`)
 * Wikipédia Fr (`sent_id` prefix: `frwiki_50.1000`)
 * Newspaper *Est Républicain* (`sent_id` prefix: `annodis.er`)
 * European Medicines Agency (`sent_id` prefix: `emea-fr-dev` and `emea-fr-test`)

# Acknowledgments

The conversion has been performed by Bruno Guillaume with the Graph Rewriting System [described here](https://gitlab.inria.fr/grew/DSQtoSUD) developed by Bruno Guillaume and Guy Perrier.

The Sequoia Corpus was presented in [(Candito & Seddah, 2012)](https://hal-univ-diderot.archives-ouvertes.fr/hal-00698938/) and revised later, notably during the project of deep annotation described in [(Candito & al. 2014)](http://hal.inria.fr/docs/00/97/15/74/PDF/deep_sequoia.final_with_keywords.pdf) and [(Perrier & al. 2014)](http://talc2.loria.fr/deep-sequoia/papers/syntaxe_profonde.pdf).

# References
**(Candito & Seddah, 2012)** Marie Candito, Djamé Seddah. [Le corpus Sequoia : annotation syntaxique et exploitation pour l'adaptation d'analyseur par pont lexical](https://hal-univ-diderot.archives-ouvertes.fr/hal-00698938/). TALN 2012 - 19e conférence sur le Traitement Automatique des Langues Naturelles, Jun 2012, Grenoble, France. 2012.

**(Candito & al. 2014)** Marie Candito, Guy Perrier, Bruno Guillaume, Corentin Ribeyre, Karën Fort, Djamé Seddah and Éric de la Clergerie. (2014) [Deep Syntax Annotation of the Sequoia French Treebank](http://hal.inria.fr/docs/00/97/15/74/PDF/deep_sequoia.final_with_keywords.pdf). *Proc. of LREC 2014*, Reykjavík, Iceland.

**(Perrier & al. 2014)** Guy Perrier, Marie Candito, Bruno Guillaume, Corentin Ribeyre, Karën Fort and Djamé Seddah. (2014) [Un schéma d'annotation en dépendances syntaxiques profondes pour le français](http://talc2.loria.fr/deep-sequoia/papers/syntaxe_profonde.pdf). *Proc. of TALN 2014*, Marseille, France.

**(Bonfante & al. 2018)** Guillaume Bonfante, Bruno Guillaume, Guy Perrier. [Application of Graph Rewriting to Natural Language Processing](https://hal.inria.fr/hal-01814386). ISTE Wiley, 1, pp.272, 2018, Logic, Linguistics and Computer Science Set.

# Changelog
* 2023-05-15 v2.12
  * The treebank is now maintained in SUD and converted to UD. See https://github.com/surfacesyntacticud/SUD_French-Sequoia
* 2020-11-14 v2.7
  * No major change
* 2020-05-15 v2.6
  * Fix some annotation errors found during PARSEME-Fr project
  * Fix some inconsistent lemmas and morphological features
* 2019-11-15 v2.5
  * Update the conversion process to improve consistency with other French treebanks:
     * expletive annotation with relations `expl:subj`, `expl:comp` and `expl:pass`
     * `aux` -> `aux:tense`
     * `MWEPOS` -> `EXTPOS`
* 2019-05-15 v2.4
  * Several corrections in the original corpus (often found during PARSEME-Fr annotation project)
  * Update the conversion process (mainly to handle new validation rules)
* 2018-11-15 v2.3
  * Change date annotation
  * Improve NOUN/PROPN distinction
  * Several corrections in the original corpus and in the conversion process
* 2018-04-15 v2.2
  * Subtyping of the `obl` relation with 3 relations `obl:arg`, `obl:mod`, `obl:agent`
  * Several corrections in the original corpus and in the conversion process
* 2017-11-15 v2.1
  * Manual corrections in the original Treebank
  * Application of an updated conversion system, taking into account new decisions taken for harmonisation of several French Treebanks (causative, copules, auxiliaries)
* 2017-03-01 v2.0
  * First release in UD


=== Machine-readable metadata (DO NOT REMOVE!) ================================
Data available since: UD v2.0
License: LGPL-LR
Includes text: yes
Genre: wiki medical news nonfiction
Lemmas: converted from manual
UPOS: converted from manual
XPOS: not available
Features: converted from manual
Relations: converted from manual
Contributors: Candito, Marie; Seddah, Djamé; Perrier, Guy; Guillaume, Bruno
Contributing: elsewhere
Contact: bruno.guillaume@inria.fr
===============================================================================
