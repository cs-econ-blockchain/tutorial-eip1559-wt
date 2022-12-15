# Tutorial for “Empirical Analysis of EIP-1559: Transaction Fees, Waiting Time, and Consensus Security”
## Project information
- **Author**: Tianyu Wu, Applied Mathematics and Computational Science, Class of 2023, Duke Kunshan University
- **Instructor**: Prof. Luyao Zhang, Duke Kunshan University
- **Disclaimer**: TBD
- **Acknowledgments**: I would like to express my greatest gratitude to Prof Luyao Zhang, the Principal Investigator (PI) of the project “Understanding Waiting Time in Transaction Fee Mechanisms”, and Prof Fan Zhang, the Co-PI for their generous and inspiring instructions.

- **Project Summary**: 

In this article, we provide a tutorial for replicating the waiting time results in the paper entitled [“Empirical Analysis of EIP-1559: Transaction Fees, Waiting Time, and Consensus Security”](https://arxiv.org/abs/2201.05574). As a data descriptor, we introduce two reliable data sources related to the empirical analysis of waiting time in the transaction fee mechanism: mempool data and blockchain transaction-level data, and describe the workflow to integrate these two data sources for further analysis. Subsequently, we demonstrate the step-by-step instructions for the data importing process and create a series of visualizations to replicate, validate, and extend the results in the original paper that advances the understanding of how the EIP-1559 can affect waiting time in the transaction fee mechanism on Ethereum .

## Table of Contents
- [Data](https://github.com/cs-econ-blockchain/tutorial-eip1559-wt#data)
- [Code](https://github.com/cs-econ-blockchain/tutorial-eip1559-wt#code)
- [Spotlight](https://github.com/cs-econ-blockchain/tutorial-eip1559-wt#spotlight)
- [More about the Author](https://github.com/cs-econ-blockchain/tutorial-eip1559-wt#more-about-the-author)
- [References](https://github.com/cs-econ-blockchain/tutorial-eip1559-wt#references)



## Data
<div class="table-wrapper" markdown="block">

|                    |**Mempool Data**|**Blockchain Data**|
|--------------------|:--------------------:|:--------------------:|
| **Data Source**    | Observed by nodes set on the blockchain|[Kaggle - Ethereum Blockchain](https://www.kaggle.com/datasets/bigquery/ethereum-blockchain)|
| **Queried Data**   |[Kaggle - Mempool Data (With Filtered Version)](https://www.kaggle.com/datasets/sunshineluyaozhang/eip1559-waiting-time)|[Kaggle - Queried Blockchain Data](https://www.kaggle.com/datasets/henrytyw/queried-blockchain-data)|
| **Processed Data** |[Kaggle - Processed Data]()|[Kaggle - Processed Data]()|

</div>


## Code
- [Query Data](https://github.com/cs-econ-blockchain/tutorial-eip1559-wt/blob/main/code/data_query_colab.ipynb)
- [Process Data](https://github.com/cs-econ-blockchain/tutorial-eip1559-wt/blob/main/code/data_process_colab.ipynb)
- [Analyze Data](https://github.com/cs-econ-blockchain/tutorial-eip1559-wt/blob/main/code/data_analysis_colab.ipynb)

## Spotlight
- Figures
- Posters
- Slides
- Presentations
- Review articles
- Media appearance

## More about the Author
<img src="https://github.com/cs-econ-blockchain/tutorial-eip1559-wt/blob/main/Tianyu_Wu.jpg" width="100">
Tianyu Wu is a senior student at Duke Kunshan University, majoring in Applied Mathematics and Computational Science/Math. He has been serving on many pioneering interdisciplinary projects for the great cause of research, innovation, and leadership, mentored by Prof Luyao Zhang.


## References

### Data Source
- Data Source Title and URL
### Code Source
- Code Source Title and URL
### Articles
- Article Source Title and URL
### Literature
- Literature References in [Chicago Author-Date](https://www.chicagomanualofstyle.org/tools_citationguide/citation-guide-2.html) Style and [BibTex](https://scholar.google.com/) 

Levin, Dan, and Luyao Zhang. 2020. “Bridging Level-K to Nash Equilibrium.” *The Review of Economics and Statistics* 104 (6): 1329–40. https://doi.org/10.1162/rest_a_00990.

```
@article{levin2022bridging,
  title={Bridging level-k to nash equilibrium},
  author={Levin, Dan and Zhang, Luyao},
  journal={Review of Economics and Statistics},
  volume={104},
  number={6},
  pages={1329--1340},
  year={2022},
  publisher={MIT Press One Rogers Street, Cambridge, MA 02142-1209, USA journals-info~…}
}
```

