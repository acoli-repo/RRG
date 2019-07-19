
# RRG Corpus
Treebank according to the Role and Reference Grammar (van Valin and Lapolla, 1997)

Constructed from manual annotations for syntax (Universal Dependencies) and frame semantics (PropBank).

## Annotated data

We provide a full conversion of the English Web Treebank. Converters have been developed against the dev/answers subset only. For reasons of copyright, we cannot disseminate the EWT just yet, the source data can be acquired from https://github.com/UniversalDependencies/UD_English-EWT (version 1.4) and https://github.com/propbank/propbank-release/tree/master/data/google/ewt. The interested user may run our scripts to produce that data himself. However, note that the PropBank data omits several files, so before running our scripts, make sure to operate on the same files.

In addition, we provide RRG gold data based on English examples from Van Valin and LaPolla (1997) and van Valin (2008). For these, UD v.1.4 annotations have been created using the Stanford Parser and (in parts) manually corrected. We did not correct systematic errors that are also found in the UD data (e.g., attachment of controller of a relative clause as subject of the relative clause).

Observations on the source data:
* Occasional errors in UD annotations (e.g., attachment of controller of a relative clause as subject of the relative clause). These have not been fixed.
* Occasional mismatches between PB and RRG semantic roles. We preserve the PB split between modifiers (periphery) and core arguments (ARG), unless a "modifier" occurs as syntactic subject or direct object.

## Content

<code>release/</code>
+ generated RRG data, TIGER XML format; 
  also includes generation scripts

<code>doc/</code>
+ documentation (papers, slides)
  
<code>input/</code>
+ text and annotated source documents

## References and Usage

The code for building the RRG Corpus is licensed under the Apache License v.2, see the scripts in the release folder. The RRG gold data (textbook examples) provided in the release folder also fall under this license.

The EWT data is at pre-release stage, the formal license will be decided depending on copyright clearance for the source data. We aim for a publication of the annotations (possibly excluding the source text) under CC-BY. Until then, this data can be rebuilt locally using our scripts, but use at your own risk, and drop us a line when doing so.

When referring to this data, please attribute us as follows:

* Christian Chiarcos and Christian Fäth (2019), Graph-Based Annotation Engineering: Towards a Gold Corpus for Role and Reference Grammar, in Eskevich et al. (eds.), Proceedings of the 2nd Conference on Language, Data and Knowledge (LDK 2019), Leipzig, Germany, May 2019, Schloss Dagstuhl -- Leibniz-Zentrum fuer Informatik, OpenAccess Series in Informatics (OASIcs; 70), doi 10.4230/OASIcs.LDK.2019.9, p. 9:1--9:11

## History

Creating a gold corpus for Role and Reference Grammar is meant to be a showcase for the annotation engineering framework currently developed by CC, CF and others (https://github.com/acoli-repo/conll-rdf). This is an ideal test case as this goes far beyond conversion from one format to another. Instead, several sources of information (syntactic annotations, morphological annotations, semantic annotations, lexical knowledge bases) are decomposed and combined for deriving a representation that is richer than any of its source formats.

- 2019-08-20 v.015 corpus and workflow presented at the International Conference on Role and Reference Grammar 2019 (RRG2019), Buffalo, NY -- MRP, CC and CF
- 2019-05-22 v.015 corpus and workflow presented at the 2nd Conference on Language, Data and Knowledge (LDK-2019), Leipzig, Germany -- CC and CF
- since Aug 2018 v.015 (EWT/UD+PB, developed on dev/answers) -- CC
- 2018-08-10 release v.014 (EWT/UD, developed on dev/answers) -- CC
- 2018-07-15 release v.013 (RRG1997+RRG2005, keeping ARG/AAJ as in RRG1997) -- CC
- 2018-07-08 release v.012 (RRG1997, RRG template validation ok except for treatment of "have to" as core cosubordination) -- CC
- 2018-07-04 release v.011 (RRG1997, structural validation) -- CC
- 2018-07-03 release v.010 (RRG1997, all plausible, not validated, yet) -- CC
- 2018-05-21 EWT repository created, begun parser development for corpus examples -- CC 
- 2018-01-09 internal RRG repository created, begun parser development for textbook examples -- CC
- since 2015 development of the CoNLL-RDF technology stack, see https://github.com/acoli-repo/conll-rdf -- CC, CF and others

For a piece of related research, compare https://rrgbank.phil.hhu.de, an effort to derive RRG annotations from manual annotations of the Penn Treebank conducted in the TreeGraSP project (07/2017-06/2022). Similar to our effort, the RRGBank aims to provide a major RRG corpus for English, but no data has been released thus far. A key difference between both approaches is that their annotations are derivative from one particular type of source annotation (Penn Treebank), whereas we combine different pieces of information in order to obtain a representation that is richer than any of the source formats.

## Contributors and Acknowledgements

- CC - Christian Chiarcos, ACoLi, Goethe-Universität Frankfurt, Germany, chiarcos@informatik.uni-frankfurt.de
- CF - Christian Fäth, ACoLi, Goethe-Universität Frankfurt, Germany, faeth@informatik.uni-frankfurt.de
- MRP - Monika Rind-Pawlowski, ACoLi/LiODi, Goethe-Universität Frankfurt, Germany, pawlowski@lingua.uni-frankfurt.de

The research of Christian Chiarcos and Monika Rind-Pawlowski has been conducted in the context of the Early Carreer Research Group "Linked Open Dictionaries (LiODi)'', funded 2015-2020 by the German Ministry of Education and Research (BMBF) in the context of the 2014/2015 eHumanities programme. The research of Christian Fäth was partially supported by the Special Information Service "Linguistics'' (FID Linguistik), funded 2016-2019 by the German Research Foundation (DFG).

Brought to you by ACoLi/LiODi 2015-2018.
