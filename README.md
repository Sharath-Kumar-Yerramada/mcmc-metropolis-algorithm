# MCMC Metropolis Algorithm

## Overview
Implementation and analysis of the Metropolis algorithm based on
Chapter 4 of *MCMC from Scratch* (Hanada & Matsuura, Springer 2022).
Course project for Advanced Statistical Methods I, BSDS (Semester IV),
Indian Statistical Institute Bangalore (May 2026). Group 11.

## What's in this repo
- `Metropolis_codes.R` — all R simulation code
- `Metropolis_Algorithm_Report.pdf` — full project report (24 pages)
- `Metropolis_Algorithm_Presentation.pdf` — slide deck (29 slides)

## Key Results
- Verified histogram convergence for K = 10², 10³, 10⁵, 10⁷, 10⁸ samples
  against the standard Gaussian
- Extended the algorithm to the **Exponential distribution** (original
  contribution — not in the textbook)
- Demonstrated burn-in, autocorrelation (τ ≈ 20 for Gaussian, τ ≈ 100
  for Exponential), and Jackknife error estimation
- Showed the effect of step size c on acceptance rate and convergence;
  optimal range is 30%–80% acceptance
- Proved correctness via Detailed Balance

## Topics Covered
- Metropolis accept-reject algorithm
- Why the partition function Z cancels
- Burn-in / thermalization
- Autocorrelation and the Jackknife method
- Step size tuning
- Box-Muller as a special case of MCMC

## Tools
R

## References
- Hanada & Matsuura, *MCMC from Scratch*, Springer Nature, 2022
- Metropolis et al., *Journal of Chemical Physics*, 21(6), 1953
