
# FineGym: A Hierarchical Video Dataset for Fine-grained Action Understanding

### [Project Page](https://sdolivia.github.io/FineGym/) | [Videos](https://www.youtube.com/playlist?list=PL2wRKCL5yrJRBnIxWhmVr3xLJahdK5DGJ) | [Paper](https://arxiv.org/abs/2004.06704)

[FineGym: A Hierarchical Video Dataset for Fine-grained Action Understanding](https://sdolivia.github.io/FineGym/) <br>
 [Dian Shao](https://sdolivia.github.io/)<sup>1</sup>,
 [Yue Zhao](https://zhaoyue-zephyrus.github.io)<sup>1</sup>,
 [Bo Dai](http://daibo.info/)<sup>1</sup>,
 [Dahua Lin](http://dahualin.org/)<sup>1</sup> <br>
 <sup>1</sup> MMLab, The Chinese University of Hong Kong

<img src='assets/teaser.png'/>

<div align="center">
    <img src="assets/finegym_logo.png">
</div>

## News!
- 07/2020: We release pre-extracted features of FineGym dataset from 20 models for you to choose freely! See the following for more details!
- 05/2020: Talks and Demo about FineGym can all be found here: [FineGym Youtube Playlist] (https://www.youtube.com/playlist?list=PL2wRKCL5yrJRBnIxWhmVr3xLJahdK5DGJ).
- 04/2020: Annotations of FineGym Dataset are released! Please refer to [FineGym Homepage] (https://sdolivia.github.io/FineGym/) for more details!
- 03/2020: The Paper [FineGym: A Hierarchical Video Dataset for Fine-grained Action Understanding] (https://openaccess.thecvf.com/content_CVPR_2020/html/Shao_FineGym_A_Hierarchical_Video_Dataset_for_Fine-Grained_Action_Understanding_CVPR_2020_paper.html) is accepted by CVPR 2020 as an Oral Paper, and we got Three Strong Accepts!

## Model Zoo
### Pose Estimation
For Gym99 (for details of the subset gym99 & gym288 please refer to the [FineGym Homepage] (https://sdolivia.github.io/FineGym/)) :

<center>

| Model        | Backbone     | Pre-trained | Fine-tuned | Mean Class ACC | Top-1 ACC | Train-features            | Val-Features            | Feature-size per inst. |
|--------------|--------------|-------------|------------|----------------|-----------|---------------------------|-------------------------|------------------------|
| BN-Inception | BN-Inception | ImageNet    | -          | -              | -         | [Gym99-train-bninception] | [Gym99-val-bninception] | 12 x 1024 x 1 x 1      |
| ResNet50     | ResNet50     | ImageNet    | -          | -              | -         | [Gym99-train-r50]         | [Gym99-val-r50]         | 12 x 2048 x 1 x 1      |
| TSN          | BN-Inception | ImageNet    | Gym99      | 61.4           | 74.8      | [Gym99-train-tsn]         | [Gym99-val-tsn]         | 12 x 1024 x 1 x 1      |
| I3D          | ResNet50     | ImageNet    | Gym99      | 63.2           | 74.8      | [Gym99-train-i3d-imnet]   | [Gym99-val-i3d-imnet]   | 12 x 2048 x 1 x 1 x 1  |
| I3D          | ResNet50     | Kinetics    | Gym99      | 64.4           | 75.6      | [Gym99-train-i3d-kin]     | [Gym99-val-i3d-kin]     | 12 x 2048 x 1 x 1 x 1  |
</center>

For Gym288:

<center>

| Model        | Backbone     | Pre-trained | Fine-tuned | Mean Class ACC | Top-1 ACC | Train-features            | Val-Features            | Feature-size per inst. |
|--------------|--------------|-------------|------------|----------------|-----------|---------------------------|-------------------------|------------------------|
| BN-Inception | BN-Inception | ImageNet    | -          | -              | -         | [Gym288-train-bninception] | [Gym288-val-bninception] | 12 x 1024 x 1 x 1      |
| ResNet50     | ResNet50     | ImageNet    | -          | -              | -         | [Gym288-train-r50]         | [Gym288-val-r50]         | 12 x 2048 x 1 x 1      |
| TSN          | BN-Inception | ImageNet    | Gym288      | 26.5           | 68.3      | [Gym288-train-tsn]         | [Gym288-val-tsn]         | 12 x 1024 x 1 x 1      |
| I3D          | ResNet50     | ImageNet    | Gym288      | 27.9           | 66.7      | [Gym288-train-i3d-imnet]   | [Gym288-val-i3d-imnet]   | 12 x 2048 x 1 x 1 x 1  |
| I3D          | ResNet50     | Kinetics    | Gym288      | 28.2           | 66.1      | [Gym288-train-i3d-kin]     | [Gym288-val-i3d-kin]     | 12 x 2048 x 1 x 1 x 1  |

</center>
