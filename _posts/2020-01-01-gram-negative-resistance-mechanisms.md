---
title: "Gram negative resistance mechansims"
date: 2020-01-01
---



# Notes on Gram negative acquired resistance mechanisms
## Alessandro Gerada
### Introduction
The aim of this brief document is to summarise some general principles that allow the reader to identify acquired resistance mechanisms in Enterobacterales. For the purpose of this document this shall include organisms such as *E. coli*, *Klebsiella* spp., *Proteus* spp, *Enterobacter* spp, etc but importantly it will not extend to the nonfermenters (*Pseudomonas* spp., *Acinetobacter* spp., *Stenotrophomonas maltophilia*). This is not meant to be an exhaustive document - there exist other excellent papers that go into more detail, such as:
* [CMR review on AmpC beta-lactamases](https://cmr.asm.org/content/22/1/161)
* [CMR review on ESBLs](https://cmr.asm.org/content/18/4/657#sec-53)
* [EUCAST Resistance mechanisms](https://www.eucast.org/fileadmin/src/media/PDFs/EUCAST_files/Resistance_mechanisms/EUCAST_detection_of_resistance_mechanisms_170711.pdf)

Some notes on treatment options are also included, although again this is not meant to be an exhaustive list.
### Extended-spectrum beta-lactamases (ESBL)
Knowing the definition of ESBL gets us halfway towards understanding how best to detect them. ESBLs are defined as:
*a group of β-lactamases which share the ability to hydrolyse third-generation cephalosporins and aztreonam yet are inhibited by clavulanic acid.*
Therefore this explains the use of Cefpodoxime as a screening test for ESBLs. The definitive phenotypic test is synergy testing with a beta-lactamase inhibitor. The principle behind these tests is important.
#### Screening tests
A third generation cephalosporin disc is the most sensitive and convenient. Cefpodoxime performs this role best.
#### Genotypic tests
There are some genotypic ESBL tests available. For example, some of the various [Biofire Filmarray](https://www.biofiredx.com/products/the-filmarray-panels/filmarraybcid/) products can detect CTX-M. The main issue is that there are many different types and variations of ESBL (CTX, TEM, SHV, OXA-types), therefore the utility of a CTX-M PCR depends on whether this is the predominant gene in the tested population.
#### Phenotypic tests
These are probably the most useful confirmatory tests for ESBLs.

Enterobacterales that do *not* produce ESBL have a particular MIC or disc zone to third-generation cefalosporins. This is *not* affected by the presence of clavulanic acid.

Enterobacterales that *do* produce ESBL show (as per the original definition) a reduction of MIC (or increase in zone size) when the third-generation cefalosporin is combined with clavulanic acid.
#### Other tests
A chromogenic cefalosporin colorimetric test is available as a screening test, and follows the same principles as the chromogenic cefalosporin test for beta-lactamase detection in *Staph. aureus*.
### AmpC beta-lactamases
The first point to make, and perhaps the most important, is that there are two types of AmpC beta-lactamases that we need to be concerned with:

* Chromosomal AmpC - these can be produced constitutively by certain bacterial species (such as *Enterobacter* spp., *C. freundii*, *M. morganii*, *P. aeruginosa*). These organisms in effect **always** have the ability to produce AmpC beta-lactamase through de-repression. Therefore whenever we isolate these organisms, we should assume that they can produce AmpC beta-lactamases, and should ignore any other results such as Cefoxitin susceptibility.
> An interesting question - does *E. coli* have a chromosomal AmpC?
* Acquired (usually plasmid mediated) AmpC - these have a similar effect to the above, but are acquired by bacterial species that otherwise do *not* have a chromosomal AmpC (organisms such as *Klebsiella* spp.). For these we do need further testing to determine their abscence or presence.

All the points below only apply to acquired AmpC.
#### Screening tests
Cefoxitin is the most useful screening antibiotic for AmpC. However while it is very sensitive, it is not particularly specific, as there are other mechanisms of resistance against this antibiotic (such as porin loss). Therefore, we should also look at Cefotaxime and/or Ceftazidime. We should expect that if there is an acquired AmpC (rather than porin loss against Cefoxitin) that there is resistance to one of these agents as well.

In many laboratories, this is really where the AmpC story ends. Trying to confirm acquired AmpC further is high effort (especially as many isolates also co-produce ESBL) with low clinical yield, so many do not bother.

In summary (where "X" = any result):

| Organism | Cefoxitin | Cefotaxime/Ceftazidime | Interpretation
|----------|-----------|------------------------|----------------
| Has chromosomal AmpC | X | X | AmpC positive
| Does not have chromosomal AmpC | S | X | AmpC negative
| Does not have chromosomal AmpC | R | S | AmpC negative
| Does not have chromosomal AmpC | R | R | AmpC positive

#### Genotypic tests
PCR for different AmpC enzymes is available, but not in common routine use. Look elsewhere if you are curious.

#### Phenotypic tests
For exam purposes, it is worth mentioning that AmpC are inhibited by cloxacillin, giving similar results to the ESBL synergy tests if using cloxacillin instead of clavulanic acid, which is in theory a confirmatory test.

### Carbapenemase-producing Enterobacterales (CPE)
This is a heterogenous group, and impossible to cover completely. Remember also that other mechanisms (such as AmpC de-repression with porin loss) are important causes of carbapenem resistance. It is however possible to learn a few tricks to distinguish between the 5 main classes:

* OXA-48
* KPC
* Metallo-beta-lactamases (MBL):
  * VIM
  * NDM
  * IMP

Fortunately if we group the metallo-beta-lactamases together we only have to deal with 3 groups (in the laboratory and even clinically VIM/NDM/IMP behave very similarly).

#### Screening tests
Ertapenem is the most sensitive antibiotic for CPE screening. Any zone smaller than 25mm in a suspect organism should be investigated further. Meropenem can also be used (better specificity at the cost of sensitivity).

#### Phenotypic tests
Until a few years ago, the Modified Hodge test was used as a phenotypic test for CPE. Thankfully (as this test is a bit tricky to explain) it is no longer recommended, due to poor performance.

Synergy tests can be used to identify CPE, and are quite popular exam questions:
* Synergy with boronic acid - **KPC** (although be aware that this also applies to AmpC)
* Synergy with dipicolinic acid (DPA) or EDTA - **MBL**
* OXA-48 does not exhibit synergy with any agent

#### Genotypic tests
These are by far the most practically useful tests to confirm the presence of CPE. [Cepheid Xpert Carba-R](https://www.cepheid.com/en/tests/Healthcare-Associated-Infections/Xpert-Carba-R) detects the 5 main CPE classes quickly and with good results.

#### Other tests
It is possible to use colorimetric tests and even MALDI-TOF for the detection of CPE. However it is unlikely that these tests would appeal to a laboratory that has genotypic methods available.

Is it possible to summarise ESBL/AmpC/CPEs in one table? Yes, but at what cost?

| Mechanism | Synergy | Antibiotic hints | Beta-lactam treatment options
|-----------|---------|------------------|-----------
| ESBL | Clavulanic acid ( + 3rd gen cefalosporin) | Cefpodoxime R <br> Cefepime R| Meropenem <br> Ertapenem <br> Temocillin <br> Ceftazidime-avibactam <br> Ceftolozane-tazobactam
| Acquired AmpC | Boronic acid or cloxacillin (+ 3rd gen cefalosporin) | Cefoxitin + Ceftazidime/Cefotaxime R <br> Cefepime S | Similar to ESBL
| KPC | Boronic acid (+ carbapenem) | | Meropenem-vaborbactam <br> Ceftazidime-avibactam <br> Imipenem-relebactam <br> Cefiderocol
| OXA-48 | None | High level Temocillin R <br> Ceftazidime S | Ceftazidime-avibactam <br> Ceftazidime <br> Cefiderocol
| MBL | DPA/EDTA (+ carbapenem) | Aztreonam S | Aztreonam-avibactam <br> Aztreonam <br> Cefiderocol


**Important- this table does not apply if there are multiple resistance mechanisms.**

This table does not include non-beta-lactam classes of antibiotics, which can be used depending on susceptibility testing and source of infection. These agents, if sensitive, include:
* quinolones
* aminoglycosides
* polymixins
* tigecycline
* co-trimoxazole
* chloramphenicol

### Conclusion and unanswered questions
There remain many unanswered questions in this field:
* Can we use piperacillin-tazobactam to treat ESBL/AmpC? [MERINO trial suggests not, at least for "definitive" therapy](https://pubmed.ncbi.nlm.nih.gov/30208454/)
* Should we give combination therapy to all patients with invasive CPE infection, even if sensitive to one of the new beta-lactams? (probably, since resistance during treatment can occur with agents such as ceftazidime-avibactam)
* Should we care about colonisation detected on IPC screens in patients who are unwell?

It is also worth reviewing acquired colistin resistance (*mcr* genes) altough this seems to have gone quiet recently - possibly due to the introduction of new Gram-negative antibacterial agents having been released.
