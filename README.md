# José F. Aguilar Madeira

**Associate Professor (with Habilitation in Mathematics)** · Department of Mathematics, ISEL — Polytechnic Institute of Lisbon

**Integrated Researcher** · IDMEC / LAETA, Instituto Superior Técnico, Universidade de Lisboa

Research in **Optimization and Decision Sciences**: derivative-free optimization, multiobjective optimization, global and local direct-search methods, and applied operations research developed in partnership with industry.

---

## Published Algorithms

| Method | Description | Reference |
| --- | --- | --- |
| **DMS** — Direct MultiSearch | Local multiobjective optimization without derivatives | Custódio, Madeira, Vaz & Vicente, 2011 |
| **GLODS** — Global and Local Optimization using Direct Search | Single-objective global optimization | Custódio & Madeira, *Journal of Global Optimization*, 2015 |
| **MultiGLODS** | Global multiobjective optimization without derivatives | Custódio & Madeira, 2018 |
| **GLODS-SI** — Scale-Invariant variant for engineering design optimization | Companion code: [`GLODS_SI`](https://github.com/aguilarmadeira/GLODS_SI) | Madeira, *Journal of Computational Design and Engineering* (2026), Open Access — DOI [10.1093/jcde/qwag049](https://doi.org/10.1093/jcde/qwag049) |

## Recent theoretical and algorithmic work

A two-part contribution on mixed-variable optimisation, in which the structural and algorithmic components reference one another:

- **Structural foundation** — *Mixed-Variable Optimisation as a Metric Product Space: Transient Categorical Geometry and a Hierarchy of Local Optimality*. Manuscript under review. Preprint: [Zenodo](https://zenodo.org/records/18704776). Companion code: [`mixed-spaces-supplementary`](https://github.com/aguilarmadeira/mixed-spaces-supplementary).
- **Algorithmic instantiation** — *Deterministic Neighborhood Rotation (DNR) for Categorical Variables in Derivative-Free Optimization*. Working paper. Preprint: [Zenodo](https://zenodo.org/records/19257923). Code release planned upon acceptance for publication.


**Companion repositories**

- [`GLODS_SI`](https://github.com/aguilarmadeira/GLODS_SI) — implementation and reproducibility artefacts for GLODS-SI
- [`MOO_Prob_Matlab`](https://github.com/aguilarmadeira/MOO_Prob_Matlab) — multiobjective benchmark test problems over continuous and mixed-variable decision spaces under controlled scale heterogeneity · DOI [10.5281/zenodo.20783713](https://doi.org/10.5281/zenodo.20783713)
- [`DFO_Benchmark_Suite`](https://github.com/aguilarmadeira/DFO_Benchmark_Suite) — solver-independent benchmark for derivative-free and mixed-variable black-box optimization: continuous, discrete and categorical problems with known global optima · v2.1.0 DOI [10.5281/zenodo.24041183](https://doi.org/10.5281/zenodo.24041183) · all versions DOI [10.5281/zenodo.20782892](https://doi.org/10.5281/zenodo.20782892)
- [`mixed-spaces-supplementary`](https://github.com/aguilarmadeira/mixed-spaces-supplementary) — supplementary code for a manuscript on mixed-variable optimisation as a metric product space

---

## Benchmark test-problem collections

Open, self-contained MATLAB test problems for benchmarking derivative-free solvers, across single- and multi-objective settings and continuous, discrete, categorical and mixed-variable decision spaces. `DFO_Benchmark_Suite` v2.1.0 instantiates the same base problems in **all seven combinations of the three variable types** — continuous (C), ordered discrete (D) and categorical (K) — so that the effect of each type, and of their combination, can be compared on identical base problems with known global optima.

| Setting | Variables | Base problems | Instances | Repository |
| --- | --- | --- | --- | --- |
| Single-objective (v2.1.0) | C, D, K, DK, CD, CK, CDK (7 type patterns²), known global optima | 55 + Family BK | 841 | [`DFO_Benchmark_Suite`](https://github.com/aguilarmadeira/DFO_Benchmark_Suite) |
| Single-objective (v1.0.0) | Continuous / Mixed (C/D/K), 8 heterogeneity strategies | 63 | 504 + 504 | [`DFO_Benchmark_Suite` @ v1.0.0](https://github.com/aguilarmadeira/DFO_Benchmark_Suite/tree/v1.0.0) |
| Multi-objective | Continuous | 108 | 864 (× 8 strategies) | [`MOO_Prob_Matlab`](https://github.com/aguilarmadeira/MOO_Prob_Matlab) |
| Multi-objective | Mixed (C/D/K) | 108 | 864 (× 8 strategies) | [`MOO_Prob_Matlab`](https://github.com/aguilarmadeira/MOO_Prob_Matlab) |
| Multi-objective — base set¹ | Continuous | 108 | — (unscaled) | [`MOO_Prob_Matlab`](https://github.com/aguilarmadeira/MOO_Prob_Matlab) |

<sub>The eight heterogeneity strategies are shared by `DFO_Benchmark_Suite` v1.0.0 and `MOO_Prob_Matlab`. The `sobol_digit_oscillatory` contrast is κ = 1e8 in the single-objective suite and κ = 1e6 in the multi-objective suite, matching the settings used in the respective studies.</sub>

<sub>¹ Base set: MATLAB conversions of the original Direct MultiSearch (DMS) problems, originally distributed in AMPL — the reference set (`problems/`) from which the multi-objective collections above are derived.</sub>

<sub>² Variable-type patterns of `DFO_Benchmark_Suite` v2.1.0: all continuous (C), all ordered discrete (D), all categorical (K), and the mixed combinations DK, CD, CK and CDK, built from 55 classical base instances; continuous coordinates under three scale strategies (baseline, moderate, extreme) where they change the problem; plus Family BK, synthetic problems with nominal categories and a controlled continuous–categorical interaction. Every instance has a known, justified global optimum; the domains are chosen so that the optimum is never at the centre of the box (v2.0.0, DOI [10.5281/zenodo.24037856](https://doi.org/10.5281/zenodo.24037856), is superseded).</sub>

<sub>Archived and citable on Zenodo — `DFO_Benchmark_Suite`: v2.1.0 DOI [10.5281/zenodo.24041183](https://doi.org/10.5281/zenodo.24041183), v2.0.0 DOI [10.5281/zenodo.24037856](https://doi.org/10.5281/zenodo.24037856), v1.0.0 DOI [10.5281/zenodo.20782893](https://doi.org/10.5281/zenodo.20782893), all versions DOI [10.5281/zenodo.20782892](https://doi.org/10.5281/zenodo.20782892) · `MOO_Prob_Matlab`: DOI [10.5281/zenodo.20783713](https://doi.org/10.5281/zenodo.20783713).</sub>

---

## Teaching

- [`optimization-course`](https://github.com/aguilarmadeira/optimization-course) — lecture notes and code for the **Optimization** course at ISEL: slides in Portuguese and English (PDF), MATLAB and Python code that reproduces every example on the slides, and Google Colab notebooks. Covers univariate and multivariate methods, constrained optimization, global optimization (GLODS, simulated annealing, genetic algorithms) and multiobjective optimization (DMS, NSGA-II).
- [`linear-algebra-course`](https://github.com/aguilarmadeira/linear-algebra-course) — slides, exercise sheets and code for the **Linear Algebra** course at ISEL: slides and exercise sheets in Portuguese and English (PDF), with solutions released during the semester, and short Python/MATLAB examples with Google Colab notebooks. Covers complex numbers, vector spaces, matrices and linear systems, determinants, inner product and geometry in ℝ³, and eigenvalues and diagonalization.
---

## Research Interests

Derivative-free optimization · Multiobjective optimization · Direct-search methods · Decision Sciences and operations research · Industrial applications in transit operations, vehicle routing, postal logistics and energy systems

---

## Profiles and Affiliations

[ORCID 0000-0001-9523-3808](https://orcid.org/0000-0001-9523-3808) · [CiênciaVitae 6F1E-DCF0-D6EC](https://www.cienciavitae.pt/6F1E-DCF0-D6EC) · [ResearcherID N-6918-2016](https://www.webofscience.com/wos/author/record/N-6918-2016) · [Scopus 7003405549](https://www.scopus.com/authid/detail.uri?authorId=7003405549) · [Personal page](https://web.tecnico.ulisboa.pt/aguilarmadeira/)

[IDMEC](https://www.idmec.tecnico.ulisboa.pt/) · [ISEL — Department of Mathematics](https://www.isel.pt/)

---

## Indicators

h-index 22 · 1,363 citations (Web of Science) · Two PhDs (Mathematics, IST 2019; Mechanical Engineering, IST 2004) · Habilitation in Mathematics (Universidade de Évora, 2021)

---

## Selected Awards

- **2023** — IPL / CGD Scientific Excellence Award (Technologies and Engineering, triennium 2020–2022)
- **2021** — IPL / CGD Award for Recognition of Activities with Community Relevance (triennium 2018–2020)
- **2019–2022** — Four IPL / CGD merit diplomas for scientific work in Technologies and Engineering
- **2004–2021** — *Excelente* (highest rating) in 18 consecutive ISEL teaching evaluations

---

## Contact

ISEL · Rua Conselheiro Emídio Navarro 1, 1959-007 Lisboa, Portugal · `jose.madeira (at) isel.pt`
IDMEC · Av. Rovisco Pais 1, 1049-001 Lisboa, Portugal · `aguilarmadeira (at) tecnico.ulisboa.pt`
