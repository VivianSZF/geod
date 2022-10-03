# Improving 3D-aware Image Synthesis with A Geometry-aware Discriminator

<img src="./docs/assets/teaser.jpg"/>

**Figure:** *(a) Existing 3D-aware GANs where only the generator is made 3D-aware with the help of NeRF. (b) GeoD where the discriminator supervises the generator with the extracted geometry.*

> **Improving 3D-aware Image Synthesis with A Geometry-aware Discriminator** <br>
> Zifan Shi, Yinghao Xu, Yujun Shen, Deli Zhao, Qifeng Chen, Dit-Yan Yeung <br>
> *Thirty-sixth Conference on Neural Information Processing Systems (NeurIPS 2022)*

[[Paper](https://arxiv.org/pdf/2209.15637.pdf)]
[[Project Page](https://vivianszf.github.io/geod)]
[[Demo](https://youtu.be/qqAxEMSUYiE)]

This work aims at improving 3D-aware image synthesis from the discriminator's perspective.
    Despite the advancement of synthesis quality, existing methods fail to obtain moderate 3D 
    shapes. We argue that, considering the two-player game in the formulation of GANs, 
    *only making the generator 3D-aware is not enough*. To address this issue, we propose 
    **GeoD** through learning a geometry-aware discriminator to improve 3D-aware GANs. 
    Concretely, besides differentiating real and fake samples from the 2D image space, the 
    discriminator is additionally asked to derive the geometry information from the inputs, 
    which is then applied as the guidance of the generator. Such a simple yet effective design 
    facilitates learning substantially more accurate 3D shapes. Extensive experiments on various 
    generator architectures and training datasets verify the superiority of GeoD over 
    state-of-the-art alternatives. Moreover, our approach is registered as a general framework such 
    that a more capable discriminator (*i.e.*, with a third task of novel view synthesis 
    beyond domain classification and geometry extraction) can further assist the generator with 
    a better multi-view consistency.


## Results

Qualitative comparison with pi-GAN as the base model.
<img src="./docs/assets/fig_pigan.jpg"/>


3D reconstruction and novel view synthesis on real data with GAN inversion.
<img src="./docs/assets/inversion.jpg"/>



## BibTeX

```bibtex
@inproceedings{shi2022improving,
    title   = {Improving 3D-aware Image Synthesis with A Geometry-aware Discriminator},
    author  = {Shi, Zifan and Xu, Yinghao and Shen, Yujun and Zhao, Deli and Chen, Qifeng and Yeung, Dit-Yan},
    booktitle = {NeurIPS},
    year    = {2022}
  }
```
