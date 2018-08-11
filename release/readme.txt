RRG TreeBank
============
bootstrapped from Stanford/UD v.1 annotations, complemented with PropBank annotations

1. building an RRG wrapper around Stanford parser, replicate 1997 and 2005 examples
1.a parse transformation
1.b validation by templates

2. apply this wrapper to a corpus with Stanford-compatible annotation, i.e., a UD v.1 corpus or PTB+Stanford conversion
2.a structural validation (on all: to make sure we arrive at valid XML files)
2.b parse transformation (on dev set/answers)
2.c no additional validation templates

3. improve the output by integrating semantic annotations, esp. PropBank

content
-------
RRG1997.*.xml
TIGER edition of the syntax examples of
Robert D. Van Valin and Randy J. Lapolla (1997), Syntax. Structure, meaning and function. Cambridge University Press, New York.
Note that these are not annotated, but have been converted automatically using (manually corrected) output of the Stanford parser
Also note that as of v.013, these are updated to RRG05 representations
Note that these are frozen at v.013

RRG2005.*.xml
TIGER edition of the syntax examples of
Robert D. Van Valin (2005), Exploring the Syntax-Semanrics Interface. CUP
Note that unlike the RRG theory, we preserve AAJ and ARG labels as well as explicit operators for selected adverbs
Note that these are frozen at v.013

EWT.*.xml
TIGER edition of RRG parses derived from UD + PropBank (EWT corpus)
v.014 edition (currently being compiled) based on UD, only
v.015 edition (yet to come) integrating PB

scripts*xml
sh and sparql scripts for conversion

history
-------
- 2018-08-10 v.014 (EWT/UD conversion, developed on dev/answers) -- CC
- 2018-07-15 v.013 (RRG1997+RRG2005, keeping ARG/AAJ as in RRG1997) -- CC
- 2018-07-08 v.012 (RRG1997, RRG template validation ok except for treatment of "have to" as core cosubordination) -- CC
- 2018-07-04 v.011 (RRG1997, structural validation) -- CC
- 2018-07-03 v.010 (RRG1997, all plausible, not validated, yet) -- CC
- 2018-05-21 repository created -- CC 

contributors
------------
CC - chiarcos@informatik.uni-frankfurt.de