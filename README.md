# PatchScaler: An Efficient Patch-independent Diffusion Model for Image Super-Resolution
[Yong Liu](https://scholar.google.com/citations?user=DT0LPIEAAAAJ&hl=en&oi=sra), 
[Hang Dong](https://scholar.google.com/citations?user=4DKepr8AAAAJ&hl=en&oi=sra), 
[Jinshan Pan](https://jspan.github.io/), 
Qingji Dong, 
Kai Chen, 
Rongxiang Zhang, 
Lean Fu, 
[Fei Wang](http://www.aiar.xjtu.edu.cn/info/1046/1242.htm)<br/>

:sparkling_heart: If our  PatchScaler is helpful to your researches or projects, please help star this repository. Thanks! :hugs: 

![visitors](https://visitor-badge.laobi.icu/badge?page_id=yongliuy/PatchScaler) 
<img alt="GitHub" src="https://img.shields.io/badge/license-Apache_2.0-brightgreen">
[![GitHub Stars](https://img.shields.io/github/stars/yongliuy/PatchScaler?style=social)](https://github.com/yongliuy/PatchScaler/)

>While diffusion models significantly improve the perceptual quality of super-resolved images, they usually require a large number of sampling steps, resulting in high computational costs and long inference times. 
Recent efforts have explored reasonable acceleration schemes by reducing the number of sampling steps. 
However, these approaches treat all regions of the image equally, overlooking the fact that regions with varying levels of reconstruction difficulty require different sampling steps. 
To address this limitation, we propose PatchScaler, an efficient patch-independent diffusion pipeline for single image super-resolution. 
Specifically, PatchScaler introduces a Patch-adaptive Group Sampling (PGS) strategy that groups feature patches by quantifying their reconstruction difficulty and establishes shortcut paths with different sampling configurations for each group. 
To further optimize the patch-level reconstruction process of PGS, we propose a texture prompt that provides rich texture conditional information to the diffusion model. 
The texture prompt adaptively retrieves texture priors for the target patch from a common reference texture memory. 
Extensive experiments show that our PatchScaler achieves superior performance in both quantitative and qualitative evaluations, while significantly speeding up inference. 
<p align="center">
<img src=assets/method.png width="1000px"/>
</p>

## :snowboarder: Update
- **2024.11.20**: Update lastest results.
- **2024.05.27**: Create this repository.


## :whale: License
This project is released under the [Apache 2.0 license](./LICENSE). Redistribution and use should follow this license.

## :trophy: Results on Real-world Image SR
<p align="center">
<img src=assets/results.png width="1000px"/>
</p>

## :star: BibTeX
If you find this project useful for your research, please use the following BibTeX entry.
```
@inproceedings{liu2024patchscaler,
  title={PatchScaler: An Efficient Patch-independent Diffusion Model for Super-Resolution},
  author={Yong Liu, Hang Dong, Jinshan Pan, Qingji Dong, Kai Chen, Rongxiang Zhang, Xing Mei, Lean Fu, and Fei Wang},
  year={2024}
}
```
