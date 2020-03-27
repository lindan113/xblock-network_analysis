
## Description
This dataset contains transaction records of 445 phishing accounts and 445 non-phishing accounts of Ethereum. We obtain 445 phishing accounts labeled by [Etherscan](etherscan.io) and the same number of randomly selected unlabeled accounts as our objective nodes. The dataset can be used to conduct node classification of financial transaction networks. 

We collect the transaction records based on an assumption that for a typical money transfer flow centered on a phishing node, the previous node of the phishing node may be a victim, and the next one to three nodes may be the bridge nodes with money laundering behaviors, as figure shows. Therefore, we collect subgraphs by [K-order sampling](https://ieeexplore.ieee.org/document/8964468) with K-in = 1, K-out = 3 for each of the 890 objective nodes and then splice them into a large-scale network with 86,623 nodes. 

![A schematic illustration of a directed K-order subgraph for phishing node classification.](https://s1.ax1x.com/2020/03/27/GCZGmd.md.jpg)

## Website
[XBlock](http://xblock.pro/ethereum/) collects the current mainstream blockchain data and is one of the blockchain data platforms with the largest amount of data and the widest coverage in the academic community.

All blockchain datasets have been cleaned and classified in a standardized way, which can be easily downloaded into a standard and consistent format. 

## Citation
```
@article{ wu2019tedge,
	author = "Jiajing Wu and Dan Lin and Qi Yuan and Zibin Zheng",
	title = "T-EDGE: Temporal WEighted MultiDiGraph Embedding for Ethereum Transaction Network Analysis",
	journal = "arXiv preprint arXiv:1905.08038",
	year = "2019",
	URL = "https://arxiv.org/abs/1905.08038"
}
```

## Contact
Please contact Dan Lin (lind8@mail2.sysu.edu.cn) for any questions about the dataset.
