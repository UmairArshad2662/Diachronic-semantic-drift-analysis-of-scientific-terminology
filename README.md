# Diachronic Semantic Drift in Scientific Terminology (1665–1920)

A computational linguistics project tracking the lexical evolution of foundational scientific vocabulary (*cell*, *charge*, *current*, *mass*, *ray*) across 255 years of the Royal Society Corpus (RSC 6.0 Open).

### Key Features
- **Temporal Slicing**: Partitions 250+ years of scientific publications into three historical eras (1665–1750, 1751–1830, 1831–1920).
- **Distributional Semantics**: Trains independent Skip-Gram with Negative Sampling (SGNS) models per epoch.
- **Coordinate Alignment**: Maps vector spaces into a shared coordinate frame via Orthogonal Procrustes (SVD).
- **Statistical Validation**: Evaluates global cosine displacement $\Delta(w)$ and local Jaccard neighborhood turnover ($J_{10}$) against frequency-matched control baselines (*water*, *iron*, *glass*, *day*) using Welch's $t$-test ($p < 0.01$).
