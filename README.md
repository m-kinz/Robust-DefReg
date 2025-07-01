# Robust-DefReg: a robust coarse to fine non-rigid point cloud registration method based on graph convolutional neural networks [(Paper Link)](https://iopscience.iop.org/article/10.1088/1361-6501/ad916c/meta)

Point cloud registration is a critical process in computer vision and measurement science, aimed at determining transformations between corresponding sets of points for accurate spatial alignment. In particular, non-rigid registration involves estimating flexible transformations that map a source point cloud to a target point cloud, even under conditions of stretching, compression, or other complex deformations. This task becomes especially challenging when addressing measurement-specific issues like varying degrees of deformation, noise, and outliers, all of which can impact measurement accuracy and reliability. This paper introduces Robust-DefReg, a novel method for non-rigid point cloud registration that applies graph convolutional networks (GCNNs) within a coarse-to-fine registration framework. This end-to-end pipeline harnesses global feature learning to establish robust correspondences and precise transformations, enabling high accuracy across different deformation scales and noise levels. A key contribution of Robust-DefReg is its demonstrated resilience to various challenges, such as substantial deformations, noise, and outliers, factors often underreported in existing registration literature. In addition, we present SynBench, a comprehensive benchmark dataset specifically designed for evaluating non-rigid point cloud registration in realistic measurement scenarios. Unlike previous datasets, SynBench incorporates a range of challenges, making it a valuable tool for the fair assessment of registration methods in measurement applications. Experimental results on SynBench and additional datasets show that Robust-DefReg consistently outperforms state-of-the-art methods, offering higher registration accuracy and robustness, even with up to 45% outliers. 

# SynBench Dataset [(Data Link)](https://doi.org/10.11588/data/R9IKCF)
Despite the existence of several datasets for deformable point cloud registration, the absence of a comprehensive benchmark with all challenges makes it difficult to achieve fair evaluations among different methods. SynBench, a new non-rigid point cloud registration dataset created using SimTool—a toolset for soft body simulation in Flex and Unreal Engine. SynBench provides the ground truth of corresponding points between two point sets and encompasses key registration challenges, including varying levels of deformation, noise, outliers, and incompleteness. To the best of the authors’ knowledge, compared to existing datasets, SynBench possesses three particular characteristics: 1) it is the first benchmark that provides various challenges for non-rigid point cloud registration, 2) SynBench encompasses challenges of varying difficulty levels, 3) It includes ground truth corresponding points both before and after deformation. The authors believe that SynBench makes it possible for future non-rigid point cloud registration methods to present a fair comparison of their achievements. The SynBench is publicly available under https://doi.org/10.11588/data/R9IKCF.

# SimTool [(Paper Link)](https://www.sciencedirect.com/science/article/pii/S2665963823000581), [(Code Link)](https://github.com/m-kinz/SimTool)
SynBench dataset is created using SimTool — a toolset for soft body simulation in Flex and Unreal Engine. 


# Citation
**If you use Robust-DefReg code, please cite:**

@article{monji2024robust,<br />
  title={Robust-DefReg: a robust coarse to fine non-rigid point cloud registration method based on graph convolutional neural networks},<br />
  author={Monji-Azad, Sara and Kinz, Marvin and M{\"a}nnel, David and Scherl, Claudia and Hesser, J{\"u}rgen},<br />
  journal={Measurement Science and Technology},<br />
  volume={36},<br />
  number={1},<br />
  pages={015426},<br />
  year={2024},<br />
  publisher={IOP Publishing}<br />
}

**If you use SynBench Dataset please cite both the paper and data:** <br />

@article{monji2024robust,<br />
  title={Robust-DefReg: a robust coarse to fine non-rigid point cloud registration method based on graph convolutional neural networks},<br />
  author={Monji-Azad, Sara and Kinz, Marvin and M{\"a}nnel, David and Scherl, Claudia and Hesser, J{\"u}rgen},<br />
  journal={Measurement Science and Technology},<br />
  volume={36},<br />
  number={1},<br />
  pages={015426},<br />
  year={2024},<br />
  publisher={IOP Publishing}<br />
}

@data{data/R9IKCF_2023,<br />
author = {Marvin Kinz},<br />
publisher = {heiDATA},<br />
title = {{SimTool-SynBench}},<br />
year = {2023},<br />
version = {V2},<br />
doi = {10.11588/data/R9IKCF},<br />
url = {https://doi.org/10.11588/data/R9IKCF}<br />
}

**If you use SimTool, please cite:**

@article{monji2023simtool,<br />
  title={SimTool: A toolset for soft body simulation using Flex and Unreal Engine},<br />
  author={Monji-Azad, Sara and Kinz, Marvin and Hesser, J{\"u}rgen and L{\"o}w, Nikolas},<br />
  journal={Software Impacts},<br />
  volume={17},<br />
  pages={100521},<br />
  year={2023},<br />
  publisher={Elsevier}<br />
}

