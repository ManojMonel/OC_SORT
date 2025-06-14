# OC-SORT

[![arXiv](https://img.shields.io/badge/arXiv-2203.14360-<COLOR>.svg)](https://arxiv.org/abs/2203.14360) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) ![test](https://img.shields.io/static/v1?label=By&message=Pytorch&color=red)

**Observation-Centric SORT (OC-SORT)** is a pure motion-model-based multi-object tracker. It aims to improve tracking robustness in **crowded scenes and when objects are in non-linear motion**. It is designed by recognizing and fixing limitations in Kalman filter and [SORT](https://arxiv.org/abs/1602.00763). It is flexible to integrate with different detectors and matching modules, such as appearance similarity. It remains, **Simple, Online and Real-time**.

### Pipeline
<center>
<img src="assets/teaser.png" width="600"/>
</center>


### Observation-centric Re-Update 
<center>
<img src="assets/ocr.png" width="600"/>
</center>



## Benchmark Performance

[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/observation-centric-sort-rethinking-sort-for/multi-object-tracking-on-dancetrack)](https://paperswithcode.com/sota/multi-object-tracking-on-dancetrack?p=observation-centric-sort-rethinking-sort-for) 
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/observation-centric-sort-rethinking-sort-for/multiple-object-tracking-on-kitti-tracking)](https://paperswithcode.com/sota/multiple-object-tracking-on-kitti-tracking?p=observation-centric-sort-rethinking-sort-for)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/observation-centric-sort-rethinking-sort-for/multi-object-tracking-on-mot17)](https://paperswithcode.com/sota/multi-object-tracking-on-mot17?p=observation-centric-sort-rethinking-sort-for) 
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/observation-centric-sort-rethinking-sort-for/multi-object-tracking-on-mot20-1)](https://paperswithcode.com/sota/multi-object-tracking-on-mot20-1?p=observation-centric-sort-rethinking-sort-for) 
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/observation-centric-sort-rethinking-sort-for/multiple-object-tracking-on-crohd)](https://paperswithcode.com/sota/multiple-object-tracking-on-crohd?p=observation-centric-sort-rethinking-sort-for)






If you find this work useful, please consider to cite our paper:
```
@inproceedings{cao2023observation,
  title={Observation-centric sort: Rethinking sort for robust multi-object tracking},
  author={Cao, Jinkun and Pang, Jiangmiao and Weng, Xinshuo and Khirodkar, Rawal and Kitani, Kris},
  booktitle={Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition},
  pages={9686--9696},
  year={2023}
}
```
