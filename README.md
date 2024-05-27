# PatchScaler: An Efficient Patch-independent Diffusion Model for Super-Resolution
[Yong Liu](https://scholar.google.com/citations?user=DT0LPIEAAAAJ&hl=en&oi=sra), 
[Hang Dong](https://scholar.google.com/citations?user=4DKepr8AAAAJ&hl=en&oi=sra), 
[Jinshan Pan](https://jspan.github.io/), 
Qingji Dong, 
Kai Chen, 
Rongxiang Zhang, 
Xing Mei, 
Lean Fu, 
[Fei Wang](http://www.aiar.xjtu.edu.cn/info/1046/1242.htm)<br/>

:sparkling_heart: If our  PatchScaler is helpful to your researches or projects, please help star this repository. Thanks! :hugs: 

![visitors](https://visitor-badge.laobi.icu/badge?page_id=yongliuy/PatchScaler) 
<img alt="GitHub" src="https://img.shields.io/badge/license-Apache_2.0-brightgreen">
[![GitHub Stars](https://img.shields.io/github/stars/yongliuy/PatchScaler?style=social)](https://github.com/yongliuy/PatchScaler/)

>Diffusion models significantly improve the quality of super-resolved images with their impressive content generation capabilities. However, the huge computational costs limit the applications of these methods.
Recent efforts have explored reasonable inference acceleration to reduce the number of sampling steps, but the computational cost remains high as each step is performed on the entire image. 
This paper introduces PatchScaler, a patch-independent diffusion-based single image super-resolution (SR) method, designed to enhance the efficiency of the inference process.
The proposed method is motivated by the observation that not all the image patches within an image need the same sampling steps for reconstructing high-resolution images. 
Based on this observation, we thus develop a Patch-adaptive Group Sampling (PGS) to divide feature patches into different groups according to the patch-level reconstruction difficulty and dynamically assign an appropriate sampling configuration for each group so that the inference speed can be better accelerated. 
In addition, to improve the denoising ability at each step of the sampling, we develop a texture prompt to guide the estimations of the diffusion model by retrieving high-quality texture priors from a patch-independent reference texture memory. 
Experiments show that our PatchScaler achieves favorable performance in both quantitative and qualitative evaluations with fast inference speed. 
<p align="center">
<img src=assets/method.png width="1000px"/>
</p>

## Update
- **2024.05.27**: Create this repository.

## Coming soon...
- [ ] New project website
- [ ] The training scripts
- [ ] Releasing pretrained models
- [ ] The inference scripts

## License
This project is released under the [Apache 2.0 license](./LICENSE). Redistribution and use should follow this license.


## BibTeX
If you find this project useful for your research, please use the following BibTeX entry.
```
@inproceedings{liu2024patchscaler,
  title={PatchScaler: An Efficient Patch-independent Diffusion Model for Super-Resolution},
  author={Yong Liu, Hang Dong, Jinshan Pan, Qingji Dong, Kai Chen, Rongxiang Zhang, Xing Mei, Lean Fu, and Fei Wang},
  year={2024}
}
```
