# Notebook scope and preservation notes

## File inspection

The packaged notebook is the original `codes_diffeq_solv.nb` supplied with the request. Its file content was copied unchanged into `notebooks/`; no input cells, saved outputs, or notebook metadata were edited. The source identifies Wolfram Mathematica 13.1. The original file includes extensive cached graphics and output.

## Structure and observed calculations

The notebook has six top-level sections:

1. **RG for N = 2** — defines the two-component large-`Nc` beta functions, displays a flow stream plot (with a stated example `epsilon = 0.95`, `Nc = 80`), and includes an interactive flow plot.
2. **Fixed point solutions for N = 2** — solves selected fixed-point conditions and obtains perturbative expressions.
3. **In polar coordinates** — rewrites/reduces selected flows along special angular directions and solves the resulting one-variable fixed-point conditions.
4. **Stability of fixed points** — differentiates the two-component beta functions to build a Jacobian/stability matrix and evaluates eigenvalues at selected fixed points, including series in `epsilon` and `1/Nc`.
5. **Fixed points and their stability for N = 3.** — defines a three-component beta-function system and examines selected fixed-point configurations and associated linear stability/eigenvalue expansions.
6. **IR stability** — collects selected three-component stability cases and discusses infrared stability.

These descriptions report the operations present in the notebook. They do not independently validate the mathematical derivation or every saved result.

## Boundaries

- The notebook does not contain a general numerical ODE integration workflow such as `NDSolve` or `NIntegrate`; its `StreamPlot` cells visualize vector fields, not computed time-dependent trajectories.
- It examines specific cases and expansions rather than conducting an exhaustive parameter-space survey.
- The notebook does not calculate entanglement entropy or independently demonstrate all claims in the associated paper.
- The explanatory text and definitions in the paper govern interpretation. For the full scientific context, see [the published article](https://doi.org/10.1103/z7zr-577m).
- Saved output may be version- and front-end-dependent. Re-evaluation in a different Mathematica release may alter graphical appearance or dynamic behavior.

## Packaging choices

The paper PDF was not included: it is copyright © 2026 American Physical Society, and this repository can link to the DOI instead. No `LICENSE` file was added because the supplied materials do not establish permission to license the notebook. Before adding a software license, obtain confirmation from the notebook's rights holder; separately verify any rights needed for the desired reuse.
