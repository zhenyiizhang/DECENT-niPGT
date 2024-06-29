# DECENT-niPGT
[![pytorch](https://img.shields.io/badge/PyTorch_1.8+-ee4c2c?logo=pytorch&logoColor=white)](https://pytorch.org/get-started/locally/)
[![license](https://img.shields.io/badge/License-MIT-green.svg?labelColor=gray)](https://github.com/zhenyiizhang/DECENT-niPGT/blob/main/LICENSE.txt)

## Introduction
We present DECENT-niPGT (deep CNV reconstruction of niPGT), a novel deep learning framework aimed at mitigating maternal contamination in SECM and reconstructing embryonic copy number variations (CNVs). DECENT leverages sequence and methylation information from both embryonic and maternal sources, utilizing convolutional neural networks and attention mechanisms to infer the origin of sequence reads. Overall, DECENT contributes to substantially enhancing the diagnostic accuracy and effectiveness of SECM-based niPGT, establishing a robust groundwork for the extensive clinical utilization of niPGT in the field of reproductive medicine.

<p align="center">
  <img src=https://github.com/zhenyiizhang/DECENT-niPGT/blob/main/figures/main.svg alt="[main]">
</p>

## Get Started

- For the ```conda``` users, you can create a new conda environment (DECENT) using 
```bash
conda env create -f environment.yml
```

- In MAC OS, there's an issue with installing pysam-related packages. Below is alternative way to install in a seprate conda environment:
```bash
conda env create -f environment_mac.yml
conda activate DECENT
pip install pysam
```

Then both are also needed to install bedtools related packages, it's recommended to refer to [here](https://bedtools.readthedocs.io/en/latest/content/installation.html).