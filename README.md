# RG notebook for *Surface topological quantum criticality II*

This repository preserves the Mathematica notebook used for numerical and symbolic checks of selected renormalization-group (RG) equations discussed in:

> Saran Vijayan and Fei Zhou, “Surface topological quantum criticality II: Conformal manifolds, isolated fixed points, and entanglement,” *Physical Review B* **113**, 045134 (2026). https://doi.org/10.1103/z7zr-577m

The notebook is a compact, author-provided computational record. It is not a complete reproduction package for every result in the paper.

## Contents

- [`notebooks/codes_diffeq_solv.nb`](notebooks/codes_diffeq_solv.nb) — original notebook.
- [`docs/SCOPE.md`](docs/SCOPE.md) — inspected scope, limitations, and preservation notes.
- [`CITATION.cff`](CITATION.cff) — citation metadata for the paper associated with this code.
- [`.gitignore`](.gitignore) — common Mathematica-generated and operating-system files.

## Requirements

The notebook identifies itself as created with Wolfram Mathematica 13.1. Use Mathematica 13.1 or a later version for the closest compatibility. It relies on standard built-in functions including `StreamPlot`, `Manipulate`, `Solve`, `D`, `Eigenvalues`, and `Series`; no external packages are declared in the notebook.

A licensed Wolfram Mathematica installation may be required to evaluate the notebook. Wolfram Player can display some saved notebook content, but it does not provide the full evaluation workflow.

## Open and run

1. Download or clone this repository.
2. Open `notebooks/codes_diffeq_solv.nb` in Mathematica.
3. The file contains saved output as well as input cells. To reproduce calculations, evaluate cells in order from the beginning (select **Evaluation → Evaluate Notebook**), or evaluate individual cells in sequence.
4. Interactive `Manipulate` output can be explored in Mathematica. If a saved output appears stale or a dynamic control does not initialize, evaluate its input cell again.

The notebook contains large cached plot output, so opening the file may take a short while. Saved output is part of the preserved original file; regenerating it can yield rendering differences between Mathematica versions.

## What the notebook evaluates

The notebook develops selected finite- and large-\(N_c\) RG calculations described in the paper. It includes:

- two-coupling beta functions for the notebook's `N = 2` case and stream plots of their flow in the `(g1,g2)` plane, including a plot at `epsilon = 0.95`, `Nc = 80`;
- algebraic fixed-point conditions and reductions of the flow in polar-coordinate special directions;
- linear stability matrices built from derivatives of the beta functions and their eigenvalues at selected fixed points;
- series expansions in small `epsilon` and large `Nc` for selected fixed-point/eigenvalue expressions;
- three-coupling (`N = 3`) beta functions, selected fixed-point cases, stability analyses, and discussion of infrared stability.

The notebook should be read as a collection of selected symbolic manipulations and visualizations. In particular, a stream plot is a visualization of the stated beta functions over the plotted range; it is not by itself a numerical integration of trajectories over arbitrary scales.

## Scope and limitations

The notebook does not, by itself, reproduce all analytical arguments, field-theory derivations, or conclusions of the paper. It does not implement a general-purpose RG solver, scan the full parameter space, establish the full conformal-manifold structure, calculate entanglement entropy, or reproduce every figure and result in the article. Its calculations are restricted to the expressions, parameter choices, expansions, and fixed-point cases explicitly present in the notebook. See [`docs/SCOPE.md`](docs/SCOPE.md) for details.

No scientific code has been refactored or silently corrected in this package. The notebook carries forward its original code and saved outputs; apparent inconsistencies or version-sensitive outputs should be checked against the paper and the relevant input cells before drawing conclusions.

## Connection to the paper and citation

Use the peer-reviewed paper as the source of truth for scientific definitions, derivations, interpretation, and claims. The notebook is supporting computational material for selected RG equations and plots, not a substitute for the article. Cite the paper as listed in [`CITATION.cff`](CITATION.cff) and in the block above. Cite this repository separately if you use or redistribute its notebook, once a repository URL and release are assigned.

## Copyright and reuse

No software license is included. The attached paper states © 2026 American Physical Society, and the notebook's redistribution/license status is not specified by the materials inspected. A license should be added only after the relevant rights holder confirms that the notebook can be licensed. Public availability on GitHub alone does not grant permission to reuse or redistribute the contents.
