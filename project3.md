# 3D Teeth Scan Segmentation 


Implementation of [MeshSegNet: Deep Multi-Scale Mesh Feature Learning for Automated Labeling of Raw Dental Surface from 3D Intraoral Scanners](https://ieeexplore.ieee.org/abstract/document/8984309) [1] for automated tooth segmentation and labeling on raw dental surfaces. 
The dataset used for this project is the challenge 3DTeethSeg22 dataset (associated with MICCAI 2022) [2] and is publicly available.


<figure>
  <img src="./assets/images/project3/preds_vs_gt.gif" width="600" />
  <figcaption>Ground truth (left) vs. Predictions (right)</figcaption>
</figure>

## Code

The code is available on [![GitHub](https://i.stack.imgur.com/tskMh.png) GitHub](https://github.com/hippolytemayard/teeth-3d-mesh-segmentation)


## Dataset

The *3DTeethSeg22_challenge* dataset contains a collection of 3D dental surface scans obtained from intraoral scanners. These scans represent the raw dental surfaces of patients and serve as the input data for the segmentation task. The dataset includes a diverse range of dental conditions and variations, capturing different teeth shapes, sizes, and occlusions. A total of 1800 3D intra-oral scans have been collected for 900 patients covering their upper and lower jaws separately.


## Implementation Details

We base our implementation on MeshSegNet paper [1] as well as the official implementation (see [![GitHub](https://i.stack.imgur.com/tskMh.png) GitHub](https://github.com/Tai-Hsien/MeshSegNet/tree/master)).

<img src="./assets/images/project3/meshsegnet_architecture.png" width="800" />

## Training

- [] Monitoring model evaluation

## References 

[1] Tai-Hsien Wu, Chia-Jung Hsu, Sheng-Hong Huang, et al., "MeshSegNet: Deep Multi-Scale Mesh Feature Learning for Automated Labeling of Raw Dental Surface from 3D Intraoral Scanners," in IEEE Transactions on Medical Imaging, vol. 39, no. 4, pp. 945-956, April 2020. Available at: [Link](https://ieeexplore.ieee.org/abstract/document/8984309)


[2] "3DTeethSeg22_challenge: Dataset for the MICCAI 2022 3D Teeth Segmentation Challenge," GitHub repository, https://github.com/abenhamadou/3DTeethSeg22_challenge.

```
@article{ben20233dteethseg,
title={3DTeethSeg'22: 3D Teeth Scan Segmentation and Labeling Challenge},
author={Achraf Ben-Hamadou and Oussama Smaoui and Ahmed Rekik and Sergi Pujades and Edmond Boyer and Hoyeon Lim and Minchang Kim and Minkyung Lee and Minyoung Chung and Yeong-Gil Shin and Mathieu Leclercq and Lucia Cevidanes and Juan Carlos Prieto and Shaojie Zhuang and Guangshun Wei and Zhiming Cui and Yuanfeng Zhou and Tudor Dascalu and Bulat Ibragimov and Tae-Hoon Yong and Hong-Gi Ahn and Wan Kim and Jae-Hwan Han and Byungsun Choi and Niels van Nistelrooij and Steven Kempers and Shankeeth Vinayahalingam and Julien Strippoli and Aurélien Thollot and Hugo Setbon and Cyril Trosset and Edouard Ladroit},
journal={arXiv preprint arXiv:2305.18277},
year={2023}
}

@article{ben2022teeth3ds,
title={Teeth3DS: a benchmark for teeth segmentation and labeling from intra-oral 3D scans},
author={Ben-Hamadou, Achraf and Smaoui, Oussama and Chaabouni-Chouayakh, Houda and Rekik, Ahmed and Pujades, Sergi and Boyer, Edmond and Strippoli, Julien and Thollot, Aur{\'e}lien and Setbon, Hugo and Trosset, Cyril and others},
journal={arXiv preprint arXiv:2210.06094},
year={2022}
}
```