# RNA Binding Protein Specific RNA Dinucleotide Conformers

## Summary
- We have utilized the non-redundant protein-RNA docking benchmark version 3.0 (PRDBv3.0), comprising 288 protein-RNA complexes from PDB with ≤35% sequence identity.  
- Analyzed 7,607 dinucleotides from these protein-RNA complexes using twelve geometric parameters to study RNA conformational states.  
- Classified dinucleotides by interface location: 3,912 (52.42%) at interface and 3,695 (47.58%) non-interface.  
- Also analyzed 15,549 dinucleotides from 145 non-redundant RNA-only structures to provide a baseline for RNA geometric parameters.  
- Applied Density-Based Spatial Clustering of Applications with Noise (DBSCAN) on backbone and side chain torsion angles to identify 29 unique RNA dinucleotide conformer clusters.

## Cluster and Parameter Description
1. Cluster: DBSCAN-derived clusters representing unique dinucleotide conformations.  
2. PDB ID: Source complex identifier from Protein Data Bank.  
3. Chain: Chain containing the cluster representative.  
4. NtC: Dinucleotide conformer type (new conformers highlighted).  
5-20. Various torsion angles (δ, ε, ζ, α, β, γ, χ) for ith and (i+1)th nucleotides, base plane torsion (μ), Sugar Pucker, Glycosidic Bond rotation, secondary structure (SS), and interface status.

## Transformed Confal Score (scaled 0–100)
\[
\text{Confal Score} = \max\left(0, 100 - \sum_{i=1}^{n} \frac{|\theta_i - \mu_i|}{\sigma_i^2} \right)
\]
- θᵢ: Observed torsion angle (0°–360°)  
- μᵢ: Cluster mean torsion angle (0°–360°)  
- σᵢ: Standard deviation in the reference conformer class  
- n: Number of torsion angles considered  

## Keywords
protein-RNA recognition, torsion angle, RNA dinucleotide conformation, RNA conformational landscape, RNA conformers library.

## Citation
Shri Kant, Savan Masipeddi, and Ranjit Prasad Bahadur. Deciphering conformational preferences of RNA in protein-RNA recognition.
