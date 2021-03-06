Extensions
==========

Some SMARTS implementations include extensions and differences to atom and bond primitives. This section documents these differences.

OpenEye
-------

`Publically documented <a href="http://docs.eyesopen.com/toolkits/oechem/cplusplus/SMARTS.html">`

+--------------+-----------------------+
| R <NUMBER>   | Ring bond count       |
+--------------+-----------------------+
| ^ <NUMBER>   | Atomic hybridisation  |
+--------------+-----------------------+

CACTVS
------

`Publically documented <a href="http://85.214.192.197/Documentation/html/tcl_reference-44.htm#pgfId-624130">`

+--------------------------------------+----------------------------------------------------------------+
| <PRIMITIVE> { <NUMBER> - <NUMBER>? } | Attribute range (e.g. H{0-2} = H0,H1,H2)                       |
+--------------------------------------+----------------------------------------------------------------+
| <PRIMITIVE> [ <NUMBER> + ]           | Attribute enumeration (e.g. [H[012]] = H0,H1,H2)               |
+--------------------------------------+----------------------------------------------------------------+
| [~\w+?]                              | Explicit superatoms                                            |
+--------------------------------------+----------------------------------------------------------------+
| n/a                                  | Implicit superatoms                                            |
+--------------------------------------+----------------------------------------------------------------+
| HA                                   | Hydrogen acceptor                                              |
+--------------------------------------+----------------------------------------------------------------+
| HD                                   | Hydrogen donor                                                 |
+--------------------------------------+----------------------------------------------------------------+
| D                                    | Deuterium                                                      |
+--------------------------------------+----------------------------------------------------------------+
| T                                    | Tritium                                                        |
+--------------------------------------+----------------------------------------------------------------+
| a <NUMBER>                           | Aromatic ring membership                                       |
+--------------------------------------+----------------------------------------------------------------+
| e <NUMBER>                           | Pi electrons in ring                                           |
+--------------------------------------+----------------------------------------------------------------+
| X                                    | Hetroatom                                                      |
+--------------------------------------+----------------------------------------------------------------+
| #X                                   | Hetroatom                                                      |
+--------------------------------------+----------------------------------------------------------------+
| ?                                    | Wildcard                                                       |
+--------------------------------------+----------------------------------------------------------------+
| i <NUMBER> ?                         | Insaturation                                                   |
+--------------------------------------+----------------------------------------------------------------+
| G <NUMBER> ?                         | Insaturation                                                   |
+--------------------------------------+----------------------------------------------------------------+
| z <NUMBER> ?                         | Adjacent hetroatoms                                            |
+--------------------------------------+----------------------------------------------------------------+
| T <NUMBER>                           | Adjacent hetroatoms                                            |
+--------------------------------------+----------------------------------------------------------------+

+--------------------------------------+----------------------------------------------------------------+
| <PRIMITIVE> ! <PRIMITIVE>            | Atoms are not connected                                        |
+--------------------------------------+----------------------------------------------------------------+
| <PRIMITIVE> | <PRIMITIVE>            | Complex bond                                                   |
+--------------------------------------+----------------------------------------------------------------+

+--------------------------------------+----------------------------------------------------------------+
| [$$(<SMARTS>)]                       | Non-overlapping recursive SMARTS                               |
+--------------------------------------+----------------------------------------------------------------+

+--------------------------------------+----------------------------------------------------------------+
| [^<PRIMITIVE>]                       | Exclusion                                                      |
+--------------------------------------+----------------------------------------------------------------+


MOE
---

Retrospectively inferred in AMBIT from `Lee et al. Supplementary Matterial <http://pubs.acs.org/doi/abs/10.1021/ci8001815>`

+--------------+---------------------------------------+
| #X           | Hetroatom                             |
+--------------+---------------------------------------+
| #G <NUMBER>  | Group (e.g. #G16 matches chalcogens)  |
+--------------+---------------------------------------+
| #N           | Electronegative atom                  |
+--------------+---------------------------------------+
| v <NUMBER>   | Non-hydrogen bonded valence           |
+--------------+---------------------------------------+
| i            | Insaturation                          |
+--------------+---------------------------------------+

Jmol
----

http://chemapps.stolaf.edu/jmol/docs/examples-12/Jmol-12.0-quickstart.pdf
r500 and r600 for 5 and 6 member aromatic rings IIRC

ICM
---

http://www.molsoft.com/man/smiles.html


References
----------

http://blueobelisk.shapado.com/questions/list-of-smarts-extensions



