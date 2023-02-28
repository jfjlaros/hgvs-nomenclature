# duplication

## Definition

Duplication: a sequence change between the translation initiation (start) and termination (stop) codon where, compared to a reference sequence, a copy of one or more amino acids are inserted <b>directly C-terminal</b> of the original copy of that sequence.

## Description

Format:  **"prefix""amino\_acid(s)+position(s)\_duplicated""dup"**,  e.g. p.(Cys76\_Glu79dup)

**"prefix"**  =  reference sequence used  =  p.<br>
**"amino_acid(s)+position(s)\_duplicated"**  =  amino acid with position or range (first amino acid with position to last amino acid with position) duplicated  =  Cys76\_Glu79<br>
**"dup"**  =  type of change is a duplication =  dup

## Notes

* all variants **should be** described at the DNA level, descriptions at the RNA and/or protein level may be given in addition
* **prefix** reference sequence accepted is "p." (protein).
* predicted consequences, i.e. without experimental evidence (no RNA or protein sequence analysed), should be given in parentheses, e.g. p.(Arg727\_Ser783dup).
* the "amino\_acids+positions\_duplicated" should contain **two different** positions, i.e. Cys76\_Glu79, not Cys76\_Cys76.
    * the "positions\_duplicated" should be listed from **5' to 3'**, i.e. Cys76\_Glu79, not Glu79\_Cys76.
* by definition, duplication may only be used when the additional copy is **directly C-terminal** of the original copy (a "tandem duplication").
    * when the extra copy is, at the protein level, not in tandem (directly C-terminal), the change should be described as **insertion** ([_see Insertion_](/recommendations/protein/variant/insertion/)).
    * duplications extending the amino acid sequence at the C-terminal end with one or more amino acids are described as [_Extension_](/recommendations/protein/variant/extension)
* for all descriptions the **most C-terminal position** possible of the reference sequence is arbitrarily assigned to have been changed (**3'rule**)
* duplications at the DNA or RNA level, **starting N-terminal of and including** the translation termination (stop) codon usually have no (predicted) effect on the protein level.
* duplications at DNA or RNA level
    * which introduce an **immediate** translation termination (stop) codon at the protein level are described as a nonsense variant.
    * **encoding a translation stop codon** in the duplicated sequence are at the protein level described as an insertion of this sequence, not as a deletion-insertion removing the entire C-terminal amino acid sequence.
    * encoding an open reading frame which **after** the duplicated sequence shift to another reading frame are described as a frame shift.
## Examples

* one amino acid
    * NP\_003997.2:p.Val7dup: a duplication of amino acid Val7 in the reference sequence NP\_003997.2
    * NP\_003997.2:p.(Val7dup): the **predicted** consequence at the protein level is a duplication of amino acid Val7 in the reference sequence NP\_003997.2
    * NP\_003997.2:p.Trp4dup: a duplication of amino acid Trp4 in the sequence MetLeuTrpTrpGlu to MetLeuTrpTrp**<font color="red">Trp</font>**Glu: **NOTE:** for duplications in single amino acid stretches or tandem repeats, the most C-terminal residue is arbitrarily assigned to have been duplicated    
* several amino acids
    * NP\_003997.2:p.Lys23\_Val25dup: a duplication of amino acids Lys23 to Val25 in reference sequence NP\_003997.2
    * NP\_003997.2:p.(Pro458\_Gly460dup): a duplication of amino acids Pro458-Pro459-Gly460 in reference sequence NP\_003997.2: **NOTE:** the underlying DNA variant (LRG\_232t1:c.1365\_1373dup) affects amino acids Pro455-Pro456-Gly457 but the 3'rule needs to be applied
* one or more exons
    * NP\_003997.2:p.(His321\_Glu383dup): the predicted consequences of a duplication of exon 10 of the DMD gene, duplicating amino acids His321 to Glu383 in reference sequence NP\_003997.2
    * NP\_003997.2:p.(Asp90\_Val120dup): the predicted consequences of a duplication of exon 5 of the DMD gene, duplicating amino acids Asp90 to Val120 in reference sequence NP\_003997.2: **NOTE:** since the 3'rule needs to be applied the description p.(Val89\_Gln119dup) is not correct
    * NP\_003997.2:p.(Asn444Lysfs\*15): the predicted consequences of a duplication of exons 10 to 11 of the DMD gene, creating a frame shift starting at amino acid Asn444, replacing it with Lys and terminating after fifteen codons.
    * NP\_003997.2:p.?: the predicted consequences of a duplication of exons 1 to 2 of the DMD gene: **NOTE:** since the duplication adds a second promoter/exons 1 to a normal copy of the gene, a reliable prediction of the consequences can not be made. The duplication may have no consequences, it may give a duplication of exon 2 in the transcript, it might produce both transcripts, etc.
    * NP\_003997.2:p.?: the predicted consequences of a duplication of exons 74 to 79 of the DMD gene: **NOTE:** since the duplication adds a second last exon (exon 79) to a normal copy of the gene, a reliable prediction of the consequences can not be made. The duplication may have no consequences, it may give a duplication of exons 74 to 78 in the transcript, it might produce both transcripts, etc.
* NP\_003997.1:p.Val7=/dup: a mosaic case where at amino acid position 7 besides the normal amino acid (a Val, described as “Val7=”) also protein is found containing a duplication (Val7dup): **NOTE:** for the predicted consequences of a variant the description is NP\_003997.1:p.(Val7=/dup)
## Discussion

!!! note "Why do we not describe a duplication as an insertion?"

    Although duplications are basically a special type of insertion, there are several reasons why the recommendation is to describe duplications differently;<ul><li>the description is simple and shorter,</li><li>it is clear and prevents confusion regarding the position when an insertion is incorrectly reported like "Ala22insGly".</li></ul>

!!! note "How should I describe the change "MetArgThr<b>GlySerSer</b>HisGlnTrpPhe" to "MetArgThr<b>GlySerSer</b>His<b>GlySerSer</b>GlnTrpPhe"?  The fact that the inserted sequence (GlySerSer) is present in the original sequence suggests it derives from a duplicative event."

    The variant should be described as an insertion; p.His7_Gln8insGly4_Ser6. A description using "dup" is not correct since, by definition, a duplication should be <b>directly 3'-flanking of the original copy</b> (in tandem). Note that the description given still makes it clear that the sequence inserted between p.His7 and pGln8 is probably derived from nearby, i.e. position p.Gly4 to p.Ser6, and thus likely derived from a duplicative event.

!!! note "What do you mean with "variants should be described on the protein level and not incorporate knowledge regarding the change at the DNA-level"?"

    It means that protein variant descriptions should be derived from comparing the variant protein sequence with the reference protein sequence. Knowledge on the underlying change at the DNA level should not be used. E.g. when MetTrpSerSerSerHisAsp.. changes to MetTrpSerSerSer<b><font color="red">Ser</font></b>HisAsp.. this is described as p.Ser5dup. The information that at the DNA level the change is ..ATGTGGTCCAGTTCCCACGAT.. to ..ATGTGGTCCAGT<b><font color="red">AGT</font></b>TCCCACGAT.., so the codon for Ser4 is duplicated, is not used; the description p.Ser4dup is not correct. 