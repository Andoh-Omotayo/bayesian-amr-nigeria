Bayesian Hierarchical Modeling of Antimicrobial Resistance in Nigeria
Overview

This project applies Bayesian hierarchical logistic regression using PyMC to analyze antimicrobial resistance (AMR) patterns for Ciprofloxacin.

The goal is to estimate the probability of resistance while accounting for:

Multidrug resistance (MDR)

Gene detection status

Specimen-level variation

Age-group variation

This approach provides full uncertainty quantification through posterior distributions using Markov Chain Monte Carlo (MCMC) sampling.

Why Bayesian?

Traditional logistic regression gives single-point estimates.

Bayesian modeling provides:

Probability distributions for each parameter

Credible intervals (HDI)

Full uncertainty quantification

Better modeling of hierarchical biological structure

This is critical in AMR research where uncertainty directly affects treatment policy decisions.

Model Structure

Outcome:

Ciprofloxacin resistance (Binary)

Fixed effects:

MDR status

Gene detection

Random effects:

Specimen group

Age group

Link function:

Logistic (sigmoid)

Inference method:

No-U-Turn Sampler (NUTS)

Key Results

MDR strongly increases probability of resistance.

Gene presence shows weaker but positive association.

Variability exists across specimen types and age groups.

All chains converged (R-hat ≈ 1.00).

Tools Used

Python

PyMC

ArviZ

NumPy

Pandas

Author

Omotayo Andoh
Statistics | Bayesian Modeling | AMR Research
