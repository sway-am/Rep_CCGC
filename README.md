

# Cluster-guided Contrastive Graph Clustering Network

<p align="center">   
    <a href="https://pytorch.org/" alt="PyTorch">
      <img src="https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?e&logo=PyTorch&logoColor=white" /></a>
    <a href="https://aaai.org/Conferences/AAAI-23/" alt="Conference">
        <img src="https://img.shields.io/badge/AAAI'23-brightgreen" /></a>
<p/>





An official source code for paper [Re] Reproducibility Study : Cluster-guided Contrastive
 Graph Clustering Network. If you find this repository useful to your research or work, it is really appreciate to star this repository. :heart:

-------------

### Overview

<p align = "justify"> 
We propose a Cluster-guided Contrastive deep Graph Clustering network (CCGC) by mining the intrinsic supervision information in the high-confidence clustering results. Specifically, instead of conducting complex node or edge perturbation, we construct two views of the graph by designing special Siamese encoders whose weights are not shared between the sibling sub-networks. Then, guided by the high-confidence clustering information, we carefully select and construct the positive samples from the same high-confidence cluster in two views. Moreover, to construct semantic meaningful negative sample pairs, we regard the centers of different high-confidence clusters as negative samples, thus improving the discriminative capability and reliability of the constructed sample pairs. Lastly, we design an objective function to pull close the samples from the same cluster while pushing away those from other clusters by maximizing and minimizing the cross-view cosine similarity between positive and negative samples. Extensive experimental results on six datasets demonstrate the effectiveness of CCGC compared with the existing state-of-the-art algorithms.




<div  align="center">    
    <img src="CCGC_MLRC/assests/CCGC_model.png" width=80%/>
</div>

<div  align="center">    
    Figure 1: Overall framework of CCGC.
</div>



### Requirements

The proposed CCGC is implemented with python 3.7 on Google Colab standard CPU and T4 GPU. 

Python package information is summarized in **requirements.txt**:

- torch==1.7.1
- tqdm==4.59.0
- numpy==1.19.2
- munkres==1.1.4
- scikit_learn==1.2.0





### Quick Start

Refer HOW_TO_RUN.md



### Clustering Results

<div  align="center">    
    <img src="CCGC_MLRC/assests/results.jpg" width=100%/>
</div>
<div  align="center">    
    Table 7: Clustering results of our ablation study  on six datasets.
</div>




