RRG TreeBank
============
(to be) bootstrapped from Stanford/UD v.1 annotations, complemented with PropBank annotations

1. building an RRG wrapper around Stanford parser, replicate 1997 examples
1.a parse transformation
1.b validation by templates

2. apply this wrapper to a corpus with Stanford-compatible annotation, i.e., a UD v.1 corpus or PTB+Stanford conversion
2.a structural validation (on all: to make sure we arrive at valid XML files)
2.b parse transformation (on dev set)
2.c no additional validation templates

3. improve the output by integrating semantic annotations, esp. PropBank

content
-------
RRG1997.*.xml
TIGER edition of the syntax examples of
Robert D. Van Valin and Randy J. Lapolla (1997), Syntax. Structure, meaning and function. Cambridge University Press, New York.
Note that these are not annotated, but have been converted automatically using (manually corrected) output of the Stanford parser

EWT.*.xml
TIGER edition of RRG parses derived from UD + PropBank (EWT corpus)
yet to come

history
-------
- 2018-07-08 v.012 (RRG1997, RRG template validation ok except for treatment of "have to" as core cosubordination) -- CC
- 2018-07-04 v.011 (RRG1997, structural validation) -- CC
- 2018-07-03 v.01 (RRG1997, all plausible, not validated, yet) -- CC
- 2018-05-21 repository created -- CC 

contributors
------------
CC - chiarcos@informatik.uni-frankfurt.de