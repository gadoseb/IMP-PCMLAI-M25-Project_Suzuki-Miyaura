# IMP-PCMLAI-M25-Project_Suzuki-Miyaura

Suzuki-Miyaura coupling is a popular and widely used chemical reaction that allows for the formation of carbon-carbon (C-C) bonds between aryl or vinyl halides and boronic acids or boronate esters. This reaction is a type of cross-coupling reaction, which involves the merging of two different organic molecules to create a new compound with a C-C bond (Scheme 1).

![Suzuki_coupling_scheme](https://user-images.githubusercontent.com/114429348/232866281-5a99fd52-f434-4579-b5eb-869336c7e120.jpg)

The Suzuki-Miyaura coupling reaction was first reported by Akira Suzuki and Norio Miyaura in the 1970s and has since become a fundamental tool in organic synthesis, particularly in the field of medicinal chemistry and materials science. It is known for its mild reaction conditions, high functional group tolerance, and broad substrate scope, making it applicable to a wide range of organic molecules.
The reaction typically involves the use of a palladium catalyst, along with a base and a source of boron, such as a boronic acid or boronate ester. The reaction proceeds through a transmetalation step, where the palladium catalyst facilitates the transfer of an aryl or vinyl group from the boron source to the halide substrate, forming a C-C bond in the process.
The Suzuki-Miyaura coupling reaction has been used in the synthesis of numerous complex organic molecules, including natural products, pharmaceuticals, and functional materials. It has enabled chemists to efficiently create C-C bonds in a controlled and selective manner, making it a valuable tool in modern organic chemistry.

# Notebook Structure
1. Dataset Preparation and Exploration
2. PCA and Clustering based on Chemical Similarity
3. Suzuki-Miyaura Coupling Reaction Prediction - Regression Approach
4. Conclusions

For the details about the packages used in this model, please refer to the beginning of each section of the notebook.

# Files in the repository 

- Suzuki-Miyaura_Capstone Project.ipynb = Jupyter Notebook
- Suzuki_coupling_scheme.jpg = Reaction scheme of the investigated Suzuki-Miyaura coupling
- Literature Data_colon_delimited.csv = Literature data dataset
- dataset_withtestset.csv = Experimental data dataset

# Dataset

The database was built from various literature data (which can be tracked in the `article` column) with the following instances:

- **solvent_names**: a field to store the names of the solvents used in a chemical reaction.
- **solvent_class**: a field to store the class of the solvents used in a chemical reaction, such as polar or nonpolar.
- **base_names**: a field to store the names of the bases used in a chemical reaction.
- **base_class**: a field to store the class of the bases used in a chemical reaction, such as strong or weak.
- **temperature**: a field to store the temperature at which the chemical reaction was performed in $^\circ$ C.
- **ligand**: a field to store the type of ligand used in the chemical reaction.
- **Pd source**: a field to store the source of Pd catalyst used in the chemical reaction.
- **yield**: a field to store the yield of the chemical reaction.
- **article**: a field to store the article/literature reference where the reaction was reported.
- **reaction_smiles**: a field to store the SMILES notation for the chemical reaction.
- **boronate**: a field to store the SMILES notation for the boronate compound used in the chemical reaction.
- **bromide**: a field to store the SMILES notation for the bromide compund used in the chemical reaction.
- **condition_string**: a field to store a string representing the reaction conditions (solvent, base and ligand).

This type of database is used to store and organize information about a set of chemical reactions, such as the conditions under which the reactions were performed, the reactants and catalysts used, and the yields of the reactions. 

SMILES (Simplified Molecular Input Line Entry System) is a notation for describing the structure of a molecule using a simple ASCII string. Each atom in a SMILES string is represented by a symbol, such as C for carbon, N for nitrogen, and O for oxygen, and the bonds between atoms are represented by characters such as "-" for single bonds, "=" for double bonds, and "#" for triple bonds. This notation can be read by the `rdkit` package.

The original database can be found in the `open_reaction_database_files` folder of the following repository.
N. H. Angello et al., Closed-loop optimization of general conditions for heteroaryl Suzuki coupling, version 0.1.2, Zenodo (2022); https://doi.org/10.5281/zenodo.7099435
