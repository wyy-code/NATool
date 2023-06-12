# NATool
Introducing Network Alignment Toolkit (NAToll): a lightweight, user-friendly, and highly versatile PyTorch library for implementing various network alignment algorithms. With NAToll, you can effortlessly align networks and leverage its extensive range of functionalities.

# Library for Network Alignment (Graph Alignment)
## Overview
We have developed NATool, an open-source library for network alignment, using Python and PyTorch. The software architecture is depicted in the following Figure, showcasing the robustness and efficiency of NATool's design. To facilitate the integration of representative models and enable third-party developers to extend it according to their specific requirements, we abstract this framework into two main components: Encoder and Decoder. The Encoder takes the structural information of two graphs as input, with the option to include label information, and outputs the similarity matrices of the two graphs. The Decoder processes the obtained similarity matrices to derive the final alignment matrix. The Decoder is followed by a search module for alignment tasks. To facilitate the extension to other downstream tasks such as multimodal alignment and graph representation learning, we extract the search module from the Decoder component, allowing third-party developers to modify it as needed. The output of the search module is the final evaluation metric results.

## Algorithms

We integrate eleven representative network-alignment as Encoder and deocder. Their papers and the original codes are given in the following table.

|   Encoder   |     Paper     |
|:--------:|:------------:|
|  Isorank     |    [PNAS'2008](https://www.pnas.org/content/105/35/12763)    |
|  NSD       |    [IEEE'2012](https://ieeexplore.ieee.org/document/5975146)    |
|  Big-Align  |  [IEEE'2013](https://ieeexplore.ieee.org/abstract/document/6729523)  |
|  FINAL   |  [KDD '2016](https://dl.acm.org/doi/abs/10.1145/2939672.2939766)  |
|  Regal     |    [CIKM '2018](https://dl.acm.org/doi/10.1145/3269206.3271788)    |
|  LREA        |    [WWW '2018](https://dl.acm.org/doi/10.1145/3178876.3186128)    |
|  GWL  |  [arXiv'2019](https://arxiv.org/abs/1901.06003)  |
|  CΟΝΕ   |  [CIKM '2020](https://dl.acm.org/doi/10.1145/3340531.3412136)  |
| Grampa        | [ICML'2020](https://dl.acm.org/doi/abs/10.5555/3524938.3525218) |
|  Grasp        |    [APWeb-WAIM'2021](https://link.springer.com/chapter/10.1007/978-3-030-85896-4_4)    |
| B-Grasp        | [TKDD'2023](https://dl.acm.org/doi/full/10.1145/3561058) |
|   **Decoder**   |     **Paper**     |
|  RefiNA  |  [SIAM'2021](https://epubs.siam.org/doi/abs/10.1137/1.9781611976700.20)  |
|  CAPER  |  [arXiv'2022](https://arxiv.org/abs/2208.10682)  |
|  Greed-Match  |  [-](-)   |
|  Sinkhorn  | [-](-)  |

## Acknowledgement
The Code base is built upon the following work -
- [thanhtrunghuynh93](https://github.com/thanhtrunghuynh93/networkAlignment)
- [constantinosskitsas](https://github.com/constantinosskitsas/Framework_GraphAlignment)
- [CAPER](https://github.com/GemsLab/CAPER)

















