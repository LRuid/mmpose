<!-- [BACKBONE] -->

<details>
<summary align="right"><a href="https://arxiv.org/abs/2204.12484">ViTPose</a></summary>

```bibtex
@misc{https://doi.org/10.48550/arxiv.2204.12484,
  doi = {10.48550/ARXIV.2204.12484},
  url = {https://arxiv.org/abs/2204.12484},
  author = {Xu, Yufei and Zhang, Jing and Zhang, Qiming and Tao, Dacheng},
  keywords = {Computer Vision and Pattern Recognition (cs.CV), FOS: Computer and information sciences, FOS: Computer and information sciences},
  title = {ViTPose: Simple Vision Transformer Baselines for Human Pose Estimation},
  publisher = {arXiv},
  year = {2022},
  copyright = {arXiv.org perpetual, non-exclusive license}
}
```

</details>

<!-- [DATASET] -->

<details>
<summary align="right"><a href="https://link.springer.com/chapter/10.1007/978-3-030-58545-7_12">COCO-WholeBody (ECCV'2020)</a></summary>

```bibtex
@inproceedings{jin2020whole,
  title={Whole-Body Human Pose Estimation in the Wild},
  author={Jin, Sheng and Xu, Lumin and Xu, Jin and Wang, Can and Liu, Wentao and Qian, Chen and Ouyang, Wanli and Luo, Ping},
  booktitle={Proceedings of the European Conference on Computer Vision (ECCV)},
  year={2020}
}
```

</details>

Results on COCO val2017 with detector having human AP of 56.4 on COCO val2017 dataset

> With classic decoder

| Arch                                                                                                        | Input Size |  AP   | AP<sup>50</sup> | AP<sup>75</sup> |  AR   | AR<sup>50</sup> |   ckpt   |
| :---------------------------------------------------------------------------------------------------------- | :--------: | :---: | :-------------: | :-------------: | :---: | :-------------: | :------: |
| [ViTPose-S](/configs/body_2d_keypoint/topdown_heatmap/coco/td-hm_ViTPose-small_8xb64-210e_coco-256x192.py)  |  256x192   | 0.739 |      0.903      |      0.816      | 0.792 |      0.942      | \[ckpt\] |
| [ViTPose-B](/configs/body_2d_keypoint/topdown_heatmap/coco/td-hm_ViTPose-base_8xb64-210e_coco-256x192.py)   |  256x192   | 0.757 |      0.905      |      0.829      | 0.810 |      0.946      | \[ckpt\] |
| [ViTPose-L](/configs/body_2d_keypoint/topdown_heatmap/coco/td-hm_ViTPose-large_8xb64-210e_coco-256x192.py)  |  256x192   | 0.782 |      0.914      |      0.850      | 0.834 |      0.952      | \[ckpt\] |
| [ViTPose-H](/configs/body_2d_keypoint/topdown_heatmap/coco/td-hm_ViTPose-huge_8xb64-210e_coco-256x192.py)   |  256x192   | 0.788 |      0.917      |      0.855      | 0.839 |      0.954      | \[ckpt\] |
| [ViTPose-H\*](/configs/body_2d_keypoint/topdown_heatmap/coco/td-hm_ViTPose-huge_8xb64-210e_coco-256x192.py) |  256x192   | 0.790 |     0.0.916     |      0.857      | 0.840 |      0.953      | \[ckpt\] |

*Models with * are converted from the [official repo](https://github.com/ViTAE-Transformer/ViTPose).  The config files of these models are only for validation.*

> With simple decoder

| Arch                                                                                                              | Input Size |  AP   | AP<sup>50</sup> | AP<sup>75</sup> |  AR   | AR<sup>50</sup> |    ckpt    |
| :---------------------------------------------------------------------------------------------------------------- | :--------: | :---: | :-------------: | :-------------: | :---: | :-------------: | :--------: |
| [ViTPose-S](/configs/body_2d_keypoint/topdown_heatmap/coco/td-hm_ViTPose-small-simple_8xb64-210e_coco-256x192.py) |  256x192   | 0.736 |      0.900      |      0.811      | 0.790 |      0.940      |  \[ckpt\]  |
| [ViTPose-B](/configs/body_2d_keypoint/topdown_heatmap/coco/td-hm_ViTPose-base-simple_8xb64-210e_coco-256x192.py)  |  256x192   | 0.756 |      0.906      |      0.826      | 0.809 |      0.946      |  \[ckpt\]  |
| [ViTPose-L](/configs/body_2d_keypoint/topdown_heatmap/coco/td-hm_ViTPose-large-simple_8xb64-210e_coco-256x192.py) |  256x192   | 0.781 |      0.914      |      0.853      | 0.833 |      0.952      | [ckpt](<>) |
| [ViTPose-H](/configs/body_2d_keypoint/topdown_heatmap/coco/td-hm_ViTPose-huge-simple_8xb64-210e_coco-256x192.py)  |  256x192   | 0.789 |      0.916      |      0.856      | 0.839 |      0.953      |  \[ckpt\]  |