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


| Dataset          | HOTA | AssA | IDF1 | MOTA | FP      | FN      | IDs   | Frag   |
| ---------------- | ---- | ---- | ---- | ---- | ------- | ------- | ----- | ------ |
| MOT17 (private)  | 63.2 | 63.2 | 77.5 | 78.0 | 15,129  | 107,055 | 1,950 | 2,040  |
| MOT17 (public)   | 52.4 | 57.6 | 65.1 | 58.2 | 4,379   | 230,449 | 784   | 2,006  |
| MOT20 (private)  | 62.4 | 62.5 | 76.4 | 75.9 | 20,218  | 103,791 | 938   | 1,004  |
| MOT20 (public)   | 54.3 | 59.5 | 67.0 | 59.9 | 4,434   | 202,502 | 554   | 2,345  |
| KITTI-cars       | 76.5 | 76.4 | -    | 90.3 | 2,685   | 407     | 250   | 280    |
| KITTI-pedestrian | 54.7 | 59.1 | -    | 65.1 | 6,422   | 1,443   | 204   | 609    |
| DanceTrack-test  | 55.1 | 38.0 | 54.2 | 89.4 | 114,107 | 139,083 | 1,992 | 3,838  |
| CroHD HeadTrack  | 44.1 | -    | 62.9 | 67.9 | 102,050 | 164,090 | 4,243 | 10,122 |

* Results are from reusing detections of previous methods and shared hyper-parameters. Tune the implementation adaptive to datasets may get higher performance.
* The inference speed is ~28FPS by a RTX 2080Ti GPU. If the detections are provided, the inference speed of OC-SORT association is 700FPS by a i9-3.0GHz CPU.
* A sample from DanceTrack-test set is as below and more visualizatiosn are available on [Google Drive](https://drive.google.com/drive/folders/1-T4jhHwhOAp42DGJ115yMlC7CkB-PNxy?usp=sharing)

    ![](assets/dancetrack0088_slow.gif)





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
