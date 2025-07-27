---
layout: distill
title: Single Image Portrait Relighting via Explicit Multiple Reflectance Channel Modeling
img: /assets/img/Publications/SA20_FLM.gif
authors:
  - name: Zhibo Wang
    affiliations:
      name: BNRist and School of Software, Tsinghua University.
  - name: Xin Yu
    url: "https://sites.google.com/view/xinyus-homepage/Home"
    affiliations:
      name: Australian National University
  - name: Ming Lu
    affiliations:
      name: Intel Labs, China
  - name: Quan Wang
    affiliations:
      name: Sensetime
  - name: Chen Qian
    url: "https://scholar.google.com/citations?user=AerkT0YAAAAJ&hl="
    affiliations:
      name: Sensetime
  - name: Feng Xu
    url: "http://xufeng.site/"
    affiliations:
      name: BNRist and School of Software, Tsinghua University
date: 2020-12-01
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/Publications/SA20_FLM_teaser.png' | relative_url }}" alt="" title="teaser image"/>
    </div>
</div>
<div class="caption">
    Relit results of our system. Our method outperforms [Zhou et.al 2019]<d-cite key="zhou2019deep"></d-cite> and [Sun et.al 2019]<d-cite key="sun2019single"></d-cite> and generates visually pleasing specular and shadow effect.
</div>

## Abstract

Portrait relighting aims to render a face image under different lighting conditions. Existing methods do not explicitly consider some challenging lighting effects such as specular and shadow, and thus may fail in handling extreme lighting conditions. In this paper, we propose a novel framework that explicitly models multiple reflectance channels for single image portrait relighting, including the facial albedo, geometry as well as two lighting effects, i.e., specular and shadow. These channels are finally composed to generate the relit results via deep neural networks. Current datasets do not support learning such multiple reflectance channel modeling. Therefore, we present a large-scale dataset with the ground-truths of the channels, enabling us to train the deep neural networks in a supervised manner. Furthermore, we develop a novel module named Lighting guided Feature Modulation (LFM). In contrast to existing methods which simply incorporate the given lighting in the bottleneck of a network, LFM fuses the lighting by layer-wise feature modulation to deliver more convincing results. Extensive experiments demonstrate that our proposed method achieves better results and is able to generate challenging lighting effects.

---

## Resources and Downloads

| Paper | Supplementary  | Video |
|:-:|:-:|:-:|
|<a href="{{ 'SA20_220-276_paper.pdf' | prepend: '/assets/pdf/' | relative_url }}" target="_blank"><span style="font-size: 3em; color: Tomato;"><i class="fas fa-file-pdf"></i></span></a>|<a href="{{ 'SA20_220-276_supplementary.pdf' | prepend: '/assets/pdf/' | relative_url }}" target="_blank"><span style="font-size: 3em; color: Tomato;"><i class="fas fa-file-pdf"></i></span></a>|<a href="https://drive.google.com/file/d/1tNNEHSpNJmdh25Bj4IzMLJ4Q93q_gbwL/view?usp=sharing" target="_blank"><span style="font-size: 3em; color: blueviolet;"><i class="fas fa-file-video"></i></span></a>|

## Dataset

Our dataset is available for academic research. To acquire this dataset, please download this <a href="{{ 'MRCD_Dataset_Agreement.pdf' | prepend: '/assets/pdf/' | relative_url }}" target="_blank">**agreement**</a>, read it carefully and send it back to <a href="mailto:{{ site.email | encode_email }}">**us**</a> with the signature of the director of your school or your institution. For copyright protection, we only accept the application from the director of your school or your institution.

Our dataset includes the facial scans of 438 subjects. For each subject, we capture 20 expressions. The synthetic relighting dataset is rendered using the scans of 100 subjects, which includes 270,000 valid image groups for training and 20,00 valid image groups for testing. 

> Some data is still under the examinations in SenseTime. Currently, we can provide the scans of 270 subjects. The relighting dataset includes the images of 80 subjects.
> 
> **As the agreement is based on the entire dataset, you do not need to sign the agreement again for the data released in the future.**

## Acknowledgements
This work was supported by the National Key R&D Program of China 2018YFA0704000, the NSFC (No.61822111, 61727808, 61671268) and Beijing Natural Science Foundation (JQ19015, L182052). Feng Xu is the corresponding author. The 3rd author (Ming Lu) waives his intellectual property rights of this work. We thank Tiancheng Sun for providing the relit results of the real images.

## Citation

```bibtex
@article{10.1145/3414685.3417824,
author = {Wang, Zhibo and Yu, Xin and Lu, Ming and Wang, Quan and Qian, Chen and Xu, Feng},
title = {Single Image Portrait Relighting via Explicit Multiple Reflectance Channel Modeling},
year = {2020},
issue_date = {December 2020},
publisher = {Association for Computing Machinery},
address = {New York, NY, USA},
volume = {39},
number = {6},
issn = {0730-0301},
doi = {10.1145/3414685.3417824},
journal = {ACM Trans. Graph.},
month = nov,
articleno = {220},
numpages = {13},
}
```