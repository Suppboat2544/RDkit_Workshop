# RDkit_Workshop
RDKit Workshop: Fingerprints, Descriptors, and Coding Limitations
Author: Supaporn Klabklaydee (Fujii Laboratory)

Overview
This workshop provides hands-on experience with RDKit, a popular cheminformatics library in Python. The tutorial focuses on generating different types of molecular fingerprints, calculating various molecular descriptors, and understanding common limitations and pitfalls when coding with RDKit.

Learning Objectives
By the end of this workshop, you will be able to:

Set up and use RDKit in your Python environment

Generate various types of molecular fingerprints

Calculate molecular descriptors

Compare molecular similarity using different fingerprint methods

Understand the limitations and best practices when working with RDKit

Prerequisites
Basic knowledge of Python programming

Understanding of chemistry concepts (molecular structures, SMILES notation)

Jupyter Notebook environment

Installation
Before starting the workshop, ensure RDKit is installed:

bash
pip install rdkit
Workshop Content
1. Environment Setup
RDKit installation and verification

Importing necessary modules and libraries

2. Fingerprint Generation Functions
The workshop covers multiple fingerprint algorithms:

Morgan Fingerprints (Circular Fingerprints)
Standard Morgan fingerprints (equivalent to ECFP)

Feature-based Morgan fingerprints (equivalent to FCFP)

Custom atom invariants for topology comparison

Supported Fingerprint Types
Feature Morgan: Variation of Morgan fingerprint

RDKit descriptors: Built-in molecular descriptors

Atom pairs: Topological fingerprints

Topological torsions: Structural fingerprints

3. Fingerprint Operations
Generating bit vectors and count vectors

Creating sparse fingerprints

Calculating molecular similarity using Tanimoto and Dice coefficients

Comparing different fingerprint methods

4. Practical Examples
Working with molecular structures (e.g., ibuprofen, toluene)

SMILES string processing

Similarity calculations between different molecules

Custom fingerprint generation with user-defined parameters

Key Functions Covered
python
# Basic fingerprint generation
fpgen.GetFingerprint(mol)           # Returns bit vector
fpgen.GetCountFingerprint(mol)      # Returns count vector  
fpgen.GetSparseFingerprint(mol)     # Returns sparse bit vector
fpgen.GetSparseCountFingerprint(mol) # Returns sparse count vector

# Similarity calculations
DataStructs.TanimotoSimilarity(fp1, fp2)
DataStructs.DiceSimilarity(fp1, fp2)
Usage
Clone or download the RDKIT_Workshop_BOAT-1.ipynb file

Open in Jupyter Notebook or JupyterLab

Follow the step-by-step instructions in each cell

Execute cells sequentially to understand each concept

Experiment with the provided examples and try your own molecules

Workshop Structure
Setup Section: Environment preparation and imports

Theory Section: Understanding fingerprint concepts

Hands-on Section: Practical coding exercises

Examples Section: Real-world molecular comparisons

Limitations Section: Common pitfalls and best practices

Additional Resources
RDKit Documentation

RDKit GitHub repository

Cheminformatics tutorials and examples

Notes
The workshop uses interactive examples with molecular structures

Code examples include both basic and advanced fingerprint generation techniques

Emphasis on understanding when to use different fingerprint types

Discussion of computational limitations and performance considerations

Getting Help
If you encounter issues:

Check that RDKit is properly installed

Verify Python environment compatibility

Refer to the RDKit documentation for detailed API information

Contact the Fujii laboratory for workshop-specific questions

This workshop is designed for educational purposes and provides a comprehensive introduction to molecular fingerprinting using RDKit.
