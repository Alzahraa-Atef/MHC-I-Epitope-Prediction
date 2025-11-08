Overview

This project predicts MHC-I binding epitopes from a protein sequence using BioPython and MHCflurry.
It aims to identify potential antigenic peptides that could play a role in vaccine development and immunotherapy.

 Objectives

Retrieve a protein sequence (H1N1 Hemagglutinin) from NCBI.

Generate overlapping 9-mer peptides.

Predict peptide–MHC-I binding affinities using machine learning models (MHCflurry).

Identify the top-binding epitopes with lowest predicted IC50 values.

Visualize predicted affinity scores along the protein sequence.

 Tools & Libraries

BioPython – sequence retrieval and manipulation

MHCflurry – MHC-I binding affinity prediction

Pandas – data handling

Matplotlib – data visualization

 Workflow

Retrieve the target protein sequence using BioPython’s Entrez module.

Generate all possible 9-mer peptides from the sequence.

Predict binding affinity for selected alleles:

HLA-A*02:01

HLA-B*07:02

Sort results by predicted IC50 values.

Extract the top 10 epitopes per allele.

Visualize the average IC50 values along the sequence.
