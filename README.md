# DECENT-niPGT
[![pytorch](https://img.shields.io/badge/PyTorch_2.0+-ee4c2c?logo=pytorch&logoColor=white)](https://pytorch.org/get-started/locally/)
[![license](https://img.shields.io/badge/License-MIT-green.svg?labelColor=gray)](https://github.com/zhenyiizhang/DECENT-niPGT/blob/main/LICENSE.txt)

DECENT-niPGT: Advancing maternal contamination removal and CNV reconstruction in noninvasive preimplantation genetic testing through deep learning

## Introduction
We present DECENT-niPGT (deep CNV reconstruction of niPGT), a novel deep learning framework aimed at mitigating maternal contamination in SECM and reconstructing embryonic copy number variations (CNVs). DECENT leverages sequence and methylation information from both embryonic and maternal sources, utilizing convolutional neural networks and attention mechanisms to infer the origin of sequence reads. Overall, DECENT contributes to substantially enhancing the diagnostic accuracy and effectiveness of SECM-based niPGT, establishing a robust groundwork for the extensive clinical utilization of niPGT in the field of reproductive medicine.

<p align="center">
  <img src=https://github.com/zhenyiizhang/DECENT-niPGT/blob/main/figures/main.svg alt="[main]">
</p>

## Get Started

Clone this repo:
```bash
git clone https://github.com/zhenyiizhang/DECENT-nipgt
cd DECENT-nipgt
```

- You can create a new ```conda```  environment (DECENT) using 
```bash
conda env create -f environment.yml
```

- In MAC OS, there's an issue with installing pysam-related packages. Below is alternative way to install in the conda environment:
```bash
conda env create -f environment_mac.yml
conda activate DECENT
pip install pysam
```

Both are also needed to install bedtools related packages, it's recommended to refer to [this source](https://bedtools.readthedocs.io/en/latest/content/installation.html) for more details.

If you want to conduct CNV analysis further, you should config [Ginkgo](https://github.com/robertaboukhalil/ginkgo) on your own server and then use our reference samples and scripts for analysis.

## License
DECENT-niPGT is licensed under the MIT License. However, any use of the patented technology implemented in this software for commercial purposes requires prior written approval from the patent holder. 



