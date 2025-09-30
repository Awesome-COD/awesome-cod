<p align="center">
    <img src="./imgs/Logo.png"/> <br />
</p>

<p align="center">
    <img src="https://img.shields.io/badge/-As%20awesome%20as%20you%20think!-red" alt="Awesome Badge">
    <img src="https://img.shields.io/badge/License-MIT-green.svg" alt="License: MIT">
    <img src="https://img.shields.io/github/last-commit/Awesome-COD/awesome-cod" alt="GitHub last commit">
</p>

# <p align=center>`Awesome List for Camouflaged Object Detection (COD)`

<details>
<summary><strong>:loudspeaker: Last updated: Sept/30/2025 </strong></summary>

- [09/2025] Update with ACMMM2025 and latest papers. 
- [06/2025] Update with ICCV2025 papers.    
- [06/2025] Update with CVPR2025, AAAI2025 papers.    
- [08/2024] Update with ECCV2024, MM2024 papers.  
- [04/2024] Update with CVPR2024 papers.  
- [01/2024] Update with ICLR2024, WACV2024 papers.   
- [12/2023] Update with  NeurIPS2023, AAAI2024 papers.   
- [08/2023] Update with ICCV2023, MM2023, etc. papers for COD and CIS.   
- [04/2023] Update with CVPR2023 papers for COD and CIS.
</details>

---

:teddy_bear: We mark different tasks with coloured squares:

<table>
    <tr>
        <td style="width: 20%;">:blue_square:<code>COD</code></td>
        <td style="width: 20%;">Camouflaged Object Detection (COD)</td>
        <td style="width: 20%;">:orange_square:<code>CIS</code></td>
        <td style="width: 20%;">Camouflaged Instance Segmentation (CIS)</td>
    </tr>
    <tr>
        <td style="width: 20%;">:green_square:<code>COC</code></td>
        <td style="width: 20%;">Camouflaged Object Counting (COC)</td>
        <td style="width: 20%;">:red_square:<code>VCOD</code></td>
        <td style="width: 20%;">Video Camouflaged Object Detection (VCOD)</td>
    </tr>
    <tr>
        <td style="width: 20%;">:diamond_shape_with_a_dot_inside:<code>RCOD</code></td>
        <td style="width: 20%;">Referring Camouflaged Object Detection (RCOD)</td>
        <td style="width: 20%;">:white_large_square:<code>XCOD</code></td>
        <td style="width: 20%;">Other types of COD</td>
    </tr>
</table>

---

<!--TOC-->

## 📚 Table of Contents:
<!-- - [Overview](#Overview) -->
<table style="margin-left: auto; margin-right: auto;">
    <tr>
        <td> <!--左侧内容-->
            <ul>
                <li><a href="#Preprint">Preprint</a></li>
                <li><a href="#Survey-Papers">Survey Papers</a></li>
                <li><a href="#Universal-Segmentation">Universal Segmentation</a></li>
                <li><a href="#COD">Camouflaged Object Detection (COD)</a></li>
                <li><a href="#VCOD">Video Camouflaged Object Detection (VCOD)</a></li>
                <li><a href="#CIS">Camouflaged Instance Segmentation (CIS)</a></li>
                <li><a href="#WSCOD">Weakly-supervised COD</a></li>
                <li><a href="#Semi-supervised-COD">Semi-supervised COD</a></li>
                <li><a href="#Unsupervised-COD">Unsupervised COD</a></li>
                <li><a href="#Zero-Shot-COD">Zero-Shot COD</a></li>
            </ul>
        </td>
        <td> <!--右侧内容-->
            <ul>
                <li><a href="#RefCOD">Referring COD</a></li>
                <li><a href="#OVCOS">Open-Vocabulary COS</a></li>
                <li><a href="#RGBP-COS">RGB-P COS</a></li>
                <li><a href="#MMW-COD">MMW COD</a></li>
                <li><a href="#Camouflage-Generation">Camouflage Generation</a></li>
                <li><a href="#Camouflaged-Object-Tracking">Camouflaged Object Tracking (COT)</a></li>
                <li><a href="#Spectral-COD">(Multi/Hyper-)Spectral COD</a></li>
                <li><a href="#Other-Related">Other Related</a></li>
                <li><a href="#Datasets">Datasets</a></li>
                <li><a href="#Appendix">Appendix</a></li>
            </ul>
        </td>
    </tr>
</table>

---

## Datasets

<sup>Note: Ann. Img. = Number of frames annotated in the dataset; BBbox = Bounding box; Pix. = Pixel-level mask; Ins. = Instance mask; Cate. = Category.</sup>

#### - Image COD

| **Name** | **Year** | **Pub.** | **Links** | **Type** | **Img.(Camo.)** | **BBbox** | **Pix.** | **Ins.** | **Comments**
| :------: | :------: | :-------: | :-------: | :-------: | :-------: | :-------: | :-------: | :-------: | :-------: |
[USC12K](https://github.com/ssecv/USCNet) | 2025 | ICCV | [Paper](https://arxiv.org/abs/2412.10943) | Img | 12000 |  | &check; |  | <sup><sub>Unconstrained salient & camouflaged object detection</sub></sup> 
[R2C7K](https://github.com/zhangxuying1004/RefCOD) | 2025 | PAMI | [Paper](https://github.com/zhangxuying1004/RefCOD) | Img | 5015/1600(Ref) |  | &check; |  | <sup><sub>Referring COD</sub></sup> | 
[PlantCamo](https://github.com/yjybuaa/PlantCamo) | 2025 | AIR | [Paper](https://arxiv.org/pdf/2410.17598) | Img | 1250 | &check; | &check; | &check; | <sup><sub>Plant COD</sub></sup>  |  
[CoCOD8K](https://github.com/zc199823/BBNet--CoCOD) | 2024 | TNNLS | [Paper](https://arxiv.org/abs/2310.04253) | Img | 8528 |  | &check; | | <sup><sub>Co-COD</sub></sup>  | 
[ACOD-12K](https://github.com/Kki2Eve/RISNet) | 2024 | CVPR | [Paper](https://openaccess.thecvf.com/content/CVPR2024/papers/Wang_Depth-Aware_Concealed_Crop_Detection_in_Dense_Agricultural_Scenes_CVPR_2024_paper.pdf) | Img | 6092 | &check; | &check; | | <sup><sub>RGB-D COD (Crop)</sub></sup> 
[ACOD2K](https://github.com/syxvision/FDNet) | 2023 | ICME | [Paper](https://arxiv.org/abs/2307.03943) | Img | 1500 |  | &check; | | <sup><sub>Artificial camouflaged object</sub></sup>  
[CAM-LDR](https://github.com/JingZhang617/COD-Rank-Localize-and-Segment) | 2023 | TCSVT | [Paper](https://arxiv.org/abs/2205.11333) | Img | 4040 | | | | <sup><sub>Camo ranking (fixation & ranking)</sub></sup>  
[CAMO++](https://sites.google.com/view/ltnghia/research/camo_plus_plus?authuser=0) | 2021 | TIP | [Paper](https://arxiv.org/abs/2103.17123) | Img | 2700 | &check; | &check; | &check; |  <sup><sub>Instance seg.</sub></sup>  
[NC4K](https://github.com/JingZhang617/COD-Rank-Localize-and-Segment) | 2021 | CVPR | [Paper](https://openaccess.thecvf.com/content/CVPR2021/papers/Lv_Simultaneously_Localize_Segment_and_Rank_the_Camouflaged_Objects_CVPR_2021_paper.pdf) | Img | 4121 | &check; | &check; | &check; |
[COD10K](http://dpfan.net/camouflage/) | 2020 | CVPR | [Paper](https://openaccess.thecvf.com/content_CVPR_2020/papers/Fan_Camouflaged_Object_Detection_CVPR_2020_paper.pdf) | Img | 5066 | &check; | &check; | &check; |
[CAMO](https://sites.google.com/view/ltnghia/research/camo) | 2019 | CVIU | [Paper](http://www.dgcv.nii.ac.jp/Publications/Papers/2019/cviu2019.pdf) | Img | 1250 |   | &check; |   |
[CPD1K](https://github.com/xfflyer/Camouflaged-people-detection) | 2018 | SPL | [Paper](https://ieeexplore.ieee.org/document/8336933)  | Img | 1000 |   | &check; |   | 
[CHAMELEON](https://www.polsl.pl/rau6/chameleon-database-animal-camouflage-analysis/) | 2017 | — | [Webpage](https://www.polsl.pl/rau6/chameleon-database-animal-camouflage-analysis/) | Img | 76 |   | &check; |   | 


#### - Weakly-Supervised Image COD

| **Name** | **Year** | **Pub.** | **Links** | **Type** | **Img.(Camo.)** | 
| :------: | :------: | :-------: | :-------: | :-------: | :-------: |
[P-COD](https://github.com/2231122/PCOD) | 2024 | ECCV | [Paper](https://arxiv.org/abs/2408.10777) | Point | 4040 | 
[S-COD](https://github.com/dddraxxx/Weakly-Supervised-Camouflaged-Object-Detection-with-Scribble-Annotations) | 2023 | AAAI | [Paper](https://arxiv.org/abs/2207.14083) | Scribble | 4040 | 


#### - Visual-Language Dataset

| **Name** | **Year** | **Pub.** | **Links** | **Img.(Camo.)** | **BBbox** | **Pix.** | **Ins.** | **Comments**
| :------: | :------: | :-------: | :-------: | :-------: | :-------: | :-------: | :-------: | :-------: |
[MM-CamObj](https://github.com/JCruan519/MM-CamObj) | 2025 | AAAI | [Paper](https://ojs.aaai.org/index.php/AAAI/article/view/32723) | 11363 |   | &check; |  | <sup><sub>CamObj-Align: image-text pairs; CamObj-Instruct: images and conversations with diverse instructions</sub></sup> |
[COD-TAX](https://github.com/lyu-yx/ACUMEN) | 2024 | ECCV | [Paper](https://arxiv.org/abs/2408.12086) | -- |  | &check; |  | <sup><sub>Obj masks with textual descriptions and attribute contributions</sub></sup> | 
[OVCamo](https://github.com/lartpang/OVCamo) | 2024 | ECCV | [Paper](https://arxiv.org/abs/2311.11241) | 11483 |  | &check; |  |  <sup><sub>Open-vocabulary seg. (obj. classes & masks)</sub></sup>|


#### - Video COD

| **Dataset** | **Year** | **Pub.** | **Links** | **Type** | **Clips/Ann.Img.** | **BBbox** | **Pix.** | **Ins.** | **Cate.** |**Comments** 
| :------: | :------: | :-------: | :-------: | :-------: | :-------: | :-------: | :-------: | :-------: | :-------: | :-------: |
[CamoVid60K](https://camovid.hkustvgd.com/) | 2025 | arXiv | [Paper](https://camovid.hkustvgd.com/) | Video |  218/62,774 | &check; | &check; | | &check; | 
MVCOD  | 2025 | arXiv | [Paper](https://arxiv.org/abs/2502.13859) | Video | 162/9,486 | &check; | &check; | &check; | &check; | | 
[MoCA-Mask](https://xueliancheng.github.io/SLT-Net-project/) | 2022 | CVPR | [Paper](https://arxiv.org/abs/2203.07363) | Video | 87/4,691 | &check; | &check; |   | &check; |   | 
[MoCA](https://www.robots.ox.ac.uk/~vgg/data/MoCA/) | 2020 | ACCV | [Paper](https://openaccess.thecvf.com/content/ACCV2020/html/Lamdouar_Betrayed_by_Motion_Camouflaged_Object_Discovery_via_Motion_Segmentation_ACCV_2020_paper.html) | Video | 141/7,617 | &check; |  |  |  |   | 
[CAMO UOW](https://sites.google.com/view/wanqingli/data-sets/uow-camo?authuser=0) | 2018 | TIP | [Paper](https://ieeexplore.ieee.org/document/8344427) | Video | 10/- |  | &check; |  |  | <sup><sub>Cate.: human</sub></sup>  
[CAD](https://www.user.tu-berlin.de/pbideau/motionSegmentation/index.html) | 2016 | ECCV | [Paper](https://link.springer.com/chapter/10.1007/978-3-319-46484-8_26) | Video | 9/191 |   | &check; |   |   | <sup><sub>Camouflaged Animal Dataset (CAD)</sub></sup>  


#### - Other Related Dataset 

| **Name** | **Year** | **Pub.** | **Links** | **Type** | **Img.(Camo.)** | **Ann.** | **Comments**
| :------: | :------: | :-------: | :-------: | :-------: | :-------: | :-------: | :-------: |
[IOCfish5K](https://github.com/GuoleiSun/Indiscernible-Object-Counting) | 2023 | CVPR | [Paper](https://openaccess.thecvf.com/content/CVPR2023/html/Sun_Indiscernible_Object_Counting_in_Underwater_Scenes_CVPR_2023_paper.html) | Img | 5637 | Point/Counting | <sup><sub>Indiscernible Object Counting</sub></sup>  
[CDS2K](https://github.com/DengPingFan/CSU) | 2023 | VI | [Paper](https://arxiv.org/abs/2304.11234) | Img | 2492 | BBbox+Pix. | <sup><sub>Defect seg. dataset</sub></sup>  

