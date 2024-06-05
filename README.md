# Awesome Graph Neural Network Systems [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

A list of awesome systems for graph neural network (GNN). If you have any comment, please create an [issue](https://github.com/chwan1016/awesome-gnn-systems/issues) or [pull request](https://github.com/chwan1016/awesome-gnn-systems/pulls).
## Contents
- [Open Source Libraries](#open-source-libraries)
- [Papers](#papers)
  - [Survey Papers](#survey-papers)
  - [GNN Libraries](#gnn-libraries)
  - [GNN Kernels](#gnn-kernels)
  - [GNN Compilers](#gnn-compilers)
  - [Distributed GNN Training Systems](#distributed-gnn-training-systems)
  - [Training Systems for Scaling Graphs](#training-systems-for-scaling-graphs)
  - [Quantized GNNs](#quantized-gnns)
  - [GNN Dataloaders](#gnn-dataloaders)
  - [GNN Training Accelerators](#gnn-training-accelerators)
  - [GNN Inference Accelerators](#gnn-inference-accelerators)
- [Contribute](#contribute)
## Open Source Libraries
- [PyG: Graph Neural Network Library for PyTorch](https://github.com/rusty1s/pytorch_geometric) ![GitHub stars](https://img.shields.io/github/stars/rusty1s/pytorch_geometric.svg?logo=github&label=Stars)
- [DGL: Python Package Built to Ease Deep Learning on Graph](https://github.com/dmlc/dgl) ![GitHub stars](https://img.shields.io/github/stars/dmlc/dgl.svg?logo=github&label=Stars)
- [Graph Nets: Build Graph Nets in Tensorflow](https://github.com/deepmind/graph_nets) ![GitHub stars](https://img.shields.io/github/stars/deepmind/graph_nets.svg?logo=github&label=Stars)
- [Euler: A Distributed Graph Deep Learning Framework](https://github.com/alibaba/euler) ![GitHub stars](https://img.shields.io/github/stars/alibaba/euler.svg?logo=github&label=Stars)
- [StellarGraph: Machine Learning on Graphs](https://github.com/stellargraph/stellargraph) ![GitHub stars](https://img.shields.io/github/stars/stellargraph/stellargraph.svg?logo=github&label=Stars)
- [Spektral: Graph Neural Networks with Keras and Tensorflow 2](https://github.com/danielegrattarola/spektral) ![GitHub stars](https://img.shields.io/github/stars/danielegrattarola/spektral.svg?logo=github&label=Stars)
- [PGL: An Efficient and Flexible Graph Learning Framework Based on PaddlePaddle](https://github.com/PaddlePaddle/PGL) ![GitHub stars](https://img.shields.io/github/stars/PaddlePaddle/PGL.svg?logo=github&label=Stars)
- [CogDL: An Extensive Toolkit for Deep Learning on Graphs](https://github.com/THUDM/cogdl) ![GitHub stars](https://img.shields.io/github/stars/THUDM/cogdl.svg?logo=github&label=Stars)
- [DIG: A Turnkey Library for Diving into Graph Deep Learning Research](https://github.com/divelab/DIG) ![GitHub stars](https://img.shields.io/github/stars/divelab/DIG.svg?logo=github&label=Stars)
- [Jraph: A Graph Neural Network Library in Jax](https://github.com/deepmind/jraph) ![GitHub stars](https://img.shields.io/github/stars/deepmind/jraph.svg?logo=github&label=Stars)
- [Graph-Learn: An Industrial Graph Neural Network Framework](https://github.com/alibaba/graph-learn) ![GitHub stars](https://img.shields.io/github/stars/alibaba/graph-learn.svg?logo=github&label=Stars)
- [DeepGNN: a Framework for Training Machine Learning Models on Large Scale Graph Data](https://github.com/microsoft/DeepGNN) ![GitHub stars](https://img.shields.io/github/stars/microsoft/DeepGNN.svg?logo=github&label=Stars)
## Papers
### Survey Papers
| Venue | Title | Affiliation | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Link&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;Source&nbsp;&nbsp; |
| :---: | :---: | :---------: | :---: | :----: |
|arXiv 2022|Distributed Graph Neural Network Training: A Survey|BUPT| [[paper]](https://arxiv.org/abs/2211.00216)![Scholar citations](https://img.shields.io/badge/Citations-18-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|arXiv 2022|Parallel and Distributed Graph Neural Networks: An In-Depth Concurrency Analysis|ETHZ| [[paper]](https://arxiv.org/abs/2205.09702)![Scholar citations](https://img.shields.io/badge/Citations-33-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|CSUR 2022|Computing Graph Neural Networks: A Survey from Algorithms to Accelerators|UPC| [[paper]](https://dl.acm.org/doi/10.1145/3477141)![Scholar citations](https://img.shields.io/badge/Citations-210-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
### GNN Libraries
| Venue | Title | Affiliation | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Link&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;Source&nbsp;&nbsp; |
| :---: | :---: | :---------: | :---: | :----: |
|JMLR 2021|DIG: A Turnkey Library for Diving into Graph Deep Learning Research|TAMU| [[paper]](https://arxiv.org/abs/2103.12608)![Scholar citations](https://img.shields.io/badge/Citations-85-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/divelab/DIG)![GitHub stars](https://img.shields.io/github/stars/divelab/DIG.svg?logo=github&label=Stars)|
|arXiv 2021|CogDL: A Toolkit for Deep Learning on Graphs|THU| [[paper]](https://arxiv.org/abs/2103.00959)![Scholar citations](https://img.shields.io/badge/Citations-15-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/THUDM/cogdl)![GitHub stars](https://img.shields.io/github/stars/THUDM/cogdl.svg?logo=github&label=Stars)|
|CIM 2021|Graph Neural Networks in TensorFlow and Keras with Spektral|Università della Svizzera italiana| [[paper]](https://arxiv.org/abs/2006.12138)![Scholar citations](https://img.shields.io/badge/Citations-260-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/danielegrattarola/spektral)![GitHub stars](https://img.shields.io/github/stars/danielegrattarola/spektral.svg?logo=github&label=Stars)|
|arXiv 2019|Deep Graph Library: A Graph-Centric, Highly-Performant Package for Graph Neural Networks|AWS| [[paper]](https://arxiv.org/abs/1909.01315)![Scholar citations](https://img.shields.io/badge/Citations-1.2k-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/dmlc/dgl)![GitHub stars](https://img.shields.io/github/stars/dmlc/dgl.svg?logo=github&label=Stars)|
|VLDB 2019|AliGraph: A Comprehensive Graph Neural Network Platform|Alibaba| [[paper]](https://dl.acm.org/doi/pdf/10.14778/3352063.3352127)![Scholar citations](https://img.shields.io/badge/Citations-269-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/alibaba/graph-learn)![GitHub stars](https://img.shields.io/github/stars/alibaba/graph-learn.svg?logo=github&label=Stars)|
|arXiv 2019|Fast Graph Representation Learning with PyTorch Geometric|TU Dortmund University| [[paper]](https://arxiv.org/abs/1903.02428)![Scholar citations](https://img.shields.io/badge/Citations-4.1k-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/rusty1s/pytorch_geometric)![GitHub stars](https://img.shields.io/github/stars/rusty1s/pytorch_geometric.svg?logo=github&label=Stars)|
|arXiv 2018|Relational Inductive Biases, Deep Learning, and Graph Networks|DeepMind| [[paper]](https://arxiv.org/abs/1806.01261)![Scholar citations](https://img.shields.io/badge/Citations-3.5k-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/deepmind/graph_nets)![GitHub stars](https://img.shields.io/github/stars/deepmind/graph_nets.svg?logo=github&label=Stars)|
### GNN Kernels
| Venue | Title | Affiliation | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Link&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;Source&nbsp;&nbsp; |
| :---: | :---: | :---------: | :---: | :----: |
|MLSys 2022|Understanding GNN Computational Graph: A Coordinated Computation, IO, and Memory Perspective|THU| [[paper]](https://proceedings.mlsys.org/paper/2022/file/9a1158154dfa42caddbd0694a4e9bdc8-Paper.pdf)![Scholar citations](https://img.shields.io/badge/Citations-37-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/dgSPARSE/dgNN)![GitHub stars](https://img.shields.io/github/stars/dgSPARSE/dgNN.svg?logo=github&label=Stars)|
|HPDC 2022|TLPGNN: A Lightweight Two-Level Parallelism Paradigm for Graph Neural Network Computation on GPU|GW| [[paper]](https://dl.acm.org/doi/abs/10.1145/3502181.3531467)![Scholar citations](https://img.shields.io/badge/Citations-17-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|IPDPS 2021|FusedMM: A Unified SDDMM-SpMM Kernel for Graph Embedding and Graph Neural Networks|Indiana University Bloomington| [[paper]](https://arxiv.org/abs/2011.06391)![Scholar citations](https://img.shields.io/badge/Citations-41-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/HipGraph/FusedMM)![GitHub stars](https://img.shields.io/github/stars/HipGraph/FusedMM.svg?logo=github&label=Stars)|
|SC 2020|GE-SpMM: General-purpose Sparse Matrix-Matrix Multiplication on GPUs for Graph Neural Networks|THU| [[paper]](https://arxiv.org/abs/2007.03179)![Scholar citations](https://img.shields.io/badge/Citations-99-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/hgyhungry/ge-spmm)![GitHub stars](https://img.shields.io/github/stars/hgyhungry/ge-spmm.svg?logo=github&label=Stars)|
|ICCAD 2020|fuseGNN: Accelerating Graph Convolutional Neural Network Training on GPGPU|UCSB| [[paper]](https://seal.ece.ucsb.edu/sites/default/files/publications/fusegcn_camera_ready_.pdf)![Scholar citations](https://img.shields.io/badge/Citations-19-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/apuaaChen/gcnLib)![GitHub stars](https://img.shields.io/github/stars/apuaaChen/gcnLib.svg?logo=github&label=Stars)|
|IPDPS 2020|PCGCN: Partition-Centric Processing for Accelerating Graph Convolutional Network|PKU| [[paper]](https://ieeexplore.ieee.org/document/9139807)![Scholar citations](https://img.shields.io/badge/Citations-45-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
### GNN Compilers
| Venue | Title | Affiliation | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Link&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;Source&nbsp;&nbsp; |
| :---: | :---: | :---------: | :---: | :----: |
|MLSys 2022|Graphiler: Optimizing Graph Neural Networks with Message Passing Data Flow Graph|ShanghaiTech| [[paper]](https://proceedings.mlsys.org/paper/2022/file/a87ff679a2f3e71d9181a67b7542122c-Paper.pdf)![Scholar citations](https://img.shields.io/badge/Citations-20-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/xiezhq-hermann/graphiler)![GitHub stars](https://img.shields.io/github/stars/xiezhq-hermann/graphiler.svg?logo=github&label=Stars)|
|EuroSys 2021|Seastar: Vertex-Centric Programming for Graph Neural Networks|CUHK| [[paper]](http://www.cse.cuhk.edu.hk/~jcheng/papers/seastar_eurosys21.pdf)![Scholar citations](https://img.shields.io/badge/Citations-49-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|SC 2020|FeatGraph: A Flexible and Efficient Backend for Graph Neural Network Systems|Cornell| [[paper]](https://arxiv.org/pdf/2008.11359.pdf)![Scholar citations](https://img.shields.io/badge/Citations-81-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/dglai/FeatGraph)![GitHub stars](https://img.shields.io/github/stars/dglai/FeatGraph.svg?logo=github&label=Stars)|
### Distributed GNN Training Systems
| Venue | Title | Affiliation | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Link&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;Source&nbsp;&nbsp; |
| :---: | :---: | :---------: | :---: | :----: |
|arXiv 2023|Communication-Free Distributed GNN Training with Vertex Cut|Stanford| [[paper]](https://arxiv.org/pdf/2308.03209.pdf)![Scholar citations](https://img.shields.io/badge/Citations-0-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|arXiv 2023|GNNPipe: Accelerating Distributed Full-Graph GNN Training with Pipelined Model Parallelism|Purdue| [[paper]](https://arxiv.org/pdf/2308.10087.pdf)![Scholar citations](https://img.shields.io/badge/Citations-1-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|OSDI 2023|MGG: Accelerating Graph Neural Networks with Fine-Grained Intra-Kernel Communication-Computation Pipelining on Multi-GPU Platforms|UCSB| [[paper]](https://www.usenix.org/system/files/osdi23-wang-yuke.pdf)![Scholar citations](https://img.shields.io/badge/Citations-10-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/YukeWang96/MGG_OSDI23)![GitHub stars](https://img.shields.io/github/stars/YukeWang96/MGG_OSDI23.svg?logo=github&label=Stars)|
|VLDB 2022|Sancus: Staleness-Aware Communication-Avoiding Full-Graph Decentralized Training in Large-Scale Graph Neural Networks|HKUST| [[paper]](https://www.vldb.org/pvldb/vol15/p1937-peng.pdf)![Scholar citations](https://img.shields.io/badge/Citations-49-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/chenzhao/light-dist-gnn)![GitHub stars](https://img.shields.io/github/stars/chenzhao/light-dist-gnn.svg?logo=github&label=Stars)|
|MLSys 2022|BNS-GCN: Efficient Full-Graph Training of Graph Convolutional Networks with Partition-Parallelism and Random Boundary Node Sampling|Rice, UIUC| [[paper]](https://proceedings.mlsys.org/paper/2022/file/d1fe173d08e959397adf34b1d77e88d7-Paper.pdf)![Scholar citations](https://img.shields.io/badge/Citations-53-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/RICE-EIC/BNS-GCN)![GitHub stars](https://img.shields.io/github/stars/RICE-EIC/BNS-GCN.svg?logo=github&label=Stars)|
|MLSys 2022|Sequential Aggregation and Rematerialization: Distributed Full-batch Training of Graph Neural Networks on Large Graphs|Intel| [[paper]](https://arxiv.org/abs/2111.06483)![Scholar citations](https://img.shields.io/badge/Citations-19-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/IntelLabs/SAR)![GitHub stars](https://img.shields.io/github/stars/IntelLabs/SAR.svg?logo=github&label=Stars)|
|WWW 2022|PaSca: A Graph Neural Architecture Search System under the Scalable Paradigm|PKU| [[paper]](https://dl.acm.org/doi/abs/10.1145/3485447.3511986)![Scholar citations](https://img.shields.io/badge/Citations-42-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|ICLR 2022|PipeGCN: Efficient Full-Graph Training of Graph Convolutional Networks with Pipelined Feature Communication|Rice| [[paper]](https://openreview.net/pdf?id=kSwqMH0zn1F)![Scholar citations](https://img.shields.io/badge/Citations-55-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/RICE-EIC/PipeGCN)![GitHub stars](https://img.shields.io/github/stars/RICE-EIC/PipeGCN.svg?logo=github&label=Stars)|
|ICLR 2022|Learn Locally, Correct Globally: A Distributed Algorithm for Training Graph Neural Networks|PSU| [[paper]](https://openreview.net/pdf?id=FndDxSz3LxQ)![Scholar citations](https://img.shields.io/badge/Citations-26-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/MortezaRamezani/llcg)![GitHub stars](https://img.shields.io/github/stars/MortezaRamezani/llcg.svg?logo=github&label=Stars)|
|arXiv 2021|Distributed Hybrid CPU and GPU training for Graph Neural Networks on Billion-Scale Graphs|AWS| [[paper]](https://arxiv.org/pdf/2112.15345.pdf)![Scholar citations](https://img.shields.io/badge/Citations-24-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|SC 2021|DistGNN: Scalable Distributed Training for Large-Scale Graph Neural Networks|Intel| [[paper]](https://dl.acm.org/doi/pdf/10.1145/3458817.3480856)![Scholar citations](https://img.shields.io/badge/Citations-103-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/dmlc/dgl/pull/3024)|
|SC 2021|Efficient Scaling of Dynamic Graph Neural Networks|IBM| [[paper]](https://dl.acm.org/doi/pdf/10.1145/3458817.3480858)![Scholar citations](https://img.shields.io/badge/Citations-19-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|CLUSTER 2021|2PGraph: Accelerating GNN Training over Large Graphs on GPU Clusters|NUDT| [[paper]](https://ieeexplore.ieee.org/abstract/document/9556026)![Scholar citations](https://img.shields.io/badge/Citations-15-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|OSDI 2021|$P^3$: Distributed Deep Graph Learning at Scale|MSR| [[paper]](https://www.usenix.org/system/files/osdi21-gandhi.pdf)![Scholar citations](https://img.shields.io/badge/Citations-126-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|OSDI 2021|Dorylus: Affordable, Scalable, and Accurate GNN Training with Distributed CPU Servers and Serverless Threads|UCLA| [[paper]](http://web.cs.ucla.edu/~harryxu/papers/dorylus-osdi21.pdf)![Scholar citations](https://img.shields.io/badge/Citations-122-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/uclasystem/dorylus)![GitHub stars](https://img.shields.io/github/stars/uclasystem/dorylus.svg?logo=github&label=Stars)|
|arXiv 2021|GIST: Distributed Training for Large-Scale Graph Convolutional Networks|Rice| [[paper]](https://arxiv.org/abs/2102.10424)![Scholar citations](https://img.shields.io/badge/Citations-12-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|EuroSys 2021|FlexGraph: A Flexible and Efficient Distributed Framework for GNN Training|Alibaba| [[paper]](https://dl.acm.org/doi/pdf/10.1145/3447786.3456229)![Scholar citations](https://img.shields.io/badge/Citations-47-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|EuroSys 2021|DGCL: An Efficient Communication Library for Distributed GNN Training|CUHK| [[paper]](https://dl.acm.org/doi/abs/10.1145/3447786.3456233)![Scholar citations](https://img.shields.io/badge/Citations-68-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/czkkkkkk/ragdoll)![GitHub stars](https://img.shields.io/github/stars/czkkkkkk/ragdoll.svg?logo=github&label=Stars)|
|SC 2020|Reducing Communication in Graph Neural Network Training|UC Berkeley| [[paper]](https://arxiv.org/pdf/2005.03300.pdf)![Scholar citations](https://img.shields.io/badge/Citations-101-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/PASSIONLab/CAGNET)![GitHub stars](https://img.shields.io/github/stars/PASSIONLab/CAGNET.svg?logo=github&label=Stars)|
|VLDB 2020|G$^3$: When Graph Neural Networks Meet Parallel Graph Processing Systems on GPUs|NUS| [[paper]](http://www.vldb.org/pvldb/vol13/p2813-liu.pdf)![Scholar citations](https://img.shields.io/badge/Citations-44-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/Xtra-Computing/G3)![GitHub stars](https://img.shields.io/github/stars/Xtra-Computing/G3.svg?logo=github&label=Stars)|
|IA3 2020|DistDGL: Distributed Graph Neural Network Training for Billion-Scale Graphs|AWS| [[paper]](https://arxiv.org/pdf/2010.05337.pdf)![Scholar citations](https://img.shields.io/badge/Citations-112-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/dmlc/dgl/tree/master/python/dgl/distributed)|
|MLSys 2020|Improving the Accuracy, Scalability, and Performance of Graph Neural Networks with Roc|Stanford| [[paper]](https://proceedings.mlsys.org/paper/2020/file/fe9fc289c3ff0af142b6d3bead98a923-Paper.pdf)![Scholar citations](https://img.shields.io/badge/Citations-208-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/jiazhihao/ROC)![GitHub stars](https://img.shields.io/github/stars/jiazhihao/ROC.svg?logo=github&label=Stars)|
|arXiv 2020|AGL: A Scalable System for Industrial-purpose Graph Machine Learning|Ant Financial Services Group| [[paper]](https://arxiv.org/abs/2003.02454)![Scholar citations](https://img.shields.io/badge/Citations-113-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|ATC 2019|NeuGraph: Parallel Deep Neural Network Computation on Large Graphs|PKU| [[paper]](https://www.usenix.org/system/files/atc19-ma_0.pdf)![Scholar citations](https://img.shields.io/badge/Citations-247-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
### Training Systems for Scaling Graphs
| Venue | Title | Affiliation | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Link&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;Source&nbsp;&nbsp; |
| :---: | :---: | :---------: | :---: | :----: |
|EuroSys 2023|MariusGNN: Resource-Efficient Out-of-Core Training of Graph Neural Networks|UW–Madison| [[paper]](https://arxiv.org/abs/2202.02365)![Scholar citations](https://img.shields.io/badge/Citations-24-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/marius-team/marius)![GitHub stars](https://img.shields.io/github/stars/marius-team/marius.svg?logo=github&label=Stars)|
|VLDB 2022|ByteGNN: Efficient Graph Neural Network Training at Large Scale|ByteDance| [[paper]](https://dl.acm.org/doi/abs/10.14778/3514061.3514069)![Scholar citations](https://img.shields.io/badge/Citations-57-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|ICML 2022|GraphFM: Improving Large-Scale GNN Training via Feature Momentum|TAMU| [[paper]](https://arxiv.org/abs/2206.07161)![Scholar citations](https://img.shields.io/badge/Citations-24-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/divelab/DIG/tree/dig-stable/dig/lsgraph)|
|ICML 2021|GNNAutoScale: Scalable and Expressive Graph Neural Networks via Historical Embeddings|TU Dortmund University| [[paper]](https://arxiv.org/abs/2106.05609)![Scholar citations](https://img.shields.io/badge/Citations-138-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/rusty1s/pyg_autoscale)![GitHub stars](https://img.shields.io/github/stars/rusty1s/pyg_autoscale.svg?logo=github&label=Stars)|
|OSDI 2021|GNNAdvisor: An Adaptive and Efficient Runtime System for GNN Acceleration on GPUs|UCSB| [[paper]](https://www.usenix.org/system/files/osdi21-wang-yuke.pdf)![Scholar citations](https://img.shields.io/badge/Citations-135-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/YukeWang96/OSDI21_AE)![GitHub stars](https://img.shields.io/github/stars/YukeWang96/OSDI21_AE.svg?logo=github&label=Stars)|
### Quantized GNNs
| Venue | Title | Affiliation | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Link&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;Source&nbsp;&nbsp; |
| :---: | :---: | :---------: | :---: | :----: |
|Neurocomputing 2022|EPQuant: A Graph Neural Network Compression Approach Based on Product Quantization|ZJU| [[paper]](https://www.sciencedirect.com/science/article/abs/pii/S0925231222008293)![Scholar citations](https://img.shields.io/badge/Citations-8-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/Lyun-Huang/EPQuant)![GitHub stars](https://img.shields.io/github/stars/Lyun-Huang/EPQuant.svg?logo=github&label=Stars)|
|ICLR 2022|EXACT: Scalable Graph Neural Networks Training via Extreme Activation Compression|Rice| [[paper]](https://openreview.net/pdf?id=vkaMaq95_rX)![Scholar citations](https://img.shields.io/badge/Citations-52-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/warai-0toko/Exact)![GitHub stars](https://img.shields.io/github/stars/warai-0toko/Exact.svg?logo=github&label=Stars)|
|PPoPP 2022|QGTC: Accelerating Quantized Graph Neural Networks via GPU Tensor Core|UCSB| [[paper]](https://arxiv.org/abs/2111.09547)![Scholar citations](https://img.shields.io/badge/Citations-37-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/YukeWang96/PPoPP22_QGTC)![GitHub stars](https://img.shields.io/github/stars/YukeWang96/PPoPP22_QGTC.svg?logo=github&label=Stars)|
|CVPR 2021|Binary Graph Neural Networks|ICL| [[paper]](https://arxiv.org/abs/2012.15823)![Scholar citations](https://img.shields.io/badge/Citations-50-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/mbahri/binary_gnn)![GitHub stars](https://img.shields.io/github/stars/mbahri/binary_gnn.svg?logo=github&label=Stars)|
|CVPR 2021|Bi-GCN: Binary Graph Convolutional Network|Beihang University| [[paper]](https://openaccess.thecvf.com/content/CVPR2021/html/Wang_Bi-GCN_Binary_Graph_Convolutional_Network_CVPR_2021_paper.html)![Scholar citations](https://img.shields.io/badge/Citations-50-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/bywmm/Bi-GCN)![GitHub stars](https://img.shields.io/github/stars/bywmm/Bi-GCN.svg?logo=github&label=Stars)|
|EuroMLSys 2021|Learned Low Precision Graph Neural Networks|Cambridge| [[paper]](https://arxiv.org/abs/2009.09232)![Scholar citations](https://img.shields.io/badge/Citations-33-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|World Wide Web 2021|Binarized Graph Neural Network|UTS| [[paper]](https://arxiv.org/pdf/2004.11147.pdf)![Scholar citations](https://img.shields.io/badge/Citations-29-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|ICLR 2021|Degree-Quant: Quantization-Aware Training for Graph Neural Networks|Cambridge| [[paper]](https://arxiv.org/abs/2008.05000)![Scholar citations](https://img.shields.io/badge/Citations-151-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/camlsys/degree-quant)![GitHub stars](https://img.shields.io/github/stars/camlsys/degree-quant.svg?logo=github&label=Stars)|
|ICTAI 2020|SGQuant: Squeezing the Last Bit on Graph Neural Networks with Specialized Quantization|UCSB| [[paper]](https://ieeexplore.ieee.org/abstract/document/9288186/)![Scholar citations](https://img.shields.io/badge/Citations-41-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/YukeWang96/SGQuant)![GitHub stars](https://img.shields.io/github/stars/YukeWang96/SGQuant.svg?logo=github&label=Stars)|
### GNN Dataloaders
| Venue | Title | Affiliation | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Link&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;Source&nbsp;&nbsp; |
| :---: | :---: | :---------: | :---: | :----: |
|NSDI 2023|BGL: GPU-Efficient GNN Training by Optimizing Graph Data I/O and Preprocessing|ByteDance| [[paper]](https://arxiv.org/abs/2112.08541)![Scholar citations](https://img.shields.io/badge/Citations-50-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|MLSys 2022|Accelerating Training and Inference of Graph Neural Networks with Fast Sampling and Pipelining|MIT| [[paper]](https://proceedings.mlsys.org/paper/2022/file/35f4a8d465e6e1edc05f3d8ab658c551-Paper.pdf)![Scholar citations](https://img.shields.io/badge/Citations-43-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/MITIBMxGraph/SALIENT)![GitHub stars](https://img.shields.io/github/stars/MITIBMxGraph/SALIENT.svg?logo=github&label=Stars)|
|EuroSys 2022|GNNLab: A Factored System for Sample-based GNN Training over GPUs|SJTU| [[paper]](https://dl.acm.org/doi/abs/10.1145/3492321.3519557)![Scholar citations](https://img.shields.io/badge/Citations-58-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/SJTU-IPADS/gnnlab)![GitHub stars](https://img.shields.io/github/stars/SJTU-IPADS/gnnlab.svg?logo=github&label=Stars)|
|KDD 2021|Global Neighbor Sampling for Mixed CPU-GPU Training on Giant Graphs|UCLA| [[paper]](https://arxiv.org/pdf/2106.06150.pdf)![Scholar citations](https://img.shields.io/badge/Citations-29-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|PPoPP 2021|Understanding and Bridging the Gaps in Current GNN Performance Optimizations|THU| [[paper]](https://dl.acm.org/doi/pdf/10.1145/3437801.3441585)![Scholar citations](https://img.shields.io/badge/Citations-69-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/xxcclong/GNN-Computing)![GitHub stars](https://img.shields.io/github/stars/xxcclong/GNN-Computing.svg?logo=github&label=Stars)|
|VLDB 2021|Large Graph Convolutional Network Training with GPU-Oriented Data Communication Architecture|UIUC| [[paper]](https://arxiv.org/abs/2103.03330)![Scholar citations](https://img.shields.io/badge/Citations-55-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/K-Wu/pytorch-direct_dgl)![GitHub stars](https://img.shields.io/github/stars/K-Wu/pytorch-direct_dgl.svg?logo=github&label=Stars)|
|TPDS 2021|Efficient Data Loader for Fast Sampling-Based GNN Training on Large Graphs|USTC| [[paper]](https://gnnsys.github.io/papers/GNNSys21_paper_8.pdf)![Scholar citations](https://img.shields.io/badge/Citations-28-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/zhiqi-0/PaGraph)![GitHub stars](https://img.shields.io/github/stars/zhiqi-0/PaGraph.svg?logo=github&label=Stars)|
|SoCC 2020|PaGraph: Scaling GNN Training on Large Graphs via Computation-aware Caching|USTC| [[paper]](https://dl.acm.org/doi/pdf/10.1145/3419111.3421281)![Scholar citations](https://img.shields.io/badge/Citations-125-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/zhiqi-0/PaGraph)![GitHub stars](https://img.shields.io/github/stars/zhiqi-0/PaGraph.svg?logo=github&label=Stars)|
|arXiv 2019|TigerGraph: A Native MPP Graph Database|UCSD| [[paper]](https://arxiv.org/pdf/1901.08248.pdf)![Scholar citations](https://img.shields.io/badge/Citations-67-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
### GNN Training Accelerators
| Venue | Title | Affiliation | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Link&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;Source&nbsp;&nbsp; |
| :---: | :---: | :---------: | :---: | :----: |
|ISCA 2022|Graphite: Optimizing Graph Neural Networks on CPUs Through Cooperative Software-Hardware Techniques|UIUC| [[paper]](http://iacoma.cs.uiuc.edu/iacoma-papers/isca22.pdf)![Scholar citations](https://img.shields.io/badge/Citations-23-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|ISCA 2022|Hyperscale FPGA-as-a-service architecture for large-scale distributed graph neural network|Alibaba| [[paper]](https://dl.acm.org/doi/abs/10.1145/3470496.3527439)![Scholar citations](https://img.shields.io/badge/Citations-18-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|arXiv 2021|GCNear: A Hybrid Architecture for Efficient GCN Training with Near-Memory Processing|PKU| [[paper]](https://arxiv.org/abs/2111.00680)![Scholar citations](https://img.shields.io/badge/Citations-10-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|DATE 2021|ReGraphX: NoC-enabled 3D Heterogeneous ReRAM Architecture for Training Graph Neural Networks|WSU| [[paper]](https://arxiv.org/abs/2102.07959)![Scholar citations](https://img.shields.io/badge/Citations-31-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|TCAD 2021|Rubik: A Hierarchical Architecture for Efficient Graph Learning|Chinese Academy of Sciences| [[paper]](https://arxiv.org/pdf/2009.12495.pdf)![Scholar citations](https://img.shields.io/badge/Citations-11-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|FPGA 2020|GraphACT: Accelerating GCN Training on CPU-FPGA Heterogeneous Platforms|USC| [[paper]](https://dl.acm.org/doi/pdf/10.1145/3373087.3375312)![Scholar citations](https://img.shields.io/badge/Citations-130-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/GraphSAINT/GraphACT)![GitHub stars](https://img.shields.io/github/stars/GraphSAINT/GraphACT.svg?logo=github&label=Stars)|
### GNN Inference Accelerators
| Venue | Title | Affiliation | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Link&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;Source&nbsp;&nbsp; |
| :---: | :---: | :---------: | :---: | :----: |
|JAIHC 2022|DRGN: a dynamically reconfigurable accelerator for graph neural networks|XJTU| [[paper]](https://link.springer.com/article/10.1007/s12652-022-04402-x)![Scholar citations](https://img.shields.io/badge/Citations-1-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|DAC 2022|GNNIE: GNN Inference Engine with Load-balancing and Graph-specific Caching|UMN| [[paper]](https://arxiv.org/abs/2105.10554)![Scholar citations](https://img.shields.io/badge/Citations-13-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|IPDPS 2022|Understanding the Design Space of Sparse/Dense Multiphase Dataflows for Mapping Graph Neural Networks on Spatial Accelerators|GaTech| [[paper]](https://arxiv.org/abs/2103.07977)![Scholar citations](https://img.shields.io/badge/Citations-8-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/stonne-simulator/omega)![GitHub stars](https://img.shields.io/github/stars/stonne-simulator/omega.svg?logo=github&label=Stars)|
|arXiv 2022|FlowGNN: A Dataflow Architecture for Universal Graph Neural Network Inference via Multi-Queue Streaming|GaTech| [[paper]](https://arxiv.org/abs/2204.13103)![Scholar citations](https://img.shields.io/badge/Citations-11-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|CICC 2022|StreamGCN: Accelerating Graph Convolutional Networks with Streaming Processing|UCLA| [[paper]](https://web.cs.ucla.edu/~atefehsz/publication/StreamGCN-CICC22.pdf)![Scholar citations](https://img.shields.io/badge/Citations-4-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|HPCA 2022|Accelerating Graph Convolutional Networks Using Crossbar-based Processing-In-Memory Architectures|HUST| [[paper]](https://ieeexplore.ieee.org/document/9773267)![Scholar citations](https://img.shields.io/badge/Citations-31-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|HPCA 2022|GCoD: Graph Convolutional Network Acceleration via Dedicated Algorithm and Accelerator Co-Design|Rice, PNNL| [[paper]](https://arxiv.org/abs/2112.11594)![Scholar citations](https://img.shields.io/badge/Citations-41-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)| [[code]](https://github.com/RICE-EIC/GCoD)![GitHub stars](https://img.shields.io/github/stars/RICE-EIC/GCoD.svg?logo=github&label=Stars)|
|arXiv 2022|GenGNN: A Generic FPGA Framework for Graph Neural Network Acceleration|GaTech| [[paper]](https://arxiv.org/abs/2201.08475)![Scholar citations](https://img.shields.io/badge/Citations-12-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|DAC 2021|DyGNN: Algorithm and Architecture Support of vertex Dynamic Pruning for Graph Neural Networks|Hunan University| [[paper]](https://ieeexplore.ieee.org/document/9586298)![Scholar citations](https://img.shields.io/badge/Citations-24-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|DAC 2021|BlockGNN: Towards Efficient GNN Acceleration Using Block-Circulant Weight Matrices|PKU| [[paper]](https://arxiv.org/abs/2104.06214)![Scholar citations](https://img.shields.io/badge/Citations-28-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|DAC 2021|TARe: Task-Adaptive in-situ ReRAM Computing for Graph Learning|Chinese Academy of Sciences| [[paper]](https://ieeexplore.ieee.org/abstract/document/9586193)![Scholar citations](https://img.shields.io/badge/Citations-13-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|ICCAD 2021|G-CoS: GNN-Accelerator Co-Search Towards Both Better Accuracy and Efficiency|Rice| [[paper]](https://arxiv.org/abs/2109.08983)![Scholar citations](https://img.shields.io/badge/Citations-25-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|MICRO 2021|I-GCN: A Graph Convolutional Network Accelerator with Runtime Locality Enhancement through Islandization|PNNL| [[paper]](https://dl.acm.org/doi/pdf/10.1145/3466752.3480113)![Scholar citations](https://img.shields.io/badge/Citations-88-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|arXiv 2021|ZIPPER: Exploiting Tile- and Operator-level Parallelism for General and Scalable Graph Neural Network Acceleration|SJTU| [[paper]](https://arxiv.org/abs/2107.08709)![Scholar citations](https://img.shields.io/badge/Citations-4-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|TComp 2021|EnGN: A High-Throughput and Energy-Efficient Accelerator for Large Graph Neural Networks|Chinese Academy of Sciences| [[paper]](https://arxiv.org/abs/1909.00155)![Scholar citations](https://img.shields.io/badge/Citations-165-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|HPCA 2021|GCNAX: A Flexible and Energy-efficient Accelerator for Graph Convolutional Neural Networks|GWU| [[paper]](https://ieeexplore.ieee.org/abstract/document/9407104)![Scholar citations](https://img.shields.io/badge/Citations-115-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|APA 2020|GNN-PIM: A Processing-in-Memory Architecture for Graph Neural Networks|PKU| [[paper]](http://115.27.240.201/docs/20200915165942122459.pdf)![Scholar citations](https://img.shields.io/badge/Citations-19-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|ASAP 2020|Hardware Acceleration of Large Scale GCN Inference|USC| [[paper]](https://ieeexplore.ieee.org/document/9153263)![Scholar citations](https://img.shields.io/badge/Citations-72-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|DAC 2020|Hardware Acceleration of Graph Neural Networks|UIUC| [[paper]](http://rakeshk.web.engr.illinois.edu/dac20.pdf)![Scholar citations](https://img.shields.io/badge/Citations-122-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|MICRO 2020|AWB-GCN: A Graph Convolutional Network Accelerator with Runtime Workload Rebalancing|PNNL| [[paper]](https://ieeexplore.ieee.org/abstract/document/9252000)![Scholar citations](https://img.shields.io/badge/Citations-245-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|arXiv 2020|GRIP: A Graph Neural Network Accelerator Architecture|Stanford| [[paper]](https://arxiv.org/pdf/2007.13828.pdf)![Scholar citations](https://img.shields.io/badge/Citations-83-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
|HPCA 2020|HyGCN: A GCN Accelerator with Hybrid Architecture|UCSB| [[paper]](https://arxiv.org/pdf/2001.02514.pdf)![Scholar citations](https://img.shields.io/badge/Citations-299-_.svg?logo=google-scholar&labelColor=4f4f4f&color=3388ee)||
## Contribute

We welcome contributions to [this repository](https://github.com/chwan1016/awesome-gnn-systems). To add new papers to this list, please update JSON files under `./res/papers/`. Our bots will update the paper list in `README.md` automatically. The citations of newly added papers will be updated within one day.
