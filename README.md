# Bio Snippets
Some helpful bits of code 

## Sonya's psi-BLAST tips for CapRel1455
- psiblast more sensitive than blast, can search against RefSeq genomes
- search 1:
  - WP_049001067.1 (full length)
  - max target sequence: 5000
  - evalue: < 1e-100
  - Query coverage: >= 95% (sequences that fully cover toxin and antitoxin)
  - RESULT: 89 high-confidence sequences
- search 2:
  - evalue: < 1e-10
  - query coverage: >= 85%
  - RESULTS: 1455 unique sequences (>6000 sequences)
