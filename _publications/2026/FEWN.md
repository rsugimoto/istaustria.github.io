---
layout: publication
title: "Fast and Exact Winding Numbers for Triangle Meshes"

authors:
  - name: Xie, Peiyuan
    affiliations: [1]
    url: https://visualcomputing.ist.ac.at/people/grpren/
  - name: Hafner, Christian
    affiliations: [1]
    url: https://chrishafner.github.io/
  - name: Wojtan, Chris
    affiliations: [1]
    url: https://pub.ista.ac.at/~wojtan/

affiliations:
  - name: ISTA
    url: https://ista.ac.at

publication: ACM Transactions on Graphics (Siggraph 2026)
date: 2026-07-19
doi: https://dl.acm.org/doi/10.1145/3811339

bibtex: |
  @article{FastExactWindingNumbersXie26,
    author = {Xie, Peiyuan and Hafner, Christian and Wojtan, Chris},
    title = {Fast and Exact Winding Numbers for Triangle Meshes},
    year = {2026},
    volume = {45},
    number = {4},
    journal = {ACM Trans. Graph.},
    month = jul,
    articleno = {41},
    numpages = {8}
  }

grp: wojtan
paper: https://research-explorer.ista.ac.at/download/22241/22249/2026_TransactionsGraphics_Xie.pdf
code: https://git.ista.ac.at/wojtan-group/peiyuan-xie/boundaryblaze

abstract: |
  We revisit the computation of 3D generalized winding numbers, a useful measure for inside-outside classification on triangle meshes with gaps, self-intersections, and open boundaries. At the core of our new method is an analytical reduction of the surface integral that defines the winding number, resulting in a single ray-mesh intersection test and an elementary sum over boundary edges per evaluation. This construction is orders of magnitude more efficient than the state of the art in practice, which we show in an extensive performance benchmark. Conveniently, the method also reduces to the best-available asymptotic complexity in the worst case, and it introduces no approximations apart from floating-point errors. Our algorithm is conceptually simple to understand, straightforward to implement and debug, and it works reliably even on extremely noisy and corrupt input geometry. 

teaser:
  caption: |

  images:
  - url: teaser.jpg
    alt: Fast and Exact Winding Numbers (Teaser Image)

---

## {{ page.title }}

{% include figure.html caption=page.teaser.caption images=page.teaser.images columns=1 %}

{% include authors.html authors=page.authors affiliations=page.affiliations %}

{% include publication.html publication=page.publication url=page.doi %}

### Abstract

{{ page.abstract }}

### Resources

* [Paper (5.2 MB)]({{ page.paper }})
* [**Source Code** (Git Repository)]({{ page.code }})

### Citation

{% include citation.html citation=page.bibtex %}

### Acknowledgements
We thank Sadashige Ishida and Ryusuke Sugimoto for their insightful discussions and proofreading and other members of the ISTA Visual Computing Group for their general feedback. Special thanks to David Palmer, Yi-Lu Chen, Carmen Farr and Ladislav Trnka for their help with the fastforward video. This project was funded in part by the European Research Council
(ERC Consolidator Grant 101045083 CoDiNA).

![EU](flag_yellow_low.jpg){: width="150x"}
![ERC](LOGO-ERC.jpg){: width="150px"}
