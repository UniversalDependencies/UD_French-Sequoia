# Summary
UD_French-Sequoia is an automatic conversion of the Sequoia Treebank corpus [French Sequoia corpus](http://deep-sequoia.inria.fr).

# Introduction
UD_French-Sequoia is an automatic conversion of the Sequoia Treebank corpus [French Sequoia corpus](http://deep-sequoia.inria.fr).
The conversion was done with the [Grew software](http://grew.fr) and the Graph Rewriting System [described here](https://gitlab.inria.fr/grew/SSQ_UD).

## Origin
The first version of the Sequoia Corpus was presented in (Candito & Seddah, 2012)

## Splitting
The whole corpus contains 70,624 tokens in 3,099 sentences.

In **UD_French-Sequoia**, data were randomly split into:

 * `fr_sequoia-ud-test.conllu`: 10,050 tokens in 456 sentences
 * `fr_sequoia-ud-dev.conllu`: 10,013 tokens in 412 sentences
 * `fr_sequoia-ud-train.conllu`: 50,561 tokens in 2,231 sentences

## Genres
The original sentences of the corpus are taken from:

 * French Europarl (`sent_id` prefix: `Europar.550`)
 * Wikipédia Fr (`sent_id` prefix: `frwiki_50.1000`)
 * Newspaper *Est Républicain* (`sent_id` prefix: `annodis.er`)
 * European Medicines Agency (`sent_id` prefix: `emea-fr-dev` and `emea-fr-test`)

# Acknowledgments

The conversion has been performed by Bruno Guillaume with the Graph Rewriting System [described here](https://gitlab.inria.fr/grew/SSQ_UD) developed by Bruno Guillaume and Guy Perrier.

The Sequoia Corpus was presented in (Candito & Seddah, 2012) and revised later, notably during the project of deep annotation described in (Candito & al. 2014) and (Perrier & al. 2014).

# References
**(Candito & Seddah, 2012)** Marie Candito, Djamé Seddah. [Le corpus Sequoia : annotation syntaxique et exploitation pour l'adaptation d'analyseur par pont lexical](https://hal-univ-diderot.archives-ouvertes.fr/hal-00698938/). TALN 2012 - 19e conférence sur le Traitement Automatique des Langues Naturelles, Jun 2012, Grenoble, France. 2012.

**(Candito & al. 2014)** Marie Candito, Guy Perrier, Bruno Guillaume, Corentin Ribeyre, Karën Fort, Djamé Seddah and Éric de la Clergerie. (2014) [Deep Syntax Annotation of the Sequoia French Treebank](http://hal.inria.fr/docs/00/97/15/74/PDF/deep_sequoia.final_with_keywords.pdf). *Proc. of LREC 2014*, Reykjavic, Iceland.

**(Perrier & al. 2014)** Guy Perrier, Marie Candito, Bruno Guillaume, Corentin Ribeyre, Karën Fort and Djamé Seddah. (2014) [Un schéma d'annotation en dépendances syntaxiques profondes pour le français](http://talc2.loria.fr/deep-sequoia/papers/syntaxe_profonde.pdf). *Proc. of TALN 2014*, Marseille, France.

# Changelog

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
Genre: wiki medical new nonfiction
Lemmas: converted from manual
UPOS: converted from manual
XPOS: not available
Features: converted from manual
Relations: converted from manual
Contributors: Candito, Marie; Seddah, Djamé; Perrier, Guy; Guillaume, Bruno
Contributing: elsewhere
Contact: bruno.guillaume@inria.fr
===============================================================================
