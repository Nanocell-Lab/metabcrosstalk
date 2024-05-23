# Metabcrosstalk
Metabolic Cross Talk between Bacteria and Human

This is a collaboration between the Laboratory of Molecular & Translational Immunology, PI: Estefanía Nova Lamperti, PhD, https://farmacia.udec.cl/estefania-novalamperti, and Cancer Molecular Dynamics Laboratory, PI: Alexis Salas-Burgos, PhD, https://nanocell-lab.github.io.

Universidad de Concepción - Chile

# Methodology
## Human Functional Enrichment Analysis. 
 Two statistical analyzes were performed associated with the genes derived from the proteomics analyses: i) Ingenuity Pathways Analysis (IPA), performed with the tool QIAGEN IPA, ii) Gene Ontology Enrichment Analysis (GOEA) performed with the g-profiler platform, https://biit.cs.ut.ee/gprofiler/gost (Kolberg et al. 2023). The raw data from both analyzes were processed in Python and graphs were developed for interpretation (Van Rossum y Drake 2009). The code is available at https://github.com/Nanocell-Lab/metabcrosstalk.

* src/01ProteomicsHuman.ipynb
* src/02FunctionalEnrichmentA.ipynb

## Bacterial Automatics Glutamate pathway search in Metacyc.
 We automate the identification of genes derived from the proteomics analyzes in the metabolic pathways involved in L-glutamate. A code was developed in python that consists of three steps: i) identification of the genes derived from the proteins identified in the proteomic profiles using the database of HOMD (Escapa et al. 2018), ii) identification of the metabolic pathways in Metacyc (Caspi et al. 2020) associated with a metabolite, and iii) counting of the genes found in each metabolic pathway. The source code is available at https://github.com/Nanocell-Lab/metabcrosstalk.
* src/03ProteomicsBacteria.ipynb
* src/04MetaCyc.ipynb

# Requirements
Bioinfokit
https://pypi.org/project/bioinfokit
Pandas
https://pandas.pydata.org/docs/index.html

## References
* Caspi, Ron, Richard Billington, Ingrid M Keseler, Anamika Kothari, Markus Krummenacker, Peter E Midford, Wai Kit Ong, Suzanne Paley, Pallavi Subhraveti, y Peter D Karp. 2020. «The MetaCyc database of metabolic pathways and enzymes - a 2019 update». Nucleic Acids Research 48 (D1): D445-53. https://doi.org/10.1093/nar/gkz862.
* Escapa, Isabel F., Tsute Chen, Yanmei Huang, Prasad Gajare, Floyd E. Dewhirst, y Katherine P. Lemon. 2018. «New Insights into Human Nostril Microbiome from the Expanded Human Oral Microbiome Database (eHOMD): a Resource for the Microbiome of the Human Aerodigestive Tract». mSystems 3 (6): 10.1128/msystems.00187-18. https://doi.org/10.1128/msystems.00187-18.
* Kolberg, Liis, Uku Raudvere, Ivan Kuzmin, Priit Adler, Jaak Vilo, y Hedi Peterson. 2023. «G:Profiler-Interoperable Web Service for Functional Enrichment Analysis and Gene Identifier Mapping (2023 Update)». Nucleic Acids Research 51 (W1): W207-12. https://doi.org/10.1093/nar/gkad347.
* Van Rossum, Guido, y Fred L. Drake. 2009. Python 3 Reference Manual. Scotts Valley, CA: CreateSpace.

