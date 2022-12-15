# Tutorial for “Empirical Analysis of EIP-1559: Transaction Fees, Waiting Time, and Consensus Security”
## Project information
- **Author**: Tianyu Wu, Applied Mathematics and Computational Science, Class of 2023, Duke Kunshan University
- **Acknowledgments**: I would like to express my greatest gratitude to Prof. Luyao Zhang and Prof. Fan Zhang for guidance during my summer experiential learning activities in their project entitled “Understand Waiting Time in Transaction Fee Mechanisms,” supported by Ethereum Foundation. 

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
### Methodology
<img src="https://github.com/cs-econ-blockchain/tutorial-eip1559-wt/blob/main/fig/fig1.png" width="800">

Figure 1: Workflow of mempool data integration and cleaning [[Whimsical]](https://whimsical.com/waitingtime-transaction-JuzaYc8TCWZwn3ZoMiMJy6)

<img src="https://github.com/cs-econ-blockchain/tutorial-eip1559-wt/blob/main/fig/fig2.png" width="800">

Figure 2: Derivation of waiting time on transaction level [[Whimsical]](https://whimsical.com/waitingtime-transaction-JuzaYc8TCWZwn3ZoMiMJy6)

<img src="https://github.com/cs-econ-blockchain/tutorial-eip1559-wt/blob/main/fig/fig3.png" width="800">

Figure 3: Pipeline of sample data import [[Whimsical]](https://whimsical.com/waitingtime-transaction-JuzaYc8TCWZwn3ZoMiMJy6)

### Results
<img src="https://github.com/cs-econ-blockchain/tutorial-eip1559-wt/blob/main/fig/fig4.png" width="800">

Figure 4: Waiting Time Distribution Plot and Boxplot (Pre-EIP and Post-EIP), by removing all negative waiting times [[Analyze Data]](https://github.com/cs-econ-blockchain/tutorial-eip1559-wt/blob/main/code/data_analysis_colab.ipynb)

<img src="https://github.com/cs-econ-blockchain/tutorial-eip1559-wt/blob/main/fig/fig5.png" width="800">

Figure 5: Waiting Time Distribution Plot and Boxplot (Pre-EIP and Post-EIP), by setting all negative waiting times to 0 [[Analyze Data]](https://github.com/cs-econ-blockchain/tutorial-eip1559-wt/blob/main/code/data_analysis_colab.ipynb)

<img src="https://github.com/cs-econ-blockchain/tutorial-eip1559-wt/blob/main/fig/fig6.png" width="800">

Figure 6: Median Waiting Time for Each Block (Pre-EIP and Post-EIP), Derived by Transaction Data until 08/27/2021 [[Analyze Data]](https://github.com/cs-econ-blockchain/tutorial-eip1559-wt/blob/main/code/data_analysis_colab.ipynb)

<img src="https://github.com/cs-econ-blockchain/tutorial-eip1559-wt/blob/main/fig/fig7.png" width="800">

Figure 7: Median Waiting Time for Each Block (Pre-EIP and Post-EIP with an extended period), Derived by Transaction Data until 10/27/2021 [[Analyze Data]](https://github.com/cs-econ-blockchain/tutorial-eip1559-wt/blob/main/code/data_analysis_colab.ipynb)

### Extension
<img src="https://github.com/cs-econ-blockchain/tutorial-eip1559-wt/blob/main/fig/fig8.png" width="800">

Figure 8: Difference between legacy transaction and EIP-1559 transaction after London hardfork [[Whimsical]](https://whimsical.com/legacy-and-eip-8yeixQBNpUtrRYy5NmbH7L)

<img src="https://github.com/cs-econ-blockchain/tutorial-eip1559-wt/blob/main/fig/fig9.png" width="800">

Figure 9: Median Waiting Time for Each Block (Pre-EIP and Post-EIP), with the tag differentiating between EIP and legacy auction, Derived by Transaction Data until 08/27/2021 [[Analyze Data]](https://github.com/cs-econ-blockchain/tutorial-eip1559-wt/blob/main/code/data_analysis_colab.ipynb)


## More about the Author
<img src="https://github.com/cs-econ-blockchain/tutorial-eip1559-wt/blob/main/Tianyu_Wu.jpg" width="100">
Tianyu Wu is a senior student at Duke Kunshan University, majoring in Applied Mathematics and Computational Science/Math. He has been serving on many pioneering interdisciplinary projects for the great cause of research, innovation, and leadership, mentored by Prof Luyao Zhang.


## References

### Data Source
- [Kaggle - Ethereum Blockchain](https://www.kaggle.com/datasets/bigquery/ethereum-blockchain)
- [Kaggle - Mempool Data (With Filtered Version)](https://www.kaggle.com/datasets/sunshineluyaozhang/eip1559-waiting-time)

### Code Source
- [Empirical_Analysis_of_EIP_1559_Transaction_Fees, User_Experience, and_Consensus_Security](https://github.com/SciEcon/EIP1559/tree/main/code)

### Articles
- [Empirical_Analysis_of_EIP_1559_Transaction_Fees, User_Experience, and_Consensus_Security](https://arxiv.org/abs/2201.05574)
- [DETER: Denial of Ethereum Txpool sERvices](https://cve.report/CVE-2022-23327/32c14097.pdf)
### Literature
Bibliography Li, Kai, Yibo Wang, and Yuzhe Tang. 2021. “DETER: Denial of Ethereum Txpool SERvices.” Proceedings of the 2021 ACM SIGSAC Conference on Computer and Communications Security, November. https://doi.org/10.1145/3460120.3485369.

Liu, Yulin, Yuxuan Lu, Kartik Nayak, Fan Zhang, Luyao Zhang, and Yinhong Zhao. 2022. “Empirical Analysis of EIP-1559: Transaction Fees, Waiting Time, and Consensus Security.” ArXiv:2201.05574 [Cs, Econ, Q-Fin], January. https://arxiv.org/abs/2201.05574.
