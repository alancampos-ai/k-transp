# Connection Rigidity and Curvature Recovery

#### Article: <small><strong>Connection Rigidity and Curvature Recovery from Transported Subspaces</strong> <a href=""><img src="https://cdn.simpleicons.org/doi/2dd4bf" alt="DOI" height="14" align="absmiddle"></a> <a href=""><img src="https://cdn.simpleicons.org/zenodo/2dd4bf" alt="Zenodo" height="14" align="absmiddle"></a> <a href="https://drive.google.com/drive/folders/1PlunGHC0qKcJXo_iTaZBk3y-BjwdRh8K?usp=sharing"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/google/google-original.svg" alt="Google Drive" height="14" align="absmiddle"></a></small>

We recover smooth connections and curvature from embedded spaces of transported sections. Nodal evaluation determines active parallel transports and connection values. Under radial completeness, we characterize affine observation fibers and establish an exact visibility criterion for injectivity. We derive stability bounds for nodal lifting maps. On bounded $C^{p+1}$ classes, polynomial interpolation attains the optimal curvature rate $h_X^p+\varepsilon^{p/(p+1)}$ from noisy nodal first jets. Experiments compare six methods on the flat two-torus across four grid sizes and three noise levels with 20 paired seeds. At $n=48$ and $\varepsilon=10^{-4}$, NCP attains a mean maximum sampled curvature error of $4.087\times10^{-3}$, a $75.7\%$ reduction relative to Fourier, with mean runtime $40.96$ ms. We also characterize the metrics sharing a Levi–Civita connection.

#### Dependencies

The experiments used Ubuntu 24.04.4 LTS and Python 3.12.12 with the following dependencies:

* NumPy 2.2.6
* SciPy 1.15.3
* Matplotlib 3.10.3
* psutil 7.0.0
* PyYAML 6.0.2
* threadpoolctl 3.6.0

#### Installation

```bash
docker build --pull -f docker/Dockerfile -t ncp-benchmark:1.0.0 .
docker run --rm -v ncp-dataset:/app/dataset -v ncp-results:/app/results ncp-benchmark:1.0.0
```

#### License (MIT)

* Copyright (c) alancampos-ai
* Code released under the MIT License.
