# Mathematical Analysis of the Cone Surface

**Author:** Dogan Balban  
**Language:** German (primary) and English (translation)  
**License:** CC BY 4.0

## Overview

This repository contains a complete differential-geometric analysis of the circular
cone surface defined by

$$z = -\frac{3}{4} + \frac{\pi}{2}r$$

(simplified form in cylindrical coordinates), originally expressed as

$$z = -\frac{1}{12}\cdot 3^{2} + 6\cdot\sqrt{\frac{x^{2}}{(12/\pi)^{2}}+\frac{y^{2}}{(12/\pi)^{2}}}$$

## Repository Structure

```
.
├── Kegelanalyse.tex              # German version (primary)
├── cone_analysis_en.tex          # English 
├── README.md                     # This file
├── LICENSE                       # CC BY 4.0
└── zenodo_description.md         # Zenodo metadata / abstract
```

## Key Mathematical Results

| Property | Formula / Value |
|---|---|
| Simplified form | $z = -3/4 + (\pi/2)r$ |
| Surface type | Right circular cone |
| Apex | $(0, 0, -3/4)$ |
| Slope | $m = \pi/2$ |
| **Cone half-angle** $\alpha$ (axis–generator) | $\arctan(2/\pi) \approx 32.48°$ |
| Elevation angle $\beta$ (generator–horizontal) | $\arctan(\pi/2) \approx 57.52°$ |
| **Apex angle** $2\alpha$ | $2\arctan(2/\pi) \approx 64.96°$ |
| Gaussian curvature | $K = 0$ (developable) |
| **Mean curvature** | $H = \pi/(4r\sqrt{1+\pi^2/4})$ |
| Gradient magnitude | $\|\nabla f\| = \pi/2$ (constant) |
| Lateral surface area | $A = \pi\sqrt{1+\pi^2/4}\cdot(r_2^2-r_1^2)$ |
| Volume | $V = (4/3\pi)\left[(h_2+3/4)^3-(h_1+3/4)^3\right]$ |

## Compilation

```bash
pdflatex Kegelanalyse.tex
pdflatex cone_analysis_en.tex
```

**Required LaTeX packages:** `amsmath`, `amssymb`, `amsthm`, `mathtools`, `booktabs`,
`hyperref`, `cleveref`, `float`, `array`, `xcolor`, `geometry`.

## Numerical Table Values

### Lateral Surface Area $A = \pi\sqrt{1+\pi^2/4}\cdot(r_2^2-r_1^2)$

| $r_1$ | $r_2$ | $A$ |
|---|---|---|
| 0 | 5  | 146.249 |
| 0 | 10 | 584.995 |
| 5 | 10 | 438.746 |
| 0 | 20 | 2339.979 |

### Volume $V = (4/3\pi)\left[(h_2+3/4)^3-(h_1+3/4)^3\right]$

| $h_1$ | $h_2$ | $V$ |
|---|---|---|
| −0.75 | 0  | 0.179 |
| 0     | 10 | 527.068 |
| −0.75 | 10 | 527.247 |
| 0     | 20 | 3791.601 |

## Related Publications (Companion Papers)

This paper is part of a series on the conical helix $\gamma(\theta) = (a\theta\cos\theta,\, a\theta\sin\theta,\, b\theta)$
with $a = 6/\pi^2 = 1/\zeta(2)$, $b = 3/\pi$:

1. **This paper** — Analysis of the cone $z = -3/4 + (\pi/2)r$
2. [Kegelhelix Differentialgeometrie](../conical-helix-analysis/) — Curvature, torsion, Frenet frame of the conical helix
3. Archimedean spiral analysis — The $xy$-projection

## Citation

```bibtex
@misc{balban2026kegel,
  author       = {Balban, Dogan},
  title        = {Mathematical Analysis of the Cone Surface},
  year         = {2026},
  publisher    = {GitHub},
  howpublished = {\url{[https://github.com/dogan1908/cone_analysis]}}
}
```
Publication: Differential‑Geometric Analysis of the Conical Helix — DOI: [10.5281/zenodo.18728571](https://doi.org/10.5281/zenodo.18728571)

## Contact

Questions and corrections welcome via GitHub Issues.
