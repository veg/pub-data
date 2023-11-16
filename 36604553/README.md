> **Detecting macroevolutionary genotype–phenotype associations using error-corrected rates of protein convergence**
> 
> Kenji Fukushima & David D. Pollock 
>  
> _Nature Ecology & Evolution volume 7, pages 155–170 (2023)_



| Attribute      | Value | 
| :---        |    :----   | 
| Number of MSA      | 13       | 
| MSA Format	      | `FASTA` | 
| Stored as	      | Individual alignments store as `.gz` files in `msa`    | 
| Aligners used     | See below      | 
| Filtering strategy     | <span style = "font-family: monospace">Retrieved coding sequences were formatted into in-frame sequences using the ‘pad’ function of CDSKIT v0.9.1 (https://github.com/kfuku52/cdskit). Stop codons and ambiguous codons were replaced with gaps with the ‘mask’ function of CDSKIT. Amino acid sequences from translated coding sequences were aligned using MAFFT v7.455 with the --auto option75, trimmed with ClipKIT v0.1.2 with default parameters and reverse-translated with the ‘backtrim’ function of CDSKIT. Gappy codon sites were excluded with the ‘hammer’ function of CDSKIT.</span>       |
| Tree	      | Yes, annotated tree (HyPhy style, {}) included in the `tree` directory  | 
| Sequences/MSA      | Varied       | 
| Codons/MSA      | TBD       | 
| Tree length/MSA      | TBD       | 
| Taxonomic range      | Varied       | 
| Selection analyses run      | Custom models for convergent evolution detection    |

Note: the `filtered` directory contains .FASTA (.gz) alignments (+trees) masked using `BUSTED-E` in `HyPhy v2.5.58`.

Abstract
--------

On macroevolutionary timescales, extensive mutations and phylogenetic uncertainty mask the signals of genotype–phenotype associations underlying convergent evolution. To overcome this problem, we extended the widely used framework of non-synonymous to synonymous substitution rate ratios and developed the novel metric ωC, which measures the error-corrected convergence rate of protein evolution. While ωC distinguishes natural selection from genetic noise and phylogenetic errors in simulation and real examples, its accuracy allows an exploratory genome-wide search of adaptive molecular convergence without phenotypic hypothesis or candidate genes. Using gene expression data, we explored over 20 million branch combinations in vertebrate genes and identified the joint convergence of expression patterns and protein sequences with amino acid substitutions in functionally important sites, providing hypotheses on undiscovered phenotypes. We further extended our method with a heuristic algorithm to detect highly repetitive convergence among computationally non-trivial higher-order phylogenetic combinations. Our approach allows bidirectional searches for genotype–phenotype associations, even in lineages that diverged for hundreds of millions of years.