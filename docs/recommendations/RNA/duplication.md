# duplication

## Definition

Duplication: a sequence change where, compared to a reference sequence, a copy of one or more nucleotides are inserted <b>directly 3'</b> of the original copy of that sequence.

## Description

Format:   **"prefix""position(s)\_duplicated""dup"**,  e.g. r.123\_345dup

**"prefix"**  =  reference sequence used  =  r.<br>
**"position(s)\_duplicated"**  =  position nucleotide or range of nucleotides duplicated  =  123\_345<br>
**"dup"**  =  type of change is a duplication  =  dup

## Notes

* all variants **should be** described at the DNA level, descriptions at the RNA and/or protein level may be given in addition
* **prefix** reference sequences accepted are r. (coding and non-coding RNA).
* “positions_duplicated” should contain two different positions, e.g. 123_126 not 123_123.
* the “positions_duplicated” should be listed from 5’ to 3’, e.g. 123_126 not 126_123.
* by definition, duplication may only be used when the additional copy is **directly 3’-flanking** of the original copy (a “tandem duplication”).
    * when a variant can be described as a duplication it **must** be desribed as a duplication and not as e.g. an insertion (see [_Prioritization_](/recommendations/general/))
    * when there is no evidence that the extra copy of a sequence detected is in tandem (directly 3'-flanking) the original copy, the change can not be described as a duplication, it should be described as **an insertion** ([_see Insertion_](/recommendations/RNA/variant/insertion/)).
    * **inverted duplications** are described as insertion (r.234\_235ins123\_234inv), not as a duplication ([_see Inversion_](/recommendations/RNA/variant/inversion))
* for all descriptions the **most 3' position** possible of the reference sequence is arbitrarily assigned to have been changed (**3'rule**)
    * the 3'rule also applies for changes in single residue stretches and tandem repeats
    * **NOTE:** the exception to the 3'rule for duplications around exon/exon junctions  [_see Duplications_](/recommendations/DNA/variant/duplication/) does not apply when describing variants based on a RNA reference sequence
## Examples

* r.7dup (one nucleotide): the duplication of a "u" at position r.7 in the sequence ..acuuacugcc.. to ..acuuacu**<font color="red">u</font>**gcc..: **NOTE**: it is **not** allowed to describe the variant as r.6\_7insu ([_see prioritisation_](/recommendations/general/))
* r.6\_8dup (several nucleotides): a duplication from position r.6 to r.8 in the sequence ..acaauugcc.. to ..acaauugc**<font color="red">ugc</font>**c..: **NOTE**: it is allowed to describe the variant as g.6_8dupugc
## Discussion

!!! note "Why do we not describe a duplication as an insertion?"

    Although duplications are basically a special type of insertion, there are several reasons why the recommendation is to describe duplications separately;<ul><li>the description is simple and shorter,</li><li>it is clear and prevents confusion regarding the position when an insertion is incorrectly reported like "22insg".</li></ul>

!!! note "How should I describe the change "aucg<b>aucgaucgauc</b>aggguccc" to "aucg<b>aucgaucgauc</b>a<b>aucgaucgauc</b>ggguccc"?  The fact that the inserted sequence (aucgaucgauc) is present in the original sequence suggests it derives from a duplicative event."

    The variant should be described as an insertion; r.17_18ins5_16. A description using "dup" is not correct since, by definition, a duplication should be <b>directly 3'-flanking of the original copy</b> (in tandem). Note that the description given still makes it clear that the sequence inserted between r.17 and r.18 is probably derived from nearby, i.e. position r.5 to r.16, and thus likely derived from a duplicative event.
---