<div align="center"> 
<img src="Images/image2.png" width="800" alt="Celebration"/>    
   
# Awesome 3D Scene Representation for Robotics [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
   
 


This repo contains a curative list of **3D Scene Representation papers relating to the Robotics domain**.

#### Please feel free to send me [pull requests](https://github.com/dtc111111/awesome-representation-for-robotics) or [email](mailto:dengtianchen@sjtu.edu.cn) to add papers! <br>

If you find this repository useful, please consider [citing](#citation) and STARing this list. Feel free to share this list with others!
<div align="left">   
  
---

## Overview
  - [Survey](#3dgs-survey)
    
  - [General Model](#3dgs-general-model)
    - [Photorealistic](#photorealistic)
    - [Sparse View](#sparse-view)
    - [Accelerate & Compression](#accelerate--compression)
    - [Geometry & Physics](#Geometry--Physics)

  - [1.Perception](#perception)
    - [1.1 Point Cloud](#1.1-Point-Cloud)
    - [1.2 Voxel Grid](#1.2-Voxel-Grid)
    - [1.3 Signed Distance Field (SDF)](#1.3-Signed-Distance-Field(SDF))
    - [1.4 Mesh](#1.4-Mesh)
    - [1.5 Scene Graph](#1.5-Scene-Graph)
    - [1.6 Neural Radiance Fields (NeRF)](#1.6-Neural-Radiance-Fields(NeRF))
    - [1.7 3D Gaussian Splatting (3DGS)](#1.7-3D-Gaussian-Splatting(3DGS))
    - [1.8 Foundation Model](#1.8-Foundation-Model)
    
  - [2.Mapping](#mapping)
    - [2.1 Point Cloud](#2.1-Point-Cloud)
    - [2.2 Voxel Grid](#2.2-Voxel-Grid)
    - [2.3 Signed Distance Field (SDF)](#2.3-Signed-Distance-Field(SDF))
    - [2.4 Mesh](#2.4-Mesh)
    - [2.5 Scene Graph](#2.5-Scene-Graph)
    - [2.6 Neural Radiance Fields (NeRF)](#2.6-Neural-Radiance-Fields(NeRF))
    - [2.7 3D Gaussian Splatting (3DGS)](#2.7-3D-Gaussian-Splatting(3DGS))
    - [2.8 Foundation Model](#2.8-Foundation-Model)

  - [3.Localization](#localization)
    - [3.1 Point Cloud](#3.1-Point-Cloud)
    - [3.2 Voxel Grid](#3.2-Voxel-Grid)
    - [3.3 Signed Distance Field (SDF)](#3.3-Signed-Distance-Field(SDF))
    - [3.4 Mesh](#3.4-Mesh)
    - [3.5 Scene Graph](#3.5-Scene-Graph)
    - [3.6 Neural Radiance Fields (NeRF)](#3.6-Neural-Radiance-Fields(NeRF))
    - [3.7 3D Gaussian Splatting (3DGS)](#3.7-3D-Gaussian-Splatting(3DGS))
    - [3.8 Foundation Model](#3.8-Foundation-Model)

  - [4.Navigation](#navigation)
    - [4.1 Geometric Representations](#4.1-Geometric-Representations)
    - [4.2 NeRF-based Representations](#4.2-NeRF-based-Representations)
    - [4.3 3DGS-based Representations](#4.3-3DGS-based-Representations)
    - [4.4 Foundation Model](#4.4-Foundation-Model)

  - [5.Manipulation](#manipulation)
    - [5.1 Point Cloud](#5.1-Point-Cloud)
    - [5.2 Voxel Grid](#5.2-Voxel-Grid)
    - [5.3 Signed Distance Field (SDF)](#5.3-Signed-Distance-Field(SDF))
    - [5.4 Mesh](#5.4-Mesh)
    - [5.5 Scene Graph](#5.5-Scene-Graph)
    - [5.6 Neural Radiance Fields (NeRF)](#5.6-Neural-Radiance-Fields(NeRF))
    - [5.7 3D Gaussian Splatting (3DGS)](#5.7-3D-Gaussian-Splatting(3DGS))
    - [5.8 Foundation Model](#5.8-Foundation-Model)

  - [6.Simulation](#simulation)

  - [Citation](#citation)

---
## Survey
#### [S1] A Survey on 3D Gaussian Splatting
- **🧑‍🔬 Author**：Guikun Chen, Wenguan Wang
- **🏫 Institute**：Zhejiang University
- **🔗 Link**：[[arXiv:2401.03890](https://arxiv.org/abs/2401.03890)]


#### [S2] 3D Gaussian as a New Vision Era: A Survey
- **🧑‍🔬 Author**：Ben Fei, Jingyi Xu, Rui Zhang, Qingyuan Zhou, Weidong Yang, Ying He
- **🏫 Institute**：Fudan University ⟐ Nanyang Technological University
- **🔗 Link**：[[IEEE Transactions on Visualization and Computer Graphics 2024](https://arxiv.org/abs/2402.07181)]


#### [S3] Recent Advances in 3D Gaussian Splatting
- **🧑‍🔬 Author**：Tong Wu, Yu-Jie Yuan, Ling-Xiao Zhang, Jie Yang, Yan-Pei Cao, Ling-Qi Yan, Lin Gao
- **🏫 Institute**：Chinese Academy of Sciences ⟐ VAST ⟐  University of California
- **🔗 Link**：[[arXiv:2403.11134](https://arxiv.org/abs/2403.11134)]


#### [S4] Gaussian Splatting: 3D Reconstruction and Novel View Synthesis, a Review
- **🧑‍🔬 Author**：Anurag Dalal, Daniel Hagen, Kjell G. Robbersmyr, Kristian Muri Knausgård
- **🏫 Institute**：University of Agder
- **🔗 Link**：[[IEEE Access](https://arxiv.org/abs/2405.03417)]


#### [S5] Survey on Fundamental Deep Learning 3D Reconstruction Techniques
- **🧑‍🔬 Author**：Yonge Bai, LikHang Wong, TszYin Twan
- **🏫 Institute**：McMaster University ⟐  City University of Hong Kong
- **🔗 Link**：[[arXiv:2405.03417](https://arxiv.org/abs/2407.08137)]


#### [S6] 3D Gaussian Splatting: Survey, Technologies, Challenges, and Opportunities
- **🧑‍🔬 Author**：Yanqi Bao, Tianyu Ding, Jing Huo, Yaoli Liu, Yuxin Li, Wenbin Li, Yang Gao, Jiebo Luo
- **🏫 Institute**：Nanjing University ⟐  University of Rochester ⟐ Microsoft
- **🔗 Link**：[[arXiv:2405.03417](https://arxiv.org/abs/2407.17418)]




## General Model
---
* 3D Gaussian Splatting for Real-Time Radiance Field Rendering, **SIGGRAPH, 2023**. [[Paper](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/3d_gaussian_splatting_low.pdf)] [[Website](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/)]
### Photorealistic
* Mip-splatting Alias-free 3d gaussian splatting, **CVPR, 2024**. [[Paper](https://openaccess.thecvf.com/content/CVPR2024/papers/Yu_Mip-Splatting_Alias-free_3D_Gaussian_Splatting_CVPR_2024_paper.pdf)] [[Website](https://niujinshuchong.github.io/mip-splatting/)]  [[Code](https://github.com/autonomousvision/mip-splatting)]
* FreGS: 3D Gaussian Splatting with Progressive Frequency Regularization, **CVPR 2024**. [[Paper](https://arxiv.org/pdf/2403.06908.pdf)]
* Gaussianshader: 3d gaussian splatting with shading functions for reflective surfaces, **CVPR 2024**. [[Paper](https://openaccess.thecvf.com/content/CVPR2024/papers/Jiang_GaussianShader_3D_Gaussian_Splatting_with_Shading_Functions_for_Reflective_Surfaces_CVPR_2024_paper.pdf)]
* End-to-End Rate-Distortion Optimized 3D Gaussian Representation, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2406.01597.pdf)] [[Website](https://arxiv.org/abs/2406.01597)] [[Code](https://github.com/USTC-IMCL/RDO-Gaussian)]
* Analytic-Splatting: Anti-Aliased 3D Gaussian Splatting via Analytic Integration, **ECCV 2024**. [[Paper](https://arxiv.org/pdf/2403.11056.pdf)]
* Deblurring 3D Gaussian Splatting, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2401.00834)] [[Code](https://github.com/benhenryL/Deblurring-3D-Gaussian-Splatting)]
* BAD-Gaussians: Bundle Adjusted Deblur Gaussian Splatting, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2403.11831)] [[Code](https://github.com/WU-CVGL/BAD-Gaussians)]
* MIGS: Multi-Identity Gaussian Splatting via Tensor Decomposition, **ECCV, 2024**. [[Paper](https://arxiv.org/abs/2407.07284)]
* Multi-Scale 3D Gaussian Splatting for Anti-Aliased Rendering, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2311.17089.pdf)]
* Implicit Gaussian Splatting with Efficient Multi-Level Tri-Plane Representation, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.10041)]
* GaussianPro: 3D Gaussian Splatting with Progressive Propagation, **ICML 2024**. [[Paper](https://arxiv.org/pdf/2402.14650.pdf)] [[Website](https://kcheng1021.github.io/gaussianpro.github.io/)] [[Code](https://github.com/kcheng1021/GaussianPro)]
* Spectral-GS: Taming 3D Gaussian Splatting with Spectral Entropy, *arXiv*. [[Paper](https://arxiv.org/abs/2409.12771)]
* RayGauss: Volumetric Gaussian-Based Ray Casting for Photorealistic Novel View Synthesis, *arXiv*. [[Paper](https://arxiv.org/abs/2408.03356)]
* Spec-Gaussian: Anisotropic View-Dependent Appearance for 3D Gaussian Splatting, **NeurIPS 2024**. [[Paper](https://arxiv.org/pdf/2402.15870.pdf)]
* Gaussian Splatting with Localized Points Management, *arXiv*. [[Paper](https://arxiv.org/abs/2406.04251)]
* GStex: Per-Primitive Texturing of 2D Gaussian Splatting for Decoupled Appearance and Geometry Modeling, *arXiv*. [[Paper](https://arxiv.org/abs/2409.12954)]
* 3iGS: Factorised Tensorial Illumination for 3D Gaussian Splatting, **ECCV, 2024**. [[Paper](https://arxiv.org/abs/2408.03753)]
* SA-GS: Scale-Adaptive Gaussian Splatting for Training-Free Anti-Aliasing, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.19615)] [[Website](https://kevinsong729.github.io/project-pages/SA-GS/)] [[Code](https://github.com/zsy1987/SA-GS/)]
* FreeGaussian: Guidance-free Controllable 3D Gaussian Splats with Flow Derivatives, *arXiv*. [[Paper](https://arxiv.org/abs/2410.22070)]
* GS-Blur: A 3D Scene-Based Dataset for Realistic Image Deblurring, *arXiv*. [[Paper](https://arxiv.org/abs/2410.23658)]
* GausSurf: Geometry-Guided 3D Gaussian Splatting for Surface Reconstruction, *arXiv*. [[Paper](https://arxiv.org/abs/2411.19454)]
* SfM-Free 3D Gaussian Splatting via Hierarchical Training, *arXiv*. [[Paper](https://arxiv.org/abs/2412.01553)]
* Reflective Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2412.19282)]


---

### Sparse View
* Fast Dynamic 3D Object Generation from a Single-view Video, *arXiv*. [[Paper](https://arxiv.org/pdf/2401.08742.pdf)] [[Website](https://fudan-zvg.github.io/Efficient4D/)] [[Code](https://github.com/fudan-zvg/Efficient4D)]
* GaussianObject: High-Quality 3D Object Reconstruction from Four Views with Gaussian Splatting, **ACM Transactions on Graphics**. [[Paper](https://arxiv.org/pdf/2402.10259.pdf)] [[Website](https://gaussianobject.github.io/)] [[Code](https://github.com/GaussianObject/GaussianObject)]
* LGM: Large Multi-View Gaussian Model for High-Resolution 3D Content Creation, **ECCV 2024**. [[Paper](https://arxiv.org/pdf/2402.05054.pdf)] [[Website](https://me.kiui.moe/lgm/)] [[Code](https://github.com/3DTopia/LGM)]
* IM-3D: Iterative Multiview Diffusion and Reconstruction for High-Quality 3D Generation, *arXiv*. [[Paper](https://arxiv.org/pdf/2402.08682.pdf)] [[Website](https://arxiv.org/abs/2402.08682)]
* FDGaussian: Fast Gaussian Splatting from Single Image via Geometric-aware Diffusion Model, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.10242.pdf)] [[Website](https://qjfeng.net/FDGaussian)]
* Depth-Regularized Optimization for 3D Gaussian Splatting in Few-Shot Images, **CVPRW, 2024**. [[Paper](https://arxiv.org/pdf/2311.13398.pdf)] [[Website](https://robot0321.github.io/DepthRegGS/index.html)] [[Code](https://github.com/robot0321/DepthRegularizedGS)]
* DNGaussian: Optimizing Sparse-View 3D Gaussian Radiance Fields with Global-Local Depth Normalization, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2403.06912.pdf)] [[Website](https://fictionarry.github.io/DNGaussian/)] [[Code](https://github.com/Fictionarry/DNGaussian)]
* MVSplat: Efficient 3D Gaussian Splatting from Sparse Multi-View Images, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2403.14627)] [[Website](https://donydchen.github.io/mvsplat/)] [[Code](https://github.com/donydchen/mvsplat)]
* latentSplat: Autoencoding Variational Gaussians for Fast Generalizable 3D Reconstruction, **ECCV 2024**. [[Paper](https://arxiv.org/pdf/2403.16292.pdf)] [[Website](https://geometric-rl.mpi-inf.mpg.de/latentsplat/)] [[Code](https://github.com/Chrixtar/latentsplat)]
* GRM: Large Gaussian Reconstruction Model for Efficient 3D Reconstruction and Generation, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.14621.pdf)] [[Website](https://justimyhxu.github.io/projects/grm/)] [[Code](https://github.com/justimyhxu/grm)]
* Gamba: Marry Gaussian Splatting with Mamba for single view 3D reconstruction, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.18795)]
* CoherentGS: Sparse Novel View Synthesis with Coherent 3D Gaussians, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2403.19495)] [[Website](https://people.engr.tamu.edu/nimak/Papers/CoherentGS/index.html)]
* InstantSplat: Unbounded Sparse-view Pose-free Gaussian Splatting in 40 Seconds, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.20309.pdf)] [[Website](https://instantsplat.github.io/)]
* Sp<sup>2</sup>360: Sparse-view 360 Scene Reconstruction using Cascaded 2D Diffusion Priors, *arXiv*. [[Paper](https://arxiv.org/pdf/2405.16517)]
* SparseGS: Real-Time 360° Sparse View Synthesis using Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2312.00206.pdf)] [[Website](https://formycat.github.io/SparseGS-Real-Time-360-Sparse-View-Synthesis-using-Gaussian-Splatting/)]
* FSGS: Real-Time Few-shot View Synthesis using Gaussian Splatting, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2312.00451.pdf)] [[Website](https://zehaozhu.github.io/FSGS/)] [[Code](https://github.com/VITA-Group/FSGS)]
* pixelSplat: 3D Gaussian Splats from Image Pairs for Scalable Generalizable 3D Reconstruction, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2312.12337.pdf)] [[Website](https://davidcharatan.com/pixelsplat/)] [[Code](https://github.com/dcharatan/pixelsplat)]
* Splatter Image: Ultra-Fast Single-View 3D Reconstruction, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2312.13150.pdf)] [[Website](https://szymanowiczs.github.io/splatter-image.html)] [[Code](https://github.com/szymanowiczs/splatter-image)]
* EndoSparse: Real-Time Sparse View Synthesis of Endoscopic Scenes using Gaussian Splatting, **MICCAI, 2024**. [[Paper](https://arxiv.org/abs/2407.01029)] [[Code](https://github.com/CUHK-AIM-Group/EndoSparse)]
* Learning 3D Gaussians for Extremely Sparse-View Cone-Beam CT Reconstruction, **MICCAI, 2024**. [[Paper](https://arxiv.org/abs/2407.01090)] [[Code](https://github.com/xmed-lab/DIF-Gaussian)]
* CoR-GS: Sparse-View 3D Gaussian Splatting via Co-Regularization, **ECCV, 2024**. [[Paper](https://arxiv.org/abs/2405.12110)]
* LoopSparseGS: Loop Based Sparse-View Friendly Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.00254)]
* Self-augmented Gaussian Splatting with Structure-aware Masks for Sparse-view 3D Reconstruction, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.04831)]
* ReconX: Reconstruct Any Scene from Sparse Views with Video Diffusion Model, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.16767)]
* LM-Gaussian: Boost Sparse-view 3D Gaussian Splatting with Large Model Priors, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.03456)]
* Optimizing 3D Gaussian Splatting for Sparse Viewpoint Scene Reconstruction, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.03213)]
* Object Gaussian for Monocular 6D Pose Estimation from Sparse Views, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.02581)]
* Single-View 3D Reconstruction via SO(2)-Equivariant Gaussian Sculpting Networks, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.07245)]
* Vista3D: Unravel the 3D Darkside of a Single Image, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.12193)]
* MVPGS: Excavating Multi-view Priors for Gaussian Splatting from Sparse Input Views, **ECCV 2024**. [[Paper](https://arxiv.org/pdf/2409.14316)]
* Learn to Optimize Denoising Scores for 3D Generation: A Unified and Improved Diffusion Prior on NeRF and 3D Gaussian Splatting, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2312.04820)] [[Code](https://github.com/yangxiaofeng/LODS)]
* Self-Evolving Depth-Supervised 3D Gaussian Splatting from Rendered Stereo Pairs, **BMVC 2024**. [[Paper](https://arxiv.org/abs/2409.07456)]
* Frequency-based View Selection in Gaussian Splatting Reconstruction, *arXiv*. [[Paper](https://arxiv.org/abs/2409.16470)]
* GSD: View-Guided Gaussian Splatting Diffusion for 3D Reconstruction, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2407.04237)]
* 3DGS-Enhancer: Enhancing Unbounded 3D Gaussian Splatting with View-consistent 2D Diffusion Priors, **NeurIPS 2024**. [[Paper](https://arxiv.org/abs/2410.16266)]
* Binocular-Guided 3D Gaussian Splatting with View Consistency for Sparse View Synthesis, **NeurIPS 2024**. [[Paper](https://arxiv.org/abs/2410.18822)]
* No Pose, No Problem: Surprisingly Simple 3D Gaussian Splats from Sparse Unposed Images, *arXiv*. [[Paper](https://arxiv.org/abs/2410.24207)]
* Epipolar-Free 3D Gaussian Splatting for Generalizable Novel View Synthesis, *arXiv*. [[Paper](https://arxiv.org/abs/2410.22817)]
* MVSplat360: Feed-Forward 360 Scene Synthesis from Sparse Views, *arXiv*. [[Paper](https://arxiv.org/pdf/2411.04924)]
* Structure Consistent Gaussian Splatting with Matching Prior for Few-shot Novel View Synthesis, *arXiv*. [[Paper](https://arxiv.org/abs/2411.03637)]
* FewViewGS: Gaussian Splatting with Few View Matching and Multi-stage Training, *arXiv*. [[Paper](https://arxiv.org/abs/2411.02229)]
* GPS-Gaussian+: Generalizable Pixel-wise 3D Gaussian Splatting for Real-Time Human-Scene Rendering from Sparse Views, *arXiv*. [[Paper](https://arxiv.org/abs/2411.11363)]
* SmileSplat: Generalizable Gaussian Splats for Unconstrained Sparse Images, *arXiv*. [[Paper](https://arxiv.org/abs/2411.18072)]
* NovelGS: Consistent Novel-view Denoising via Large Gaussian Reconstruction Model, *arXiv*. [[Paper](https://arxiv.org/abs/2411.16779)]
* SelfSplat: Pose-Free and 3D Prior-Free Generalizable 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2411.17190)]
* PreF3R: Pose-Free Feed-Forward 3D Gaussian Splatting from Variable-length Image SequencePreF3R: Pose-Free Feed-Forward 3D Gaussian Splatting from Variable-length Image Sequence, *arXiv*. [[Paper](https://arxiv.org/abs/2411.16877)]
* ZeroGS: Training 3D Gaussian Splatting from Unposed Images, *arXiv*. [[Paper](https://arxiv.org/abs/2411.15779)]
* Speedy-Splat: Fast 3D Gaussian Splatting with Sparse Pixels and Sparse Primitives, *arXiv*. [[Paper](https://arxiv.org/abs/2412.00578)]
* Sparse Voxels Rasterization: Real-time High-fidelity Radiance Field Rendering, *arXiv*. [[Paper](https://arxiv.org/abs/2412.04459)]
* Volumetrically Consistent 3D Gaussian Rasterization, *arXiv*. [[Paper](https://arxiv.org/abs/2412.03378)]
* PanSplat: 4K Panorama Synthesis with Feed-Forward Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2412.12096)]
* FreeSplatter: Pose-free Gaussian Splatting for Sparse-view 3D Reconstruction, *arXiv*. [[Paper](https://arxiv.org/abs/2412.09573)]
* GBR: Generative Bundle Refinement for High-fidelity Gaussian Splatting and Meshing, *arXiv*. [[Paper](https://arxiv.org/abs/2412.05908)]
* TSGaussian: Semantic and Depth-Guided Target-Specific Gaussian Splatting from Sparse Views, *arXiv*. [[Paper](https://arxiv.org/abs/2412.10051)]
* Dust to Tower: Coarse-to-Fine Photo-Realistic Scene Reconstruction from Sparse Uncalibrated Images, *arXiv*. [[Paper](https://arxiv.org/abs/2412.19518)]
* Gaussian Masked Autoencoders, *arXiv*. [[Paper](https://arxiv.org/abs/2501.03229)]
* FatesGS: Fast and Accurate Sparse-View Surface Reconstruction using Gaussian Splatting with Depth-Feature Consistency, *arXiv*. [[Paper](https://arxiv.org/abs/2501.04628)]
* FeatureGS: Eigenvalue-Feature Optimization in 3D Gaussian Splatting for Geometrically Accurate and Artifact-Reduced Reconstruction, *arXiv*. [[Paper](https://arxiv.org/abs/2501.17655)]
* See In Detail: Enhancing Sparse - view 3D Gaussian Splatting with Local Depth and Semantic Regularization, *arXiv*. [[Paper](https://arxiv.org/abs/2501.11508)]
* RDG - GS: Relative Depth Guidance with Gaussian Splatting for Real - time Sparse - View 3D Rendering, *arXiv*. [[Paper](https://arxiv.org/abs/2501.11102)]
* PoI: Pixel of Interest for Novel View Synthesis Assisted Scene Coordinate Regression, *arXiv*. [[Paper](https://arxiv.org/abs/2502.04843)]
* Splatter-360: Generalizable 360∘ Gaussian Splatting for Wide-baseline Panoramic Images, *arXiv*. [[Paper](https://arxiv.org/abs/2412.06250)]




### Accelerate & Compression
* Hash3D: Training-free Acceleration for 3D Generation, *arXiv*. [[Paper](https://arxiv.org/pdf/2404.06091)] [[Website](https://adamdad.github.io/hash3D/)] [[Code](https://github.com/Adamdad/hash3D)]
* Characterizing Satellite Geometry via Accelerated 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2401.02588.pdf)]
* TRIPS: Trilinear Point Splatting for Real-Time Radiance Field Rendering, *arXiv*. [[Paper](https://arxiv.org/pdf/2401.06003.pdf)] [[Website](https://lfranke.github.io/trips/)] [[Code](https://github.com/lfranke/trips)]
* GaussianImage: 1000 FPS Image Representation and Compression by 2D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.08551)]
* TOGS: Gaussian Splatting with Temporal Opacity Offset for Real-Time 4D DSA Rendering, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.19586)]
* Periodic Vibration Gaussian: Dynamic Urban Scene Reconstruction and Real-time Rendering, *arXiv*. [[Paper](https://arxiv.org/pdf/2311.18561.pdf)] [[Website](https://fudan-zvg.github.io/PVG/)] [[Code](https://github.com/fudan-zvg/PVG)]
* Triplane Meets Gaussian Splatting: Fast and Generalizable Single-View 3D Reconstruction with Transformers, **CVPR 2024**. [[Paper](https://arxiv.org/pdf/2312.09147.pdf)] [[Website](https://zouzx.github.io/TriplaneGaussian/)] [[Code](https://github.com/VAST-AI-Research/TriplaneGaussian)]
* DISTWAR: Fast Differentiable Rendering on Raster-based Rendering Pipelines, *arXiv*. [[Paper](https://arxiv.org/pdf/2401.05345.pdf)]
* EAGLES: Efficient Accelerated 3D Gaussians with Lightweight EncodingS, **ECCV 2024**. [[Paper](https://arxiv.org/pdf/2312.04564.pdf)] [[Website](https://efficientgaussian.github.io/)] [[Code](https://github.com/Sharath-girish/efficientgaussian)]
* Optimal Projection for 3D Gaussian Splatting, *arXiv*. [[Paper](https://browse.arxiv.org/pdf/2402.00752.pdf)]
* StopThePop: Sorted Gaussian Splatting for View-Consistent Real-time Rendering, *arXiv*. [[Paper](https://arxiv.org/pdf/2402.00525.pdf)] [[Website](https://r4dl.github.io/StopThePop/)] [[Code](https://github.com/r4dl/StopThePop)]
* GES: Generalized Exponential Splatting for Efficient Radiance Field Rendering, *CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2402.10128.pdf)] [[Website](https://abdullahamdi.com/ges/)] [[Code](https://github.com/ajhamdi/ges-splatting)]
* Identifying Unnecessary 3D Gaussians using Clustering for Fast Rendering of 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2402.13827.pdf)]
* RadSplat: Radiance Field-Informed Gaussian Splatting for Robust Real-Time Rendering with 900+ FPS, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.13806.pdf)] [[Website](https://m-niemeyer.github.io/radsplat/)]
* Mini-Splatting: Representing Scenes with a Constrained Number of Gaussians, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.14166.pdf)]
* Pixel-GS: Density Control with Pixel-aware Gradient for 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.15530.pdf)]
* Octree-GS: Towards Consistent Real-time Rendering with LOD-Structured 3D Gaussians, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.17898)] [[Website](https://city-super.github.io/octree-gs/)] [[Code](https://github.com/city-super/Octree-GS)]
* OmniGS: Omnidirectional Gaussian Splatting for Fast Radiance Field Reconstruction using Omnidirectional Images, **WACV 2025**. [[Paper](https://arxiv.org/pdf/2404.03202)]
* GSCore: Efficient Radiance Field Rendering via Architectural Support for 3D Gaussian Splatting, **ASPLOS 2024**. [[Paper](https://jaewoong.org/pubs/asplos24-gscore.pdf)]
* Scaffold-GS: Structured 3D Gaussians for View-Adaptive Rendering, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2312.00109.pdf)] [[Website](https://city-super.github.io/scaffold-gs/)] [[Code](https://github.com/city-super/Scaffold-GS)]
* Superpoint Gaussian Splatting for Real-Time High-Fidelity Dynamic Scene Reconstruction, **ICML, 2024**. [[Paper](https://arxiv.org/pdf/2406.03697)]
* FastScene: Text-Driven Fast 3D Indoor Scene Generation via Panoramic Gaussian Splatting, **IJCAI, 2024**. [[Paper](https://arxiv.org/abs/2405.05768)]
* Compressed 3D Gaussian Splatting for Accelerated Novel View Synthesis, **CVPR, 2024**. [[Paper](https://arxiv.org/abs/2401.02436)] [[Code](https://github.com/KeKsBoTer/c3dgs)]
* Compact3D: Smaller and Faster Gaussian Splatting with Vector Quantization, **ECCV, 2024**. [[Paper](https://arxiv.org/abs/2311.18159)] [[Code](https://github.com/UCDvision/compact3d)]
* HAC: Hash-grid Assisted Context for 3D Gaussian Splatting Compression, **ECCV, 2024**. [[Paper](https://arxiv.org/abs/2403.14530)] [[Code](https://github.com/YihangChen-ee/HAC)]
* Compact 3D Gaussian Representation for Radiance Field, **CVPR, 2024**. [[Paper](https://arxiv.org/abs/2311.13681)] [[Code](https://github.com/maincold2/Compact-3DGS)]
* Fast Generalizable Gaussian Splatting Reconstruction from Multi-View Stereo, **ECCV, 2024**. [[Paper](https://arxiv.org/abs/2405.12218)] [[Code](https://github.com/TQTQliu/MVSGaussian)]
* MVG-Splatting: Multi-View Guided Gaussian Splatting with Adaptive Quantile-Based Geometric Consistency Densification, *arXiv*. [[Paper](https://browse.arxiv.org/pdf/2407.11840.pdf)]
* Splatfacto-W: A Nerfstudio Implementation of Gaussian Splatting for Unconstrained Photo Collections, *arXiv*. [[Paper](https://browse.arxiv.org/pdf/2407.12306.pdf)]
* Compact 3D Gaussian Splatting for Static and Dynamic Radiance Fields, *arXiv*. [[Paper](https://arxiv.org/abs/2408.03822)]
* FLoD: Integrating Flexible Level of Detail into 3D Gaussian Splatting for Customizable Rendering, *TOG, 2025*. [[Paper](https://arxiv.org/abs/2408.12894)]
* Robust 3D Gaussian Splatting for Novel View Synthesis in Presence of Distractors, *arXiv*. [[Paper](https://arxiv.org/abs/2408.11697)]
* PRoGS: Progressive Rendering of Gaussian Splats, *arXiv*. [[Paper](https://arxiv.org/abs/2409.01761)]
* Weight Conditioning for Smooth Optimization of Neural Networks, *arXiv*. [[Paper](https://arxiv.org/abs/2409.03424)]
* 3DGS-LM: Faster Gaussian-Splatting Optimization with Levenberg-Marquardt, *arXiv*. [[Paper](https://arxiv.org/abs/2409.12892)]
* MesonGS: Post-training Compression of 3D Gaussians via Efficient Attribute Transformation, **ECCV 2024**. [[Paper](https://arxiv.org/abs/2409.09756)]
* VR-Splatting: Foveated Radiance Field Rendering via 3D Gaussian Splatting and Neural Points, *arXiv*. [[Paper](https://arxiv.org/abs/2410.17932)]
* Sort-free Gaussian Splatting via Weighted Sum Rendering, *arXiv*. [[Paper](https://arxiv.org/abs/2410.18931)]
* LightGaussian: Unbounded 3D Gaussian Compression with 15x Reduction and 200+ FPS, **NeurIPS 2024**. [[Paper](https://arxiv.org/abs/2311.17245)] [[Code](https://lightgaussian.github.io/)]
* ELMGS: Enhancing memory and computation scaLability through coMpression for 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2410.23213)]
* A Hierarchical Compression Technique for 3D Gaussian Splatting Compression, *arXiv*. [[Paper](https://arxiv.org/abs/2411.06976)]
* DyGASR: Dynamic Generalized Exponential Splatting with Surface Alignment for Accelerated 3D Mesh Reconstruction, *arXiv*. [[Paper](https://arxiv.org/abs/2411.09156)]
* Projecting Gaussian Ellipsoids While Avoiding Affine Projection Approximation, *arXiv*. [[Paper](https://arxiv.org/abs/2411.07579)]
* Mini-Splatting2: Building 360 Scenes within Minutes via Aggressive Gaussian Densification, *arXiv*. [[Paper](https://arxiv.org/abs/2411.12788)]
* SCIGS: 3D Gaussians Splatting from a Snapshot Compressive Image, *arXiv*. [[Paper](https://arxiv.org/abs/2411.12471)]
* Beyond Gaussians: Fast and High-Fidelity 3D Splatting with Linear Kernels, *arXiv*. [[Paper](https://arxiv.org/abs/2411.12440)]
* 3D Convex Splatting: Radiance Field Rendering with 3D Smooth Convexes3D Convex Splatting: Radiance Field Rendering with 3D Smooth Convexes, *arXiv*. [[Paper](https://arxiv.org/abs/2411.14974)]
* Textured Gaussians for Enhanced 3D Scene Appearance Modeling, *arXiv*. [[Paper](https://arxiv.org/abs/2411.18625)]
* HEMGS: A Hybrid Entropy Model for 3D Gaussian Splatting Data Compression, *arXiv*. [[Paper](https://arxiv.org/abs/2411.18473)]
* Pushing Rendering Boundaries: Hard Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2412.04826)]
* Faster and Better 3D Splatting via Group Training, *arXiv*. [[Paper](https://arxiv.org/abs/2412.07608)]
* Temporally Compressed 3D Gaussian Splatting for Dynamic Scenes, *arXiv*. [[Paper](https://arxiv.org/abs/2412.05700)]
* QUEEN: QUantized Efficient ENcoding of Dynamic Gaussians for Streaming Free-viewpoint Videos, *arXiv*. [[Paper](https://arxiv.org/abs/2412.04469)]
* SG-Splatting: Accelerating 3D Gaussian Splatting with Spherical Gaussians, *arXiv*. [[Paper](https://arxiv.org/abs/2501.00342)]
* Locality-aware Gaussian Compression for Fast and High-quality Rendering, *arXiv*. [[Paper](https://arxiv.org/abs/2501.05757)]
* Trick-GS: A Balanced Bag of Tricks for Efficient Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2501.14534)]
* HAC++: Towards 100X Compression of 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2501.12255)]
* GoDe: Gaussians on Demand for Progressive Level of Detail and Scalable Compressiong, *arXiv*. [[Paper](https://arxiv.org/abs/2501.13558)]
* Exploring the Versal AI Engine for 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2502.11782)]



### Geometry & Physics
* 2D Gaussian Splatting for Geometrically Accurate Radiance Fields, **SIGGRAPH, 2024**. [[Paper](https://arxiv.org/pdf/2403.17888)] [[Website](https://surfsplatting.github.io/)]  [[Code](https://github.com/hbb1/2d-gaussian-splatting)]
* Gaussian Splashing: Dynamic Fluid Synthesis with Gaussian Splatting, *arXiv*. [[Paper](https://browse.arxiv.org/pdf/2401.15318.pdf)] [[Website](https://amysteriouscat.github.io/GaussianSplashing/)]
* GaMeS: Mesh-Based Adapting and Modification of Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2402.01459.pdf)] [[Code](https://github.com/waczjoan/gaussian-mesh-splatting)]
* Mesh-based Gaussian Splatting for Real-time Large-scale Deformation, *arXiv*. [[Paper](https://arxiv.org/pdf/2402.04796.pdf)]
* Reconstruction and Simulation of Elastic Objects with Spring-Mass 3D Gaussians, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.09434)] [[Website](https://zlicheng.com/spring_gaus/)] [[Code](https://github.com/Colmar-zlicheng/Spring-Gaus)]
* Texture-GS: Disentangling the Geometry and Texture for 3D Gaussian Splatting Editing, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.10050)] [[Website](https://slothfulxtx.github.io/TexGS/)] [[Code](https://github.com/slothfulxtx/Texture-GS)]
* DN-Splatter: Depth and Normal Priors for Gaussian Splatting and Meshing, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.17822)] [[Website](https://maturk.github.io/dn-splatter/)] [[Code](https://github.com/maturk/dn-splatter)]
* Feature Splatting: Language-Driven Physics-Based Scene Synthesis and Editing, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2404.01223)] [[Website](https://feature-splatting.github.io/)] [[Code](https://github.com/vuer-ai/feature_splatting)]
* Surface Reconstruction from Gaussian Splatting via Novel Stereo Views, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2404.01810)] [[Website](https://gs2mesh.github.io/)]
* RaDe-GS: Rasterizing Depth in Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2406.01467)] [[Website](https://baowenz.github.io/radegs/)]
* Trim 3D Gaussian Splatting for Accurate Geometry Representation, *arXiv*. [[Paper](https://arxiv.org/abs/2406.07499)] [[Website](https://trimgs.github.io/)] [[Code](https://github.com/YuxueYang1204/TrimGS)]
* Effective Rank Analysis and Regularization for Enhanced 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2406.11672)] [[Website](https://junhahyung.github.io/erankgs.github.io/)]
* PhysGaussian: Physics-Integrated 3D Gaussians for Generative Dynamics, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2311.12198.pdf)] [[Website](https://xpandora.github.io/PhysGaussian/)] [[Code](https://github.com/XPandora/PhysGaussian)]
* SuGaR: Surface-Aligned Gaussian Splatting for Efficient 3D Mesh Reconstruction and High-Quality Mesh Rendering, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2311.12775.pdf)] [[Website](https://imagine.enpc.fr/~guedona/sugar/)] [[Code](https://github.com/Anttwo/SuGaR)]
* NeuSG: Neural Implicit Surface Reconstruction with 3D Gaussian Splatting Guidance, *arXiv*. [[Paper](https://arxiv.org/pdf/2312.00846.pdf)]
* Projecting Radiance Fields to Mesh Surfaces, **SIGGRAPH, 2024**. [[Paper](https://arxiv.org/abs/2406.11570)]
* GVKF: Gaussian Voxel Kernel Functions for Highly Efficient Surface Reconstruction in Open Scenes, **NeurIPS 2024**. [[Paper](https://arxiv.org/abs/2411.01853)]
* GeoGaussian: Geometry-aware Gaussian Splatting for Scene Rendering, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.11324.pdf)]
* Enhancement of 3D Gaussian Splatting using Raw Mesh for Photorealistic Recreation of Architectures, *arXiv*. [[Paper](https://arxiv.org/pdf/2407.15435.pdf)]
* Integrating Meshes and 3D Gaussians for Indoor Scene Reconstruction with SAM Mask Guidance, *arXiv*. [[Paper](https://arxiv.org/pdf/2407.16173.pdf)]
* 2DGH: 2D Gaussian-Hermite Splatting for High-quality Rendering and Better Geometry Reconstruction, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.16982.pdf)]
* Depth Estimation Based on 3D Gaussian Splatting Siamese Defocus, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.12323.pdf)]
* DepthSplat: Connecting Gaussian Splatting and Depth, *arXiv*. [[Paper](https://arxiv.org/abs/2410.13862)]
* Quadratic Gaussian Splatting for Efficient and Detailed Surface Reconstruction, *arXiv*. [[Paper](https://arxiv.org/abs/2411.16392)]
* Geometry Field Splatting with Gaussian Surfels, *arXiv*. [[Paper](https://arxiv.org/abs/2411.17067)]
* G2SDF: Surface Reconstruction from Explicit Gaussians with Implicit SDFs, *arXiv*. [[Paper](https://arxiv.org/abs/2411.16898)]
* GSurf: 3D Reconstruction via Signed Distance Fields with Direct Gaussian Supervision, *arXiv*. [[Paper](https://arxiv.org/abs/2411.15723)]
* SplatSDF: Boosting Neural Implicit SDF via Gaussian Splatting Fusion, *arXiv*. [[Paper](https://arxiv.org/abs/2411.15468)]
* Generative Densification: Learning to Densify Gaussians for High-Fidelity Generalizable 3D Reconstruction, *arXiv*. [[Paper](https://arxiv.org/abs/2412.06234)]
* Pgsr: Planar-based gaussian splatting for efficient and high-fidelity surface reconstruction, **TVCG 2024**. [[Paper](https://ieeexplore.ieee.org/abstract/document/10747190/)]
* Gasp: Gaussian splatting for physic-based simulations,*arXiv*. [[Paper](https://arxiv.org/abs/2409.05819)]
* Physics3D: Learning Physical Properties of 3D Gaussians via Video Diffusion,*arXiv*. [[Paper](https://arxiv.org/abs/2406.04338)]
* CDGS: Confidence-Aware Depth Regularization for 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2502.14684)]




## 1.Perception<a id="perception"></a>
### 1.1 Point Cloud<a id="1.1-Point-Cloud"></a>
* PIXOR: Real-time 3D Object Detection from Point Clouds, **CVPR, 2018**. [[Paper](https://openaccess.thecvf.com/content_cvpr_2018/papers/Yang_PIXOR_Real-Time_3D_CVPR_2018_paper.pdf)][[Code](https://github.com/philip-huang/PIXOR)]
* PointPillars: Fast Encoders for Object Detection From Point Clouds, **CVPR, 2019**. [[Paper](https://ieeexplore.ieee.org/document/8954311)][[Code](https://github.com/nutonomy/second.pytorch)]
* 3DSSD: Point-based 3D Single Stage Object Detector, **CVPR, 2020**. [[Paper](https://openaccess.thecvf.com/content_CVPR_2020/papers/Yang_3DSSD_Point-Based_3D_Single_Stage_Object_Detector_CVPR_2020_paper.pdf)][[Code](https://github.com/JIA-Lab-research/3DSSD)]
* Self-Supervised Learning of Scene-Graph Representations for Robotic Sequential Manipulation Planning, **CoRL, 2020**. [[Paper](https://proceedings.mlr.press/v155/nguyen21b.html)]
* PointContrast: Unsupervised Pre-training for 3D Point Cloud Understanding, **ECCV, 2020**. [[Paper](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123480579.pdf)][[Code](https://github.com/facebookresearch/PointContrast)]
* Multimodal Virtual Point 3D Detection, **NeurIPS, 2021**. [[Paper](https://proceedings.neurips.cc/paper_files/paper/2021/file/895daa408f494ad58006c47a30f51c1f-Paper.pdf)][[Code](https://github.com/tianweiy/MVP)]
* Center-based 3D Object Detection and Tracking, **CVPR, 2021**. [[Paper](https://openaccess.thecvf.com/content/CVPR2021/papers/Yin_Center-Based_3D_Object_Detection_and_Tracking_CVPR_2021_paper.pdf)][[Code](https://github.com/zion-king/Center-based-3D-Object-Detection-and-Tracking)]
* SceneGraphFusion: Incremental 3D Scene Graph Prediction from RGB-D Sequences, **CVPR, 2021**. [[Paper](https://openaccess.thecvf.com/content/CVPR2021/papers/Wu_SceneGraphFusion_Incremental_3D_Scene_Graph_Prediction_From_RGB-D_Sequences_CVPR_2021_paper.pdf)][[Code](https://github.com/ShunChengWu/SceneGraphFusion)][[Website](https://shunchengwu.github.io/SceneGraphFusion)]
* A Unified Query-based Paradigm for Point Cloud Understanding， **CVPR, 2022**. [[Paper](https://openaccess.thecvf.com/content/CVPR2022/papers/Yang_A_Unified_Query-Based_Paradigm_for_Point_Cloud_Understanding_CVPR_2022_paper.pdf)][[Code](https://github.com/JIA-Lab-research/DeepVision3D)]
### 1.2 Voxel Grid<a id="1.2-Voxel-Grid"></a>
* OctoMap: AnEfficient Probabilistic 3D Mapping Framework Based on Octrees, **AUTON ROBOT, 2013**. [[Paper](https://courses.cs.washington.edu/courses/cse571/16au/slides/hornung13auro.pdf)][[Code](https://github.com/OctoMap/octomap)]
* VoxelNet: End-to-End Learning for Point Cloud Based 3D Object Detection, **CVPR, 2018**. [[Paper](https://openaccess.thecvf.com/content_cvpr_2018/papers/Zhou_VoxelNet_End-to-End_Learning_CVPR_2018_paper.pdf)][[Website](https://yjh-jm.github.io/3d%20object%20detection/voxelnet/)]
* VMNet: Voxel-Mesh Network for Geodesic-Aware 3D Semantic Segmentation, **ICCV, 2021**. [[Paper](https://ieeexplore.ieee.org/document/9710530)][[Code](https://github.com/hzykent/VMNet)]
* VoxFormer: Sparse Voxel Transformer for Camera-based 3D Semantic Scene Completion, **CVPR, 2023**. [[Paper](https://openaccess.thecvf.com/content/CVPR2023/papers/Li_VoxFormer_Sparse_Voxel_Transformer_for_Camera-Based_3D_Semantic_Scene_Completion_CVPR_2023_paper.pdf)][[Code](https://github.com/NVlabs/VoxFormer)]
### 1.3 Signed Distance Field (SDF)<a id="1.3-Signed-Distance-Field(SDF)"></a>
* SurroundSDF: Implicit 3D Scene Understanding Based on Signed Distance Field, **CVPR, 2024**. [[Paper](https://openaccess.thecvf.com/content/CVPR2024/papers/Liu_SurroundSDF_Implicit_3D_Scene_Understanding_Based_on_Signed_Distance_Field_CVPR_2024_paper.pdf)][[Code](https://github.com/xiaomi-mlab/SurroundSDF)][[Website](https://xiaomi-mlab.github.io/SurroundSDF/)]
### 1.4 Mesh<a id="1.4-Mesh"></a>
### 1.5 Scene Graph<a id="1.5-Scene-Graph"></a>
* 3D Scene Graph: A structure for unified semantics, 3D space, and camera, **ICCV, 2019**. [[Paper](https://openaccess.thecvf.com/content_ICCV_2019/papers/Armeni_3D_Scene_Graph_A_Structure_for_Unified_Semantics_3D_Space_ICCV_2019_paper.pdf)][[Code](https://github.com/StanfordVL/3DSceneGraph)]
* Hydra: A Real-time Spatial Perception System for 3D Scene Graph Construction and Optimization, **RSS, 2022**. [[Paper](https://www.roboticsproceedings.org/rss18/p050.pdf)][[Code](https://github.com/MIT-SPARK/Hydra)]
* SGFormer: Semantic Graph Transformer for Point Cloud-Based 3D Scene Graph Generation, **AAAI, 2024**. [[Paper](https://ojs.aaai.org/index.php/AAAI/article/download/28197/28391)][[Code](https://github.com/Andy20178/SGFormer)]
### 1.6 Neural Radiance Fields (NeRF)<a id="1.6-Neural-Radiance-Fields(NeRF)"></a>
* CLIP-NeRF: Text-and-Image Driven Manipulation of Neural Radiance Fields, **CVPR, 2022**. [[Paper](https://openaccess.thecvf.com/content/CVPR2022/papers/Wang_CLIP-NeRF_Text-and-Image_Driven_Manipulation_of_Neural_Radiance_Fields_CVPR_2022_paper.pdf)][[Code](https://github.com/cassiePython/CLIPNeRF)][[Website](https://cassiepython.github.io/clipnerf/)]
* LERF: Language Embedded Radiance Fields, **ICCV, 2023**. [[Paper](https://openaccess.thecvf.com/content/ICCV2023/papers/Kerr_LERF_Language_Embedded_Radiance_Fields_ICCV_2023_paper.pdf)][[Code](https://github.com/kerrj/lerf)][[Website](https://www.lerf.io/)]
* NeRF-Det: Learning Geometry-Aware Volumetric Representation for Multi-View 3D Object Detection, **ICCV, 2023**, [[Paper](https://openaccess.thecvf.com/content/ICCV2023/papers/Xu_NeRF-Det_Learning_Geometry-Aware_Volumetric_Representation_for_Multi-View_3D_Object_Detection_ICCV_2023_paper.pdf)][[Code](https://github.com/facebookresearch/NeRF-Det)][[Website](https://chenfengxu714.github.io/nerfdet/)]
* SNI-SLAM: Semantic Neural Implicit SLAM, **CVPR, 2024**. [[Paper](https://openaccess.thecvf.com/content/CVPR2024/papers/Zhu_SNI-SLAM_Semantic_Neural_Implicit_SLAM_CVPR_2024_paper.pdf)][[Code](https://github.com/IRMVLab/SNI-SLAM)]
* GaussianFormer: Scene as Gaussians for Vision-Based 3D Semantic Occupancy Prediction, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2405.17429)] [[Code](https://github.com/huang-yh/GaussianFormer)][[Website](https://wzzheng.net/GaussianFormer/)]
* 2D-Guided 3D Gaussian Segmentation, **ASIANComNet, 2024**. [[Paper](https://arxiv.org/pdf/2312.16047.pdf)]
* GO-N3RDet: Geometry Optimized NeRF-enhanced 3D Object Detector, **CVPR, 2025**, [[Paper](https://openaccess.thecvf.com/content/CVPR2025/papers/Li_GO-N3RDet_Geometry_Optimized_NeRF-enhanced_3D_Object_Detector_CVPR_2025_paper.pdf)][[Code](https://github.com/ZechuanLi/GO-N3RDet)]
### 1.7 3D Gaussian Splatting (3DGS)<a id="1.7-3D-Gaussian-Splatting(3DGS)"></a>
* 6DGS: 6D Pose Estimation from a Single Image and a 3D Gaussian Splatting Model, **ECCV, 2024**. [[Paper](https://www.ecva.net/papers/eccv_2024/papers_ECCV/papers/06914.pdf)][[Code](https://github.com/mbortolon97/6dgs)][[Website](https://mbortolon97.github.io/6dgs/)]
* GOI: Find 3D Gaussians of Interest with an Optimizable Open-vocabulary Semantic-space Hyperplane, **MM, 2024**. [[Paper](https://arxiv.org/pdf/2405.17596)][[Code](https://github.com/Quyans/GOI-Hyperplane)][[Website](https://quyans.github.io/GOI-Hyperplane/)]
* Click-Gaussian: Interactive Segmentation to Any 3D Gaussians, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2407.11793)][[Website](https://seokhunchoi.github.io/Click-Gaussian/)]
* GS2Pose: Two-stage 6D Object Pose Estimation Guided by Gaussian Splatting, **CVPR, 2024**. [[Website](https://arxiv.org/abs/2411.03807)]
* Gaussian Grouping: Segment and Edit Anything in 3D Scenes, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2312.00732.pdf)] [[Code](https://github.com/lkeab/gaussian-grouping)][[Website](https://ymq2017.github.io/gaussian-grouping/)]
* SRIF: Semantic Shape Registration Empowered by Diffusion-based Image Morphing and Flow Estimation, **SA, 2024**. [[Paper](https://arxiv.org/abs/2409.11682)][[Code](https://github.com/rqhuang88/SRIF)]
* OpenGaussian: Towards Point-Level 3D Gaussian-based Open Vocabulary Understanding, **NeurIPS, 2024**. [[Paper](https://proceedings.neurips.cc/paper_files/paper/2024/file/21f7b745f73ce0d1f9bcea7f40b1388e-Paper-Conference.pdf)][[Code](https://github.com/yanmin-wu/OpenGaussian)][[Website](https://3d-aigc.github.io/OpenGaussian/)]
* Feature 3DGS: Supercharging 3D Gaussian Splatting to Enable Distilled Feature Fields, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2312.03203.pdf)][[Code](https://github.com/ShijieZhou-UCLA/feature-3dgs)][[Website](https://feature-3dgs.github.io/)]
* Language Embedded 3D Gaussians for Open-Vocabulary Scene Understanding, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2311.18482.pdf)][[Code](https://github.com/buaavrcg/LEGaussians)][[Website](https://buaavrcg.github.io/LEGaussians/)]
* LangSplat: 3D Language Gaussian Splatting, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2312.16084.pdf)][[Code](https://github.com/minghanqin/LangSplat)][[Website](https://langsplat.github.io/)]
* FMGS: Foundation Model Embedded 3D Gaussian Splatting for Holistic 3D Scene Understanding,**IJCV, 2024**. [[Paper](https://arxiv.org/pdf/2401.01970.pdf)][[Code](https://github.com/google-research/foundation-model-embedded-3dgs)][[Website](https://xingxingzuo.github.io/fmgs/)]
* EgoLifter: Open-world 3D Segmentation for Egocentric Perception, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2403.18118.pdf)][[Code](https://github.com/facebookresearch/egolifter)][[Website](https://egolifter.github.io/)]
* Touch-GS: Visual-Tactile Supervised 3D Gaussian Splatting, **IROS 2024**. [[Paper](https://arxiv.org/pdf/2403.09875.pdf)][[Code](https://github.com/armlabstanford/Touch-GS)][[Website](https://armlabstanford.github.io/touch-gs)]
* EvGGS: A Collaborative Learning Framework for Event-based Generalizable Gaussian Splatting, **ICML, 2024**. [[Paper](https://arxiv.org/pdf/2405.14959.pdf)][[Code](https://github.com/Mercerai/EvGGS)]
* Object and Contact Point Tracking in Demonstrations Using 3D Gaussian Splatting, **CoRL, 2024**. [[Paper](https://arxiv.org/abs/2411.03555)]
* GaussianCut: Interactive segmentation via graph cut for 3D Gaussian Splatting, **NeurIPS, 2024**. [[Paper](https://arxiv.org/abs/2411.07555)][[Code](https://github.com/umangi-jain/gaussiancut)][[Website](https://umangi-jain.github.io/gaussiancut/)]
* A General Framework to Boost 3D GS Initialization for Text-to-3D Generation by Lexical Richness, **MM, 2024**. [[Paper](https://arxiv.org/pdf/2408.01269.pdf)][[Code](https://github.com/cyjdlhy/DreamInit)][[Website](https://vlislab22.github.io/DreamInit/)]
* Language-Embedded Gaussian Splats (LEGS): Incrementally Building Room-Scale Representations with a Mobile Robot, **IROS 2024**. [[Paper](https://arxiv.org/abs/2409.18108)][[Code](https://github.com/uynitsuj/LEGS)][[Website](https://berkeleyautomation.github.io/LEGS/)]
* DarkGS: Learning Neural Illumination and 3D Gaussians Relighting for Robotic Exploration in the Dark, **IROS, 2024**. [[Paper](https://arxiv.org/pdf/2403.10814)] [[Code](https://github.com/tyz1030/darkgs)]
* PRTGS: Precomputed Radiance Transfer of Gaussian Splats for Real-Time High-Quality Relighting, **MM, 2024**. [[Paper](https://arxiv.org/pdf/2408.03538)]
* Thermal3D-GS: Physics-induced 3D Gaussians for Thermal Infrared Novel-view Synthesis, **ECCV 2024**. [[Paper](https://arxiv.org/pdf/2409.08042)][[Code](https://github.com/mzzcdf/Thermal3DGS)]
* Relightable 3D Gaussian: Real-time Point Cloud Relighting with BRDF Decomposition and Ray Tracing, **ECCV 2024**. [[Paper](https://arxiv.org/pdf/2311.16043.pdf)][[Code](https://github.com/NJU-3DV/Relightable3DGaussian)][[Website](https://nju-3dv.github.io/projects/Relightable3DGaussian/)]
* Gaussian in the Wild: 3D Gaussian Splatting for Unconstrained Image Collections, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2403.15704)][[Code](https://github.com/EastbeanZhang/Gaussian-Wild)][[Website](https://eastbeanzhang.github.io/GS-W/)]
* SWAG: Splatting in the Wild images with Appearance-conditioned Gaussians, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2403.10427.pdf)]
* Gaussian Shadow Casting for Neural Characters, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2401.06116.pdf)][[Code](https://github.com/LuisBolanos17/GaussianShadowCasting)]
* Dynamic 3D Gaussian Tracking for Graph-Based Neural Dynamics Modeling, **CoRL, 2024**. [[Paper](https://arxiv.org/pdf/2410.18912.pdf)][[Code](https://github.com/robo-alex/gs-dynamics)][[Website](https://gs-dynamics.github.io/)]
* GS-IR: 3D Gaussian Splatting for Inverse Rendering, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2311.16473.pdf)][[Code](https://github.com/lzhnb/GS-IR)][[Website](https://github.com/lzhnb/GS-IR)]
* Event3DGS: Event-Based 3D Gaussian Splatting for High-Speed Robot Egomotion, **CoRL, 2024**. [[Paper](https://arxiv.org/abs/2406.02972)][[Website](https://tyxiong23.github.io/event3dgs)]
* Gaussian in the Dark: Real-Time View Synthesis From Inconsistent Dark Images Using Gaussian Splatting, **PG, 2024**. [[Paper](https://arxiv.org/pdf/2408.09130)][[Code](https://github.com/yec22/Gaussian-DK)]
* Modeling Uncertainty in 3D Gaussian Splatting through Continuous Semantic Splatting, **CSE, 2024**. [[Paper](https://arxiv.org/abs/2411.02547)]
* FlashSplat: 2D to 3D Gaussian Splatting Segmentation Solved Optimally, **ECCV, 2024**. [[Paper](https://arxiv.org/abs/2409.08270)][[Code](https://github.com/florinshen/FlashSplat)]
* GaussianBeV : 3D Gaussian Representation meets Perception Models for BeV Segmentation, **WACV, 2025**. [[Paper](https://openaccess.thecvf.com/content/WACV2025/papers/Chabot_GaussianBeV__3D_Gaussian_Representation_Meets_Perception_Models_for_BeV_WACV_2025_paper.pdf)]
* Segment Any 3D Gaussians, **AAAI, 2025**. [[Paper](https://jumpat.github.io/SAGA/SAGA_paper.pdf)][[Code](https://github.com/Jumpat/SegAnyGAussians)][[Website](https://jumpat.github.io/SAGA/)]
* SpectralGaussians: Semantic, spectral 3D Gaussian splatting for multi-spectral scene representation, visualization and analysis, **ISPRS J PHOTOGRAMM, 2025**. [[Paper](https://arxiv.org/pdf/2408.06975)]
* Efficient Semantic Splatting for Remote Sensing Multi-view Segmentation, **TGRS, 2025**. [[Paper](https://arxiv.org/abs/2412.05969)]
* Semantics-Controlled Gaussian Splatting for Outdoor Scene Reconstruction and Rendering in Virtual Reality, **VR, 2025**. [[Paper](https://arxiv.org/abs/2409.15959)][[Code](https://github.com/HannahHaensen/SCGS)]
* Gaga: Group Any Gaussians via 3D-aware Memory Bank, **ICLR, 2025**. [[Paper](https://arxiv.org/pdf/2404.07977.pdf)][[Code](https://github.com/weijielyu/Gaga)][[Website](https://www.gaga.gallery/)]
* Gradient-Driven 3D Segmentation and Affordance Transfer in Gaussian Splatting Using 2D Masks, **ICRA, 2025**. [[Paper](https://arxiv.org/abs/2409.11681)][[Code](https://github.com/JojiJoseph/3dgs-gradient-segmentation)][[Website](https://jojijoseph.github.io/3dgs-segmentation/)]
* Unleashing the Potential of Multi-modal Foundation Models and Video Diffusion for 4D Dynamic Physical Scene Simulation, **CVPR, 2025**. [[Paper](https://arxiv.org/abs/2411.14423)][[Code](https://github.com/zhuomanliu/PhysFlow)][[Website](https://zhuomanliu.github.io/PhysFlow/)]
* Proc-GS: Procedural Building Generation for City Assembly with 3D Gaussians, **CVPRW, 2025**. [[Paper](https://arxiv.org/abs/2412.07660)][[Code](https://github.com/city-super/ProcGS)][[Website](https://city-super.github.io/procgs/)]
* FastLGS: Speeding up Language Embedded Gaussians with Feature Grid Mapping, **AAAI, 2025**. [[Paper](https://arxiv.org/pdf/2406.01916.pdf)][[Code](https://github.com/George-Attano/FastLGS-Ex)][[Website](https://george-attano.github.io/FastLGS/)]
* SLGaussian: Fast Language Gaussian Splatting in Sparse Views, **MM, 2025**. [[Paper](https://arxiv.org/abs/2412.08331)][[Code](https://github.com/chenkangjie1123/SLGaussian)][[Website](https://chenkangjie1123.github.io/SLGaussian.github.io/)]
* DCSEG: Decoupled 3D Open-Set Segmentation using Gaussian Splatting, **CVPRW, 2025**. [[Paper](https://arxiv.org/abs/2412.10972)][[Code](https://github.com/lusxvr/dcseg)]
* CLIP-GS: Unifying Vision - Language Representation with 3D Gaussian Splatting, **ICCV, 2025**. [[Paper](https://arxiv.org/abs/2412.19142)]
* GIR: 3D Gaussian Inverse Rendering for Relightable Scene Factorization, **TPAMI, 2025**. [[Paper](https://arxiv.org/pdf/2312.05133)][[Code](https://github.com/guduxiaolang/GIR/)][[Website](https://3dgir.github.io/)]
* WeatherGS: 3D Scene Reconstruction in Adverse Weather Conditions via Gaussian Splatting, **ICRA, 2025**. [[Paper](https://www.arxiv.org/abs/2412.18862)][[Code](https://github.com/Jumponthemoon/WeatherGS)][[Website](https://jumponthemoon.github.io/weather-gs/)]
* Decoupling Appearance Variations with 3D Consistent Features in Gaussian Splatting, **AAAI, 2025**. [[Paper](https://arxiv.org/abs/2501.10788)][[Website](https://davi-gaussian.github.io/)]
* GeoSplatting: Towards Geometry Guided Gaussian Splatting for Physically-based Inverse Rendering, **ICCV, 2025**. [[Paper](https://arxiv.org/abs/2410.24204)][[Code](https://github.com/PKU-VCL-Geometry/GeoSplatting)][[Website](https://pku-vcl-geometry.github.io/GeoSplatting/)]
* TranSplat: Surface Embedding-guided 3D Gaussian Splatting for Transparent Object Manipulation, **ICRA, 2025**. [[Paper](https://arxiv.org/abs/2502.07840)][[Code](https://github.com/jeongyun0609/TranSplat)]
* OMG: Opacity Matters in Material Modeling with Gaussian Splatting, **ICLR, 2025**. [[Paper](https://arxiv.org/abs/2502.10988)][[Code](https://github.com/SilongYong/OMG)]
* DeRainGS: Gaussian Splatting for Enhanced Scene Reconstruction in Rainy Environments, **AAAI, 2025**. [[Paper](https://arxiv.org/pdf/2408.11540)][[Website](https://deraings.github.io/)]
* SeaSplat: Representing Underwater Scenes with 3D Gaussian Splatting and a Physically Grounded Image Formation Model, **ICRA, 2025**. [[Paper](https://arxiv.org/pdf/2409.17345)][[Code](https://github.com/dxyang/seasplat/)][[Website](https://seasplat.github.io/)]
* Deblur4DGS: 4D Gaussian Splatting from Blurry Monocular Video, **AAAI, 2026**. [[Paper](https://arxiv.org/abs/2412.06424)][[Code](https://github.com/ZcsrenlongZ/Deblur4DGS)][[Website](https://deblur4dgs.github.io/)]
* MATT-GS: Masked Attention-based 3DGS for Robot Perception and Object Detection, *arXiv*. [[Code](https://arxiv.org/abs/2503.19330)]
* Semantic Gaussians: Open-Vocabulary Scene Understanding with 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.15624)][[Code](https://github.com/sharinka0715/semantic-gaussians)][[Website](https://semantic-gaussians.github.io/)]
* Query-based Semantic Gaussian Field for Scene Representation in Reinforcement Learning, *arXiv*. [[Paper](https://arxiv.org/pdf/2406.02370)]
* Gaussian Control with Hierarchical Semantic Graphs in 3D Human Recovery, *arXiv*. [[Paper](https://arxiv.org/pdf/2405.12477)][[Code](https://github.com/3DHumanRehab/SemanticGraph-Gaussian)][[Website](https://wanghongsheng01.github.io/HUGS/)]
* SlingBAG: Sliding ball adaptive growth algorithm with differentiable radiation enables super-efficient iterative 3D photoacoustic image reconstruction, *arXiv*. [[Paper](https://arxiv.org/pdf/2407.11781)]
* Contrastive Gaussian Clustering: Weakly Supervised 3D Scene Segmentation, *arXiv*. [[Paper](https://arxiv.org/abs/2404.12784)][[Code](https://github.com/MyrnaCCS/contrastive-gaussian-clustering)]
* CoSSegGaussians: Compact and Swift Scene Segmenting 3D Gaussians, *arXiv*. [[Paper](https://arxiv.org/pdf/2401.05925.pdf)][[Code](https://DavidDou.github.io/CoSSegGaussians)][[Website](https://david-dou.github.io/CoSSegGaussians/)]
* Segment Anything in 3D Gaussians, *arXiv*. [[Paper](https://browse.arxiv.org/pdf/2401.17857.pdf)][[Code](https://github.com/XuHu0529/SAGS)]
* GS-PT: Exploiting 3D Gaussian Splatting for Comprehensive Point Cloud Understanding via Self-supervised Learning, *arXiv*. [[Paper](https://arxiv.org/abs/2409.04963)]
* Splat: FAST-Fast, Ambiguity-Free Semantics Transfer in Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2411.13753)][[Code](https://github.com/fastsplat/fastsplat.github.io)]
* GLS: Geometry-aware 3D Language Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2411.18066)][[Code](https://github.com/HorizonRobotics/GLS)][[Website](https://jiaxiongq.github.io/GLS_ProjectPage/)]
* GradiSeg: Gradient-Guided Gaussian Segmentation with Enhanced 3D Boundary Precision, *arXiv*. [[Paper](https://arxiv.org/abs/2412.00392)][[Website](https://alphagolzh.github.io/gradiseg.io/)]
* EaDeblur-GS: Event assisted 3D Deblur Reconstruction with Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2407.13520.pdf)]
* Automated 3D Physical Simulation of Open-world Scene with Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2411.12789)][[Website](https://sim-gs.github.io/)]
* SuperGSeg: Open-Vocabulary 3D Segmentation with Structured Super-Gaussians, *arXiv*. [[Paper](https://arxiv.org/abs/2412.10231)][[Website](https://supergseg.github.io/)]
* LineGS : 3D Line Segment Representation on 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2412.00477)][[Code](https://github.com/ericshenggle/LineGS)]
* SparseLGS: Sparse View Language Embedded Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2412.02245)][[Website](https://ustc3dv.github.io/SparseLGS/)]
* Occam's LGS: A Simple Approach for Language Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2412.01807)][[Code](https://github.com/insait-institute/OccamLGS)][[Website](https://insait-institute.github.io/OccamLGS/)]
* ChatSplat: 3D Conversational Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2412.00734)]
* RAIN-GS: Relaxing Accurate Initialization Constraint for 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.09413)][[Code](https://github.com/KU-CVLAB/RAIN-GS)][[Website](https://ku-cvlab.github.io/RAIN-GS/)]
* LumiGauss: High-Fidelity Outdoor Relighting with 2D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.04474)]
* Phys3DGS: Physically-based 3D Gaussian Splatting for Inverse Rendering, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.10335)]
* ThermalGaussian: Thermal 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.07200)][[Code](https://github.com/chen-hangyu/Thermal-Gaussian-main)][[Website](https://thermalgaussian.github.io/)]
* E-3DGS: Gaussian Splatting with Exposure and Motion Events, *arXiv*. [[Paper](https://arxiv.org/pdf/2410.16995)][[Code](https://github.com/MasterHow/E-3DGS)]
* GUS-IR: Gaussian Splatting with Unified Shading for Inverse Rendering, *arXiv*. [[Paper](https://arxiv.org/abs/2411.07478)]
* ULSR-GS: Ultra Large-scale Surface Reconstruction Gaussian Splatting with Multi-View Geometric Consistency, *arXiv*. [[Paper](https://arxiv.org/abs/2412.01402)][[Website](https://ulsrgs.github.io/)]
* FlameGS: Reconstruct flame light field via Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2412.19841)]
* GlossGau: Efficient Inverse Rendering for Glossy Surface with Anisotropic Spherical Gaussian, *arXiv*. [[Paper](https://arxiv.org/abs/2502.14129)]
### 1.8 Foundation Model<a id="1.8-Foundation-Model"></a>
* Open-vocabulary Queryable Scene Representations for Real World Planning, **ICRA, 2023**. [[Paper](https://ieeexplore.ieee.org/abstract/document/10161534)][[Code](https://github.com/ericrosenbrown/nlmap_spot)][[Website](https://nlmap-saycan.github.io/)]
* CLIP-Fields: Weakly Supervised Semantic Fields for Robotic Memory, **RSS, 2023**. [[Paper](https://arxiv.org/abs/2210.05663)][[Code](https://github.com/notmahi/clip-fields)][[Website](https://clip-fields.github.io/)] 
* Grounding DINO: Marrying DINO with Grounded Pre-Training for Open-Set Object Detection, **ECCV, 2024**. [[Paper](https://www.ecva.net/papers/eccv_2024/papers_ECCV/papers/06319.pdf)][[Code](https://github.com/IDEA-Research/GroundingDINO)]
* YOLO-World: Real-Time Open-Vocabulary Object Detection, **CVPR, 2024**. [[Paper](https://openaccess.thecvf.com/content/CVPR2024/papers/Cheng_YOLO-World_Real-Time_Open-Vocabulary_Object_Detection_CVPR_2024_paper.pdf)][[Code](https://github.com/AILab-CVC/YOLO-World)][[Website](https://wondervictor.github.io/)]
* YOLOE:Real-Time Seeing Anything, **ICCV, 2025**. [[Paper](https://openaccess.thecvf.com/content/ICCV2025/supplemental/Wang_YOLOE_Real-Time_Seeing_ICCV_2025_supplemental.pdf)][[Code](https://github.com/THU-MIG/yoloe)]
* Scene-LLM: Extending Language Model for 3D Visual Reasoning, **WACV, 2025**. [[Paper](https://openaccess.thecvf.com/content/WACV2025/papers/Fu_Scene-LLM_Extending_Language_Model_for_3D_Visual_Reasoning_WACV_2025_paper.pdf)]

## 2.Mapping<a id="mapping"></a>
### 2.1 Point Cloud<a id="2.1-Point-Cloud"></a>
- ElasticFusion: Real-time dense SLAM and light source estimation, **Int J Rob Res, 2016**. [[Website](https://journals.sagepub.com/doi/10.1177/0278364916669237)]
- COLMAP: Structure-from-Motion Revisited, **CVPR, 2016**. [[Website](https://ieeexplore.ieee.org/document/7780814)]
- QuadricSLAM: Dual Quadrics as SLAM Landmarks, **CVPR, 2018**. [[Paper](https://openaccess.thecvf.com/content_cvpr_2018_workshops/papers/w9/Nicholson_QuadricSLAM_Dual_Quadrics_CVPR_2018_paper.pdf)]
- CubeSLAM: Monocular 3-D Object SLAM, **TRO, 2019**. [[Website](https://ieeexplore.ieee.org/document/8708251)]
- ConceptFusion: Open-set Multimodal 3D Mapping. *arxiv*. [[Paper](https://openreview.net/pdf?id=zEyavwx3qf)]

### 2.2 Voxel Grid<a id="2.2-Voxel-Grid"></a>
- OctoMap: AnEfficient Probabilistic 3D Mapping Framework Based on Octrees, **AUTON ROBOT, 2013**. [[Paper](https://courses.cs.washington.edu/courses/cse571/16au/slides/hornung13auro.pdf)]
- Efficient and Probabilistic Adaptive Voxel Mapping for Accurate Online LiDAR Odometry, **RAL, 2022**. [[Website](https://ieeexplore.ieee.org/document/9813516)]
- LiDAR Road-Atlas: An Efficient Map Representation for General 3D Urban Environment, **Field Rob, 2025**. [[Website](https://ieeexplore.ieee.org/document/10876093)]

### 2.3 Signed Distance Field (SDF)<a id="2.3-Signed-Distance-Field(SDF)"></a>
- KinectFusion: Real-time dense surface mapping and tracking, **ISMAR, 2011**. [[Website](https://ieeexplore.ieee.org/document/6162880)]
- Voxgraph: Globally Consistent, Volumetric Mapping using Signed Distance Function Submaps, **RAL, 2019**. [[Website](https://arxiv.org/abs/2004.13154)]

### 2.4 Mesh<a id="2.4-Mesh"></a>
- Kimera: from SLAM to Spatial Perception with 3D Dynamic Scene Graphs, **INT J ROBOT RES, 2021**. [[Paper](https://arxiv.org/abs/2101.06894)]

### 2.5 Scene Graph<a id="2.5-Scene-Graph"></a>
- Hydra: A Real-time Spatial Perception System for 3D Scene Graph Construction and Optimization, **RSS, 2022**. [[Paper](https://www.roboticsproceedings.org/rss18/p050.pdf)]
- ConceptGraphs: Open-Vocabulary 3D Scene Graphs for Perception and Planning, **ICRA, 2024**. [[Website](https://arxiv.org/abs/2309.16650)]
- Clio: Real-Time Task-Driven Open-Set 3D Scene Graphs, **RAL, 2024**. [[Website](https://ieeexplore.ieee.org/document/10659066)]

### 2.6 Neural Radiance Fields (NeRF)<a id="2.6-Neural-Radiance-Fields(NeRF)"></a>

#### 2.6.1 SLAM
- **NeuralRecon**: Real-Time Coherent 3D Reconstruction from Monocular Video, *CVPR, 2021*.[[Paper](https://arxiv.org/pdf/2104.00681.pdf)] [[Pytorch Code](https://github.com/zju3dv/NeuralRecon/)] [[Website](https://zju3dv.github.io/neuralrecon/)]
- **Di-fusion**: Online implicit 3d reconstruction with deep priors, *CVPR, 2021*.[[Paper](https://openaccess.thecvf.com/content/CVPR2021/papers/Huang_DI-Fusion_Online_Implicit_3D_Reconstruction_With_Deep_Priors_CVPR_2021_paper.pdf)] [[Pytorch Code](https://github.com/huangjh-pub/di-fusion)]
* **iSDF**: Real-Time Neural Signed Distance Fields for Robot Perception, *RSS, 2022*. [[Paper](https://arxiv.org/abs/2204.02296)] [[Pytorch Code](https://github.com/facebookresearch/iSDF)] [[Website](https://joeaortiz.github.io/iSDF/)]
* **LENS**: LENS: Localization enhanced by NeRF synthesis, *CoRL, 2021*. [[Paper](https://arxiv.org/abs/2110.06558)] [[Video](https://www.youtube.com/watch?v=DgIpVoS6ejY)] 
* **NICE-SLAM**: Neural Implicit Scalable Encoding for SLAM, *CVPR, 2021*. [[Paper](https://arxiv.org/abs/2112.12130)] [[Pytorch Code](https://github.com/cvg/nice-slam)] [[Website](https://pengsongyou.github.io/nice-slam?utm_source=catalyzex.com)]
* **iMAP**: Implicit Mapping and Positioning in Real-Time, *ICCV, 2021*. [[Paper](https://arxiv.org/abs/2103.12352)] [[Website](https://edgarsucar.github.io/iMAP/)] [[Video](https://www.youtube.com/watch?v=c-zkKGArl5Y)] 
* **BNV-Fusion**: BNV-Fusion: Dense 3D Reconstruction using Bi-level Neural Volume Fusion, *CVPR, 2022*. [[Paper](https://arxiv.org/pdf/2204.01139.pdf)] [[Pytorch Code](https://github.com/likojack/bnv_fusion)]
* **NeRF-SLAM**: Real-Time Dense Monocular SLAM with Neural Radiance Fields, *IROS, 2023*. [[Paper](https://arxiv.org/pdf/2210.13641.pdf)] [[Pytorch Code](https://github.com/ToniRV/NeRF-SLAM)] [[Video](https://www.youtube.com/watch?v=-6ufRJugcEU)]
* **Nerfels**: Renderable Neural Codes for Improved Camera Pose Estimation, *CVPR 2022 Workshop*. [[Paper](https://openaccess.thecvf.com/content/CVPR2022W/IMW/papers/Avraham_Nerfels_Renderable_Neural_Codes_for_Improved_Camera_Pose_Estimation_CVPRW_2022_paper.pdf)]
* SDF-based RGB-D Camera Tracking in Neural Scene Representations, *ICRA Workshop, 2022*. [[Paper](https://neural-implicit-workshop.stanford.edu/assets/pdf/bruns.pdf)]
* **Orbeez-SLAM**: A Real-time Monocular Visual SLAM with ORB Features and NeRF-realized Mapping, *ICRA, 2023*. [[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10160950)] [[Video](https://www.youtube.com/watch?v=uzb-tVcPETE)] [[Code](https://github.com/MarvinChung/Orbeez-SLAM)]
* **ESLAM**: Efficient Dense SLAM System Based on Hybrid Representation of Signed Distance Fields, *CVPR,  2023*. [[Paper](https://arxiv.org/pdf/2211.11704.pdf)]
* **Vox-Fusion**: Dense Tracking and Mapping with Voxel-based Neural Implicit Representation, *ISMAR,  2022*. [[Paper](https://arxiv.org/pdf/2210.15858.pdf)] [[Website](https://yangxingrui.com/vox-fusion/)] [[Pytorch Code](https://github.com/zju3dv/Vox-Fusion)] [[Video](https://www.youtube.com/watch?v=Prp28y1b2Qs)]
* Feature-Realistic Neural Fusion for Real-Time, Open Set Scene Understanding, *ICRA,  2022*. [[Paper](https://arxiv.org/pdf/2210.03043.pdf)]  [[Website](https://yangxingrui.com/vox-fusion/)] [[Video](https://www.youtube.com/watch?v=ysaohKI_Pf0)]
* Dense RGB SLAM with Neural Implicit Maps, *ICLR, 2023*. [[Paper](https://arxiv.org/pdf/2301.08930v1.pdf)] [[Website](https://poptree.github.io/DIM-SLAM/)] [[Code](https://github.com/HKUST-3DV/DIM-SLAM)] [[Video]()]
* **vMAP**: Vectorised Object Mapping for Neural Field SLAM, *CVPR,  2023*. [[Paper](https://arxiv.org/pdf/2302.01838.pdf)] [[Website](https://kxhit.github.io/vMAP)] [[Pytorch Code](https://github.com/kxhit/vMAP)] [[Video](https://kxhit.github.io/media/vMAP/vmap_raw.mp4)]
* **NICER-SLAM**: Neural Implicit Scene Encoding for RGB SLAM, *3DV 2024*. [[Paper](https://arxiv.org/pdf/2302.03594.pdf)] [[Video](https://www.youtube.com/watch?v=tUXzqEZWg2w)]
* Implicit Map Augmentation for Relocalization, *ECCV Workshop, 2022*. [[Paper](https://link.springer.com/chapter/10.1007/978-3-031-25066-8_36)]
* **Uni-Fusion**: Universal Continuous Mapping, *TRO, 2023*.[[Paper](https://arxiv.org/pdf/2303.12678.pdf)] [[Code](https://github.com/Jarrome/Uni-Fusion)] [[Website](https://jarrome.github.io/Uni-Fusion/)]
* **NEWTON**: Neural View-Centric Mapping for On-the-Fly Large-Scale SLAM, *RAL, 2024*. [[Paper](https://arxiv.org/pdf/2303.13654v1.pdf)]
* **Point-SLAM**: Dense Neural Point Cloud-based SLAM, *ICCV, 2023*. [[Paper](https://arxiv.org/pdf/2304.04278.pdf)] [[Code](https://github.com/tfy14esa/Point-SLAM)]
* **RO-MAP**: Real-Time Multi-Object Mapping with Neural Radiance Fields, *RAL, 2023*. [[Paper](https://ieeexplore.ieee.org/document/10209177)] [[Code](https://github.com/XiaoHan-Git/RO-MAP)] [[Video](https://www.youtube.com/watch?v=sFrLXPw40wU)]
* **Co-SLAM**: Joint Coordinate and Sparse Parametric Encodings for Neural Real-Time SLAM, *CVPR, 2023*. [[Paper](https://arxiv.org/pdf/2304.14377.pdf)] [[Website](https://hengyiwang.github.io/projects/CoSLAM)]
* Neural Implicit Dense Semantic SLAM, *arXiv, 2023*. [[Paper](https://arxiv.org/pdf/2304.14560.pdf)] [[Code](https://github.com/Yasaman-Haghighi/NeuralImplicitDenseSemanticSLAM)]
* **FMapping**: Factorized Efficient Neural Field Mapping for Real-Time Dense RGB SLAM, *arXiv, 2023*. [[Paper](https://arxiv.org/pdf/2306.00579v1.pdf)] [[Website](https://vlis2022.github.io/fmap/)] [[Code](https://github.com/thua919/FMapping)] 
* **UncLe-SLAM**: Uncertainty Learning for Dense Neural SLAM, *ICCVw, 2023*. [[Paper](https://arxiv.org/pdf/2306.11048.pdf)] [[Code](https://github.com/kev-in-ta/UncLe-SLAM)]
* **iMODE**:Real-Time Incremental Monocular Dense Mapping Using Neural Field, *ICRA, 2023*. [[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10161538)]
* **NISB-Map**: Scalable Mapping With Neural Implicit Spatial Block, *RAL, 2023*. [[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10163242)]
* RGB-D Mapping and Tracking in a Plenoxel Radiance Field, *WACV, 2024*. [[Paper](https://arxiv.org/pdf/2307.03404.pdf)]
* Efficient Map Fusion for Multiple Implicit SLAM Agents, *TIV, 2023*. [[Paper](https://ieeexplore.ieee.org/abstract/document/10189088)]
* **MIPS-Fusion**: Multi-Implicit-Submaps for Scalable and Robust Online Neural RGB-D Reconstruction, *TOG, 2023*. [[Paper](https://arxiv.org/pdf/2308.08741.pdf)]
* **GO-SLAM**: Global Optimization for Consistent 3D Instant Reconstruction, *ICCV, 2023*. [[Paper](https://arxiv.org/pdf/2309.02436.pdf)] [[Website](https://youmi-zym.github.io/projects/GO-SLAM/)] [[Code](https://github.com/youmi-zym/GO-SLAM)] 
* End-to-End RGB-D SLAM with Multi-MLPs Dense Neural Implicit Representations, *RAL, 2023*. [[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10238793)]
* **DynaMoN**: Motion-Aware Fast And Robust Camera Localization for Dynamic NeRF, *RAL, 2024*. [[Paper](https://arxiv.org/pdf/2309.08927.pdf)] [[Code](https://github.com/HannahHaensen/DynaMoN)] [[Website](https://hannahhaensen.github.io/DynaMoN/)]
* **HI-SLAM**: Monocular Real-time Dense Mapping with Hybrid Implicit Fields, *RAL, 2023*. [[Paper](https://arxiv.org/pdf/2310.04787.pdf)] [[Website](https://hi-slam.github.io/)] 
* **CP-SLAM**: Collaborative Neural Point-based SLAM, *NeurIPS, 2024*. [[Paper](https://openreview.net/pdf?id=dFSeZm6dTC)] [[Code](https://github.com/hjr37/CP-SLAM)]
* Learning Neural Implicit through Volume Rendering with Attentive Depth Fusion Priors,  *NeurIPS, 2023*. [[Paper](https://arxiv.org/pdf/2310.11598.pdf)] [[Code](https://github.com/MachinePerceptionLab/Attentive_DFPrior)] [[Website](https://machineperceptionlab.github.io/Attentive_DF_Prior/)]
* **NGEL-SLAM**: Neural Implicit Representation-based Global Consistent Low-Latency SLAM System, *ICRA, 2024*. [[Paper](https://arxiv.org/pdf/2311.09525.pdf)] [[Code](https://github.com/YunxuanMao/ngel_slam)] 
* **SNI-SLAM**: Semantic Neural Implicit SLAM, *CVPR, 2024*. [[Paper](https://arxiv.org/pdf/2311.11016.pdf)] [[Code](https://github.com/IRMVLab/SNI-SLAM)]
* Implicit Event-RGBD Neural SLAM, *CVPR, 2024*. [[Paper](https://arxiv.org/pdf/2311.11013.pdf)]
* **DNS SLAM**: Dense Neural Semantic-Informed SLAM, *IROS, 2024*. [[Paper](https://arxiv.org/pdf/2312.00204.pdf)][[Code](https://github.com/Li-Kunyi/dns-slam)]
* **PLGSLAM**: Progressive Neural Scene Represenation with Local to Global Bundle Adjustment, *CVPR, 2024*. [[Paper](https://arxiv.org/pdf/2312.09866.pdf)] [[Code](https://github.com/dtc111111/plgslam)]
* **NeRF-VO**: Real-Time Sparse Visual Odometry with Neural Radiance Fields, *RAL, 2024*. [[Paper](https://arxiv.org/pdf/2312.13471.pdf)]
* Ternary-type Opacity and Hybrid Odometry for RGB-only NeRF-SLAM, *IROS, 2024*. [[Paper](https://arxiv.org/pdf/2312.13332.pdf)]
* **NID-SLAM**: Neural Implicit Representation-based RGB-D SLAM in dynamic environments, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2401.01189.pdf)]
* **DDN-SLAM**: Real-time Dense Dynamic Neural Implicit SLAM with Joint Semantic Encoding, *RAL, 2025*. [[Paper](https://arxiv.org/pdf/2401.01545.pdf)] [[Code](https://github.com/DrLi-Ming/DDN-SLAM)]
* **Hi-Map**: Hierarchical Factorized Radiance Field for High-Fidelity Monocular Dense Mapping, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2401.03203.pdf)] [[Website](https://vlis2022.github.io/fmap/)] [[Code](https://github.com/thua919/FMapping)]
* **NeuV-SLAM**: Fast Neural Multiresolution Voxel Optimization for RGBD Dense SLAM, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2402.02020.pdf)] [[Code](https://github.com/DARYL-GWZ/NeuV-SLAM)]
* **Loopy-SLAM**: Dense Neural SLAM with Loop Closures, *CVPR, 2024*. [[Paper](https://openaccess.thecvf.com/content/CVPR2024/papers/Liso_Loopy-SLAM_Dense_Neural_SLAM_with_Loop_Closures_CVPR_2024_paper.pdf)] [[Code](https://github.com/eriksandstroem/Loopy-SLAM)] [[Website](https://notchla.github.io/Loopy-SLAM/)]
* **Q-SLAM**: Quadric Representations for Monocular SLAM, *CoRL, 2024*. [[Paper](https://arxiv.org/pdf/2403.08125.pdf)]
* **DVN-SLAM**: Dynamic Visual Neural SLAM Based on Local-Global Encoding, *ICRA, 2025*. [[Paper](https://arxiv.org/pdf/2403.11776.pdf)]
* **H3-Mapping**: Quasi-Heterogeneous Feature Grids for Real-time Dense Mapping Using Hierarchical Hybrid Representation, *RAL, 2024*. [[Paper](https://arxiv.org/pdf/2403.10821.pdf)] [[Code](https://github.com/SYSU-STAR/H3-Mapping)]
* **Vox-Fusion++**: Voxel-based Neural Implicit Dense Tracking and Mapping with Multi-maps, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2403.12536.pdf)] [[Code](https://github.com/zju3dv/Vox-Fusion_Plus_Plus)]
* **MUTE-SLAM**: Real-Time Neural SLAM with Multiple Tri-Plane Hash Representations, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2403.17765.pdf)]
* **GlORIE-SLAM**: Globally Optimized RGB-only Implicit Encoding Point Cloud SLAM, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2403.19549.pdf)] [[Code](https://github.com/zhangganlin/GlORIE-SLAM)] [[Website](https://ganlinzhang.xyz/GlORIE-SLAM/)]
* Efficient 3D Instance Mapping and Localization with Neural Fields, *ICRA, 2024*. [[Paper](https://arxiv.org/pdf/2403.19797.pdf)] [[Website](https://gtangg12.github.io/iML/)]
* **NeSLAM**: Neural Implicit Mapping and Self-Supervised Feature Tracking With Depth Completion and Denoising, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2403.20034.pdf)] [[Code](https://github.com/dtc111111/NeSLAM)]
* **KN-SLAM**: Keypoints and Neural Implicit Encoding SLAM, *TIM, 2024*. [[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10474286)]
* **SLAIM**: Robust Dense Neural SLAM for Online Tracking and Mapping, *CVPRw, 2024*. [[Paper](https://arxiv.org/pdf/2404.11419.pdf)] [[Code](https://github.com/vincentcartillier/SLAIM/)] [[Website](https://vincentcartillier.github.io/slaim.html)]
* **EC-SLAM**: Real-time Dense Neural RGB-D SLAM System with Effectively Constrained Global Bundle Adjustment, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2404.13346.pdf)] [[Code](https://github.com/Lightingooo/EC-SLAM)]
* **S3-SLAM**: Sparse Tri-plane Encoding for Neural Implicit SLAM, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2404.18284)]
* **DF-SLAM**: Neural Feature Rendering Based on Dictionary Factors Representation for High-Fidelity Dense Visual SLAM System, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2404.17876)] [[Code](https://github.com/funcdecl/DF-SLAM)]
* Neural Graph Mapping for Dense SLAM with Efficient Loop Closure, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2405.03633)] [[Code](https://github.com/KTH-RPL/neural_graph_mapping)] [[Website](https://kth-rpl.github.io/neural_graph_mapping/)]
* **VPE-SLAM**: Neural Implicit Voxel-Permutohedral Encoding for SLAM, *ICRA, 2024*. [[Paper](todo)] [[Code](https://github.com/NeuCV-IRMI/VPE-SLAM)]
* **ONeK-SLAM**: A Robust Object-Level Dense SLAM Based on Joint Neural Radiance Fields and Keypoints, *ICRA 2024*. [[Paper](todo)]
* **HERO-SLAM**: Hybrid Enhanced Robust Optimization of Neural SLAM, *ICRA, 2024*. [[Paper](https://arxiv.org/pdf/2407.18813)] [[Code](https://github.com/hero-slam/HERO-SLAM)] [[Website](https://hero-slam.github.io/)]
* **NeB-SLAM**: Neural Blocks-based Salable RGB-D SLAM for Unknown Scenes, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2405.15151)]
* **ENeRF-SLAM**:A Dense Endoscopic SLAM With Neural Implicit Representation, *TMRB, 2024*. [[Paper](https://ieeexplore.ieee.org/abstract/document/10542414)] [[Code](https://github.com/Mar-lll/ENeRF-SLAM)]
* IBD-SLAM: Learning Image-Based Depth Fusion for Generalizable SLAM, *CVPR, 2024*. [[Paper](https://openaccess.thecvf.com/content/CVPR2024/papers/Yin_IBD-SLAM_Learning_Image-Based_Depth_Fusion_for_Generalizable_SLAM_CVPR_2024_paper.pdf)] [[Website](https://visual-ai.github.io/ibd-slam)]
* **RoDyn-SLAM**: Robust Dynamic Dense RGB-D SLAM with Neural Radiance Fields, *RAL, 2024*. [[Paper](https://arxiv.org/pdf/2407.01303)] [[Code](https://github.com/fudan-zvg/Rodyn-SLAM)]
* **MoD-SLAM**: Monocular Dense Mapping for Unbounded 3D Scene Reconstruction,  *RAL, 2024*. [[Paper](https://arxiv.org/pdf/2402.03762.pdf)]
* Evaluating geometric accuracy of NeRF reconstructions compared to SLAM method,  *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2407.11238)]
* **I2-SLAM**: Inverting Imaging Process for Robust Photorealistic Dense SLAM,  *ECCV, 2024*. [[Paper](https://arxiv.org/abs/2407.11347v1)]
* **TivNe-SLAM**: Dynamic Mapping and Tracking via Time-Varying Neural Radiance Fields,  *IROS, 2024*. [[Paper](https://arxiv.org/pdf/2310.18917v4)]
* **NIS-SLAM**: Neural Implicit Semantic RGB-D SLAM for 3D Consistent Scene Understanding,  *TVCG, 2024*. [[Paper](https://arxiv.org/pdf/2407.20853)] [[Website](https://zju3dv.github.io/nis_slam/)]
* **DDS-SLAM**: Dense Semantic Neural SLAM for Deforming Endoscopic Scenes, *IROS, 2024*. [Paper] [[Code](https://github.com/IRMVLab/DDS-SLAM)]
* **FI-SLAM**: Feature Fusion and Instance Reconstruction for Neural Implicit SLAM,  *IROS, 2024*. [[Paper](https://ieeexplore.ieee.org/abstract/document/10802296)] [Code]
* **LCP-Fusion**: A Neural Implicit SLAM with Enhanced Local Constraints and Computable Prior,  *IROS, 2024*. [[Paper](https://arxiv.org/pdf/2411.03610)] [[Code](https://github.com/laliwang/LCP-Fusion)]
* **NF-SLAM**: Effective, Normalizing Flow-supported Neural Field representations for object-level visual SLAM in automotive applications, *IROS, 2024*. [[Paper](https://ieeexplore.ieee.org/abstract/document/10801421)] [Code]
* **EvenNICER-SLAM**: Event-based Neural Implicit Encoding SLAM,  *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2410.03812)] [[Code](https://github.com/cs-vision/EvenNICER-SLAM)]
* **NVINS**: Robust Visual Inertial Navigation Fused with NeRF-augmented Camera Pose Regressor and Uncertainty Quantification, *IROS, 2024*. [[Paper](https://arxiv.org/pdf/2404.01400)]
* Optimizing NeRF-based SLAM with Trajectory Smoothness Constraints, *ICRA, 2025*. [[Paper](https://arxiv.org/pdf/2410.08780)]
* **LRSLAM**: Low-rank Representation of Signed Distance Fields in Dense Visual SLAM System, *ECCV, 2024*. [[Paper](https://www.ecva.net/papers/eccv_2024/papers_ECCV/papers/10364.pdf)]
* Bridging the Gap Between Explicit and Implicit Representations: Cross-Data Association for VSLAM, *TITS, 2024*. [[Paper](https://ieeexplore.ieee.org/abstract/document/10738129)]
* **MBA-SLAM**: Motion Blur Aware Dense Visual SLAM with Radiance Fields Representation, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2411.08279)] [[Code](https://github.com/WU-CVGL/MBA-SLAM)] [[Website](https://wangpeng000.github.io/MBA-SLAM/)]
* **Uni-SLAM**: Uncertainty-Aware Neural Implicit SLAM for Real-Time Dense Indoor Scene Reconstruction, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2412.00242)] [[Website](https://shaoxiang777.github.io/project/uni-slam/)]
* **iS-MAP**: Neural Implicit Mapping and Positioning for Structural Environments, *ACCV, 2024*. [[Paper](https://openaccess.thecvf.com/content/ACCV2024/papers/Wang_iS-MAP_Neural_Implicit_Mapping_and_Positioning_for_Structural_Environments_ACCV_2024_paper.pdf)] [[Code](https://github.com/00Haocheng/iS-MAP)]
- Query Quantized Neural SLAM, *AAAI, 2025*. [[Paper](https://arxiv.org/pdf/2412.16476)] [[Code](https://github.com/MachinePerceptionLab/QQ-SLAM)] [[Website](https://machineperceptionlab.github.io/QQ-SLAM-page/)]
- Hierarchical Pose Estimation and Mapping with Multi-scale Neural Feature Fields, *IRC, 2024*. [[Paper](https://arxiv.org/pdf/2412.20976)]
- **Mee-SLAM**: Memory efficient endoscopic RGB SLAM with implicit scene representation, *Expert Systems with Applications, 2025*. [[Paper](https://www.sciencedirect.com/science/article/abs/pii/S0957417424031026)]
- **Bayesian NeRF**: Quantifying Uncertainty with Volume Density for Neural Implicit Fields, *RAL, 2025*. [[Paper](https://ieeexplore.ieee.org/abstract/document/10829678)]
- **SP-SLAM**: Neural Real-Time Dense SLAM With Scene Priors, *TCSVT, 2025*. [[Paper](https://ieeexplore.ieee.org/abstract/document/10830563)]
- **SLC2-SLAM**: Semantic-guided Loop Closure with Shared Latent Code for NeRF SLAM, *RAL, 2025*. [[Paper](https://arxiv.org/pdf/2501.08880)]
- Category-level Meta-learned NeRF Priors for Efficient Object Mapping, *IROS, 2025*. [[Paper](https://arxiv.org/pdf/2503.01582)]
- **Proud-SLAM**: Neural Point-based Hybrid RGBD Monocular Dense SLAM, *ICASSP, 2025*. [[Paper](https://ieeexplore.ieee.org/abstract/document/10888965)]
- **NeRF-VIO**: Map-Based Visual-Inertial Odometry with Initialization Leveraging Neural Radiance Fields, *arXiv, 2025*. [[Paper](https://arxiv.org/pdf/2503.07952)]
- **HS-SLAM**: Hybrid Representation with Structural Supervision for Improved Dense SLAM, *ICRA, 2025*. [[Paper](https://arxiv.org/pdf/2503.21778)] [[Website](https://zorangong.github.io/HS-SLAM/)]
- Region sampling NeRF-SLAM based on Kolmogorov-Arnold network, *arXiv, 2025*. [[Paper](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0325024)] [[Code](https://github.com/GXXXXXT/RSNeRF/)]
- **NDF-SLAM**: LiDAR SLAM based on neural distance field for registration and loop closure detection, *Measurement, 2025*. [[Paper](https://www.sciencedirect.com/science/article/abs/pii/S0263224125012631)]
- **MISO**: Multiresolution Submap Optimization for Efficient Globally Consistent Neural Implicit Reconstruction, *RSS, 2025*. [[Paper](https://arxiv.org/pdf/2504.19104)] [[Code](https://github.com/ExistentialRobotics/MISO)] [[Website](https://existentialrobotics.org/miso_rss25/)]
- Monocular Visual SLAM with Adjusting Neural Radiance Fields for 3D Reconstruction in Planetary Environments, *TGRS, 2025*. [[Paper](https://ieeexplore.ieee.org/abstract/document/11023632)]
- **EC-SLAM**: Effectively constrained neural RGB-D SLAM with TSDF hash encoding and joint optimization, *PR, 2025*. [[Paper](https://www.sciencedirect.com/science/article/abs/pii/S0031320325006946)] [[Code](https://github.com/Lightingooo/EC-SLAM)]
- Spatial Coordinate Transformation for 3D Neural Implicit Mapping, *RAL, 2025*. [[Paper](https://ieeexplore.ieee.org/abstract/document/11106682)] [[Code](https://github.com/Lab-of-AI-and-Robotics/SCT_NIM)]
- SDF-Guided Keyframe Selection: Novel Boost for NeRF SLAM Loop Closure, *IROS, 2025*. [[Paper](https://ieeexplore.ieee.org/document/11246937)]
- **SLC^2-SLAM**: Semantic-Guided Loop Closure Using Shared Latent Code for NeRF SLAM, *IROS, 2025*. [[Paper](https://ieeexplore.ieee.org/document/10935649/)]
- **MARVO**: Marine-Adaptive Radiance-aware Visual Odometry, *arXiv, 2025*. [[Paper](https://arxiv.org/pdf/2511.22860)]

#### 2.6.2 Scene Reconstruction


### 2.7 3D Gaussian Splatting (3DGS)<a id="2.7-3D-Gaussian-Splatting(3DGS)"></a>

#### 2.7.1 SLAM
* HGS-Mapping: Online Dense Mapping Using Hybrid Gaussian Representation in Urban Scenes, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2403.20159.pdf)]
* MM-Gaussian: 3D Gaussian-based Multi-modal Fusion for Localization and Reconstruction in Unbounded Scenes, *arXiv*. [[Paper](https://arxiv.org/pdf/2404.04026)]
* GSFusion: Online RGB-D Mapping Where Gaussian Splatting Meets TSDF Fusion, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.12677.pdf)]
* LoopSplat: Loop Closure by Registering 3D Gaussian Splats, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.10154.pdf)]
* SGS-SLAM: Semantic Gaussian Splatting For Neural Dense SLAM,  **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2402.03246.pdf)] [[Code](https://github.com/ShuhongLL/SGS-SLAM)]
* Compact 3D Gaussian Splatting For Dense Visual SLAM, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2403.11247.pdf)] [[Code](https://github.com/dtc111111/Compact_GSSLAM)]
* NGM-SLAM: Gaussian Splatting SLAM with Radiance Field Submap, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2405.05702)]
* GGRt: Towards Generalizable 3D Gaussians without Pose Priors in Real-Time, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.10147)] [[Website](https://3d-aigc.github.io/GGRt/)]
* MGS-SLAM: Monocular Sparse Tracking and Gaussian Mapping with Depth Smooth Regularization, *arXiv 2024*. [[Paper](https://arxiv.org/pdf/2405.06241)]
* GS-SLAM: Dense Visual SLAM with 3D Gaussian Splatting, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2311.11700.pdf)]
* Photo-SLAM: Real-time Simultaneous Localization and Photorealistic Mapping for Monocular, Stereo, and RGB-D Cameras, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2311.16728.pdf)]
* SplaTAM: Splat, Track & Map 3D Gaussians for Dense RGB-D SLAM, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2312.02126.pdf)] [[Website](https://spla-tam.github.io/)] [[Code](https://github.com/spla-tam/SplaTAM)]
* Gaussian Splatting SLAM, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2312.06741.pdf)] [[Code](https://github.com/muskie82/MonoGS)] [[Website](https://rmurai.co.uk/projects/GaussianSplattingSLAM/)]
* Gaussian-SLAM: Photo-realistic Dense SLAM with Gaussian Splatting, *arXiv, 2023*. [[Paper](https://arxiv.org/pdf/2312.10070.pdf)] [[Code](https://github.com/VladimirYugay/Gaussian-SLAM)] [[Website](https://vladimiryugay.github.io/gaussian_slam/)]
* SemGauss-SLAM: Dense Semantic Gaussian Splatting SLAM, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2403.07494.pdf)]
* NEDS-SLAM: A Novel Neural Explicit Dense Semantic SLAM Framework using 3D Gaussian Splatting, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2403.11679.pdf)]
* High-Fidelity SLAM Using Gaussian Splatting with Rendering-Guided Densification and Regularized Optimization, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2403.12535.pdf)]
* RGBD GS-ICP SLAM, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2403.12550.pdf)] [[Code](https://github.com/Lab-of-AI-and-Robotics/GS_ICP_SLAM)] [[Video](https://www.youtube.com/watch?v=e-bHh_uMMxE)]
* EndoGSLAM: Real-Time Dense Reconstruction and Tracking in Endoscopic Surgeries using Gaussian Splatting, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2403.15124.pdf)] [[Website](https://endogslam.loping151.com/)] [[Code](https://github.com/Loping151/EndoGSLAM)]
* CG-SLAM: Efficient Dense RGB-D SLAM in a Consistent Uncertainty-aware 3D Gaussian Field, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2403.16095.pdf)] [[Code](https://github.com/hjr37/CG-SLAM)] [[Website](https://zju3dv.github.io/cg-slam/)]
* RTG-SLAM: Real-time 3D Reconstruction at Scale using Gaussian Splatting, **SIGGRAPH, 2024**. [[Paper](https://arxiv.org/pdf/2404.19706)] [[Code](https://github.com/MisEty/RTG-SLAM)]
* MotionGS: Compact Gaussian Splatting SLAM by Motion Filter, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2405.11129)] [[Code](https://github.com/Antonio521/MotionGS)]
* Monocular Gaussian SLAM with Language Extended Loop Closure, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2405.13748)]
* Splat-SLAM: Globally Optimized RGB-only SLAM with 3D Gaussians, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2405.16544)] [[Code](https://github.com/eriksandstroem/Splat-SLAM)]
* MG-SLAM: Structure Gaussian SLAM with Manhattan World Hypothesis, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2405.20031)]
* TAMBRIDGE: Bridging Frame-Centered Tracking and 3D Gaussian Splatting for Enhanced SLAM, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2405.19614)] [[Code](https://github.com/ZeldaFromHeaven/TAMBRIDGE-DAVID)] [[Website](https://zeldafromheaven.github.io/TAMBRIDGE/)]
* IG-SLAM: Instant Gaussian SLAM, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.01126)]
* Visual SLAM with 3D Gaussian Primitives and Depth Priors Enabling Novel View Synthesis, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.05635)]
* Towards Real-Time Gaussian Splatting: Accelerating 3DGS through Photometric SLAM, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.05635)]
* OG-Mapping: Octree-based Structured 3DGaussians for Online Dense Mapping, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.17223)]
* 3DGS-Calib: 3D Gaussian Splatting for Multimodal SpatioTemporal Calibration, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.11577)] [[Website](https://arxiv.org/abs/2403.11577)]
* COLMAP-Free 3D Gaussian Splatting, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2312.07504.pdf)]
* 6DGS: 6D Pose Estimation from a Single Image and a 3D Gaussian Splatting Model, **ECCV, 2024**. [[Paper](https://arxiv.org/abs/2407.15484)] [[Code](https://github.com/mbortolon97/6dgs)]
* Hi-SLAM: Scaling-up Semantics in SLAM with a Hierarchically Categorical Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.12518)]
* GLC-SLAM: Gaussian Splatting SLAM with Efficient Loop Closure, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.10982)]
* AG-SLAM: Active Gaussian Splatting SLAM, *arXiv*. [[Paper](https://arxiv.org/pdf/2410.17422.pdf)]
* DG-SLAM: Robust Dynamic Gaussian Splatting SLAM with Hybrid Pose Optimization, *arXiv*. [[Paper](https://arxiv.org/abs/2411.08373)]
* LiV-GS: LiDAR-Vision Integration for 3D Gaussian Splatting SLAM in Outdoor Environments, *arXiv*. [[Paper](https://arxiv.org/abs/2411.12185)]
* DGS-SLAM: Gaussian Splatting SLAM in Dynamic Environment, *arXiv*. [[Paper](https://arxiv.org/abs/2411.10722)]
* DeSiRe-GS: 4D Street Gaussians for Static-Dynamic Decomposition and Surface Reconstruction for Urban Driving Scenes, *arXiv*. [[Paper](https://arxiv.org/abs/2411.11921)]
* GaussianPretrain: A Simple Unified 3D Gaussian Representation for Visual Pre-training in Autonomous Driving, *arXiv*. [[Paper](https://arxiv.org/abs/2411.12452)]
* HI-SLAM2: Geometry-Aware Gaussian SLAM for Fast Monocular Scene Reconstruction, *arXiv*. [[Paper](https://arxiv.org/abs/2411.17982)]
* DROID-Splat: Combining end-to-end SLAM with 3D Gaussian Splatting, *arXiv*. [[Code](https://github.com/ChenHoy/DROID-Splat)]
* PG-SLAM: Photo-realistic and Geometry-aware RGB-D SLAM in Dynamic Environments, *arXiv*. [[Paper](https://arxiv.org/abs/2411.15800)]
* Gassidy: Gaussian Splatting SLAM in Dynamic Environments, *arXiv*. [[Paper](https://arxiv.org/abs/2411.15476)]
* SplatAD: Real-Time Lidar and Camera Rendering with 3D Gaussian Splatting for Autonomous Driving, *arXiv*. [[Paper](https://arxiv.org/abs/2411.16816)]
* MAC-Ego3D: Multi-Agent Gaussian Consensus for Real-Time Collaborative Ego-Motion and Photorealistic 3D Reconstruction, *arXiv*. [[Paper](https://arxiv.org/abs/2412.09723)]
* RP-SLAM: Real-time Photorealistic SLAM with Efficient 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2412.09868)]
* RGBDS-SLAM: A RGB-D Semantic Dense SLAM Based on 3D Multi Level Pyramid Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2412.01217)]
* FlashSLAM: Accelerated RGB-D SLAM for Real-Time 3D Scene Reconstruction with Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2412.00682)]
* NeRF and Gaussian Splatting SLAM in the Wild, *arXiv*. [[Paper](https://arxiv.org/abs/2412.03263)]
* GSplatLoc: Ultra - Precise Camera Localization via 3D Gaussian Splatting, *arXiv*. [[Paper](https://www.arxiv.org/abs/2412.20056)]
* CityLoc: 6 DoF Localization of Text Descriptions in Large-Scale Scenes with Gaussian Representation, *arXiv*. [[Paper](https://arxiv.org/abs/2501.08982)]
* VINGS-Mono: Visual-Inertial Gaussian Splatting Monocular SLAM in Large Scenes, *arXiv*. [[Paper](https://arxiv.org/abs/2501.08286)]
* Scaffold-SLAM: Structured 3D Gaussians for Simultaneous Localization and Photorealistic Mapping, *arXiv*. [[Paper](https://arxiv.org/abs/2501.05242)]
* PanoSLAM: Panoptic 3D Scene Reconstruction via Gaussian SLAM, *arXiv*. [[Paper](https://arxiv.org/abs/2501.00352)]
* GS-LiDAR: Generating Realistic LiDAR Point Clouds with Panoramic Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2501.13971)]
* GeomGS: LiDAR-Guided Geometry-Aware Gaussian Splatting for Robot Localization, *arXiv*. [[Paper](https://arxiv.org/abs/2501.13417)]
* VIGS SLAM: IMU-based Large-Scale 3D Gaussian Splatting SLAM, *arXiv*. [[Paper](https://arxiv.org/abs/2501.13402)]
* Advancing Dense Endoscopic Reconstruction with Gaussian Splatting-driven Surface Normal-aware Tracking and Mapping, *arXiv*. [[Paper](https://arxiv.org/abs/2501.19319)]
* DenseSplat: Densifying Gaussian Splatting SLAM with Neural Radiance Prior, *arXiv*. [[Paper](https://arxiv.org/abs/2502.09111)]
* GARAD-SLAM: 3D GAussian splatting for Real-time Anti Dynamic SLAM, *arXiv*. [[Paper](https://arxiv.org/abs/2502.03228)]
* PINGS: Gaussian Splatting Meets Distance Fields within a Point-Based Implicit Neural Map, *arXiv*. [[Paper](https://arxiv.org/abs/2502.05752)]
* SIREN: Semantic, Initialization-Free Registration of Multi-Robot Gaussian Splatting Maps, *arXiv*. [[Paper](https://arxiv.org/abs/2502.06519)]
* Multi-Modal Neural Radiance Field for Monocular Dense SLAM with a Light-Weight ToF Sensor, **ICCV, 2023**. [[Paper](https://arxiv.org/pdf/2308.14383.pdf)] [[Website](https://zju3dv.github.io/tof_slam/)] [[Code](https://github.com/zju3dv/tof_slam)]
* LIV-GaussMap: LiDAR-Inertial-Visual Fusion for Real-time 3D Radiance Field Map Rendering, **RAL, 2024**. [[Paper](https://arxiv.org/pdf/2401.14857.pdf)] [[Code](https://github.com/sheng00125/LIV-GaussMap)]
* MM3DGS SLAM: Multi-modal 3D Gaussian Splatting for SLAM Using Vision, Depth, and Inertial Measurements, **IROS, 2024**. [[Paper](https://arxiv.org/pdf/2404.00923.pdf)] [[Website](https://vita-group.github.io/MM3DGS-SLAM/)]
* MM-Gaussian: 3D Gaussian-based Multi-modal Fusion for Localization and Reconstruction in Unbounded Scenes, **IROS, 2024**. [[Paper](https://arxiv.org/pdf/2404.04026.pdf)]
* Gaussian-LIC: Photo-realistic LiDAR-Inertial-Camera SLAM with 3D Gaussian Splatting, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2404.06926.pdf)]
* Go-SLAM: Grounded Object Segmentation and Localization with Gaussian Splatting SLAM, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2409.16944.pdf)]


#### 2.7.2 Scene Reconstruction

* VastGaussian: Vast 3D Gaussians for Large Scene Reconstruction, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2402.17427.pdf)] [[Website](https://vastgaussian.github.io/)] [[Code](https://github.com/kangpeilun/VastGaussian)]
* 3DGSR: Implicit Surface Reconstruction with 3D Gaussian Splatting, **TOG 2024**. [[Paper](https://arxiv.org/pdf/2404.00409.pdf)] [[Code](https://github.com/CVMI-Lab/3DGSR)]
* A Hierarchical 3D Gaussian Representation for Real-Time Rendering of Very Large Datasets, **SIGGRAPH, 2024**. [[Paper](https://repo-sam.inria.fr/fungraph/hierarchical-3d-gaussians/hierarchical-3d-gaussians_high.pdf)] [[Website](https://repo-sam.inria.fr/fungraph/hierarchical-3d-gaussians/)]
* Fed3DGS: Scalable 3D Gaussian Splatting with Federated Learning, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.11460)] [[Code](https://github.com/DensoITLab/Fed3DGS)]
* Creating Seamless 3D Maps Using Radiance Fields, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.11364.pdf)]
* CityGaussian: Real-time High-quality Large-Scale Scene Rendering with Gaussians, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2403.20159.pdf)] [[Website](https://dekuliutesla.github.io/citygs/)]
* On Scaling Up 3D Gaussian Splatting Training, *arXiv*. [[Paper](https://arxiv.org/abs/2406.18533)] [[Website](https://daohanlu.github.io/scaling-up-3dgs/)] [[Code](https://github.com/nyu-systems/Grendel-GS)]
* HUGS: Holistic Urban 3D Scene Understanding via Gaussian Splatting, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2403.12722.pdf)] [[Code](https://xdimlab.github.io/hugs_website/)]
* SGD: Street View Synthesis with Gaussian Splatting and Diffusion Prior, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.20079.pdf)] [[Website](https://arxiv.org/abs/2403.20079)]
* Ev-GS: Event-based Gaussian splatting for Efficient and Accurate Radiance Field Rendering, *arXiv*. [[Paper](https://arxiv.org/pdf/2407.11343.pdf)]
* FlashGS: Efficient 3D Gaussian Splatting for Large-scale and High-resolution Rendering, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.07967.pdf)]
* OmniRe: Omni Urban Scene Reconstruction, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.16760.pdf)]
* GigaGS: Scaling up Planar-Based 3D Gaussians for Large Scene Surface Reconstruction, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.06685.pdf)]
* LI-GS: Gaussian Splatting with LiDAR Incorporated for Accurate Large-Scale Reconstruction, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.12899.pdf)]
* GaRField++: Reinforced Gaussian Radiance Fields for Large-Scale 3D Scene Reconstruction, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.12774.pdf)]
* EdgeGaussians -- 3D Edge Mapping via Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2409.12886)]
* DrivingForward: Feed-forward 3D Gaussian Splatting for Driving Scene Reconstruction from Flexible Surround-view Input, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.12753)]
* RenderWorld: World Model with Self-Supervised 3D Label, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.11356)]
* Drone-assisted Road Gaussian Splatting with Cross-view Uncertainty, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.15242)]
* GGS: Generalizable Gaussian Splatting for Lane Switching in Autonomous Driving, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.02382)]
* GlossyGS: Inverse Rendering of Glossy Objects with 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2410.13349)]
* L3DG: Latent 3D Gaussian Diffusion, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2410.13530.pdf)]
* PLGS: Robust Panoptic Lifting with 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2410.17505)]
* Normal-GS: 3D Gaussian Splatting with Normal-Involved Rendering, *arXiv*. [[Paper](https://arxiv.org/abs/2410.20593)]
* ODGS: 3D Scene Reconstruction from Omnidirectional Images with 3D Gaussian Splattings, *arXiv*. [[Paper](https://arxiv.org/abs/2410.20686)]
* Momentum-GS: Momentum Gaussian Self-Distillation for High-Quality Large Scene Reconstruction, *arXiv*. [[Paper](https://arxiv.org/abs/2412.04887)]
* Radiant: Large-scale 3D Gaussian Rendering based on Hierarchical Framework, *arXiv*. [[Paper](https://arxiv.org/abs/2412.05546)]
* KeyGS: A Keyframe-Centric Gaussian Splatting Method for Monocular Image Sequences, *arXiv*. [[Paper](https://arxiv.org/abs/2412.20767)]
* MVS-GS: High - Quality 3D Gaussian Splatting Mapping via Online Multi - View Stereo, *arXiv*. [[Paper](https://arxiv.org/abs/2412.19130)]
* SplatMAP: Online Dense Monocular SLAM with 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2501.07015)]
* CrossView-GS: Cross-view Gaussian Splatting For Large - scale Scene Reconstruction, *arXiv*. [[Paper](https://arxiv.org/abs/2501.01695)]
* PG-SAG: Parallel Gaussian Splatting for Fine-Grained Large-Scale Urban Buildings Reconstruction via Semantic - Aware Grouping, *arXiv*. [[Paper](https://arxiv.org/abs/2501.01677)]
* Self-Calibrating Gaussian Splatting for Large Field of View Reconstruction, *arXiv*. [[Paper](https://arxiv.org/abs/2502.09563)]
* High-Fidelity Novel View Synthesis via Splatting-Guided Diffusion, *arXiv*. [[Paper](https://arxiv.org/abs/2502.12752)]
* DHGS: Decoupled Hybrid Gaussian Splatting for Driving Scene, *arXiv*. [[Paper](https://arxiv.org/abs/2407.16600)]
* EMD: Explicit Motion Modeling for High-Quality Street Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2411.15582)]
* 4Real: Towards Photorealistic 4D Scene Generation via Video Diffusion Models, *arXiv*. [[Paper](https://arxiv.org/pdf/2406.07472.pdf)] [[Website](https://snap-research.github.io/4Real/)]
* SC4D: Sparse-Controlled Video-to-4D Generation and Motion Transfer, *arXiv*. [[Paper](https://arxiv.org/pdf/2404.03736)] [[Website](https://sc4d.github.io/)] [[Code](https://github.com/JarrentWu1031/SC4D)]
* STAG4D: Spatial-Temporal Anchored Generative 4D Gaussians, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.14939)] [[Website](https://nju-3dv.github.io/projects/STAG4D/)] [[Code](https://github.com/zeng-yifei/STAG4D)]
* TCLC-GS: Tightly Coupled LiDAR-Camera Gaussian Splatting for Surrounding Autonomous Driving Scenes, *arXiv*. [[Paper](https://arxiv.org/pdf/2404.02410.pdf)] [[Website](https://arxiv.org/abs/2404.02410)]
* EgoGaussian: Dynamic Scene Understanding from Egocentric Video with 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2406.19811)] [[Website](https://arxiv.org/abs/2406.19811)]
* Dynamic Gaussian Marbles for Novel View Synthesis of Casual Monocular Videos, *arXiv*. [[Paper](https://arxiv.org/pdf/2406.18717)] [[Website](https://arxiv.org/abs/2406.18717)]
* VGD: Vision-Only Dynamic Gaussian for Driving Simulation, *arXiv*. [[Paper](https://arxiv.org/pdf/2406.18198)] [[Website](https://arxiv.org/abs/2406.18198)]
* Modeling Ambient Scene Dynamics for Free-view Synthesis, *arXiv*. [[Paper](https://arxiv.org/pdf/2406.09395)] [[Website](https://arxiv.org/abs/2406.09395)]
* InfoGaussian: Structure-Aware Dynamic Gaussians through Lightweight Information Shaping, *arXiv*. [[Paper](https://arxiv.org/pdf/2406.05897)] [[Website](https://arxiv.org/abs/2406.05897)]
* Dynamic 3D Gaussian Fields for Urban Areas, *arXiv*. [[Paper](https://arxiv.org/pdf/2406.03175)] [[Website](https://tobiasfshr.github.io/pub/4dgf/)] [[Code](https://github.com/tobiasfshr/map4d)]
* Reconstructing and Simulating Dynamic 3D Objects with Mesh-adsorbed Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2406.01476)] [[Website](https://wcwac.github.io/MaGS-page/)] [[Code](https://github.com/wcwac/MaGS)]
* DreamPhysics: Learning Physical Properties of Dynamic 3D Gaussians with Video Diffusion Priors, *arXiv*. [[Paper](https://arxiv.org/pdf/2406.09395)] [[Website](https://arxiv.org/abs/2406.01476)] [[Code](https://github.com/tyhuang0428/DreamPhysics)]
* MoDGS: Dynamic Gaussian Splatting from Causually-captured Monocular Videos, *arXiv*. [[Paper](https://arxiv.org/pdf/2406.00434)] [[Website](https://arxiv.org/abs/2406.00434)]
* Street Gaussians for Modeling Dynamic Urban Scenes, *arXiv*. [[Paper](https://arxiv.org/pdf/2401.01339.pdf)] [[Website](https://zju3dv.github.io/street_gaussians/)] [[Code](https://github.com/zju3dv/street_gaussians)]
* DrivingGaussian: Composite Gaussian Splatting for Surrounding Dynamic Autonomous Driving Scenes, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2312.07920.pdf)] [[Website](https://pkuvdig.github.io/DrivingGaussian/)]
* HUGS: Golistic Urban 3D Scene Understanding via Gaussian Splatting, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2403.12722.pdf)] [[Website](https://xdimlab.github.io/hugs_website/)]
* Guess The Unseen: Dynamic 3D Scene Reconstruction from Partial 2D Glimpses, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2404.14410)] [[Website](https://snuvclab.github.io/gtu/)] [[Code](https://github.com/snuvclab/gtu/)]
* 4D Gaussian Splatting: Towards Efficient Novel View Synthesis for Dynamic Scenes, *arXiv*. [[Paper](https://arxiv.org/pdf/2402.03307)] [[Website](https://arxiv.org/abs/2402.03307)]
* GaussianFlow: Splatting Gaussian Dynamics for 4D Content Creation, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.12365)] [[Website](https://zerg-overmind.github.io/GaussianFlow.github.io/)] [[Code](https://github.com/Zerg-Overmind/GaussianFlow)]
* Motion-aware 3D Gaussian Splatting for Efficient Dynamic Scene Reconstruction, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.11447)] [[Website](https://arxiv.org/abs/2403.11447)]
* Bridging 3D Gaussian and Mesh for Freeview Video Rendering, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.11453)] [[Website](https://arxiv.org/abs/2403.11453)]
* Per-Gaussian Embedding-Based Deformation for Deformable 3D Gaussian Splatting, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2404.03613)] [[Website](https://jeongminb.github.io/e-d3dgs/)] [[Code](https://github.com/JeongminB/E-D3DGS)]
* 3D Geometry-aware Deformable Gaussian Splatting for Dynamic View Synthesis, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2404.06270)] [[Website](https://npucvr.github.io/GaGS/)]
* Dynamic 3D Gaussians: Tracking by Persistent Dynamic View Synthesis, **3DV, 2024**. [[Paper](https://dynamic3dgaussians.github.io/paper.pdf)] [[Website](https://dynamic3dgaussians.github.io/)] [[Code](https://github.com/JonathonLuiten/Dynamic3DGaussians)]
* Deformable 3D Gaussians for High-Fidelity Monocular Dynamic Scene Reconstruction, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2309.13101.pdf)] [[Website](https://ingra14m.github.io/Deformable-Gaussians/)] [[Code](https://github.com/ingra14m/Deformable-3D-Gaussians)]
* 4D Gaussian Splatting for Real-Time Dynamic Scene Rendering, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2310.08528.pdf)] [[Website](https://guanjunwu.github.io/4dgs/)] [[Code](https://github.com/hustvl/4DGaussians)]
* Real-time Photorealistic Dynamic Scene Representation and Rendering with 4D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2310.10642.pdf)] [[Website](https://github.com/fudan-zvg/4d-gaussian-splatting)]
* A Compact Dynamic 3D Gaussian Representation for Real-Time Dynamic View Synthesis, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2311.12897.pdf)] [[Website](https://compactdynamic3dgaussian.github.io/)] [[Code](https://github.com/raven38/EfficientDynamic3DGaussian)]
* DynMF: Neural Motion Factorization for Real-time Dynamic View Synthesis with 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2312.00112.pdf)] [[Website](https://agelosk.github.io/dynmf/)] [[Code](https://github.com/agelosk/dynmf)]
* SC-GS: Sparse-Controlled Gaussian Splatting for Editable Dynamic Scenes, **CVPR, 2024**. [[Paper](https://yihua7.github.io/SC-GS-web/materials/SC_GS_Arxiv.pdf)] [[Website](https://yihua7.github.io/SC-GS-web/)] [[Code](https://github.com/yihua7/SC-GS)]
* Gaussian-Flow: 4D Reconstruction with Dynamic 3D Gaussian Particle, *CVPR, 2024*. [[Paper](https://arxiv.org/pdf/2310.08528.pdf)] [[Website](https://nju-3dv.github.io/projects/Gaussian-Flow)]
* GauFRe: Gaussian Deformation Fields for Real-time Dynamic Novel View Synthesis, *arXiv*. [[Paper](https://arxiv.org/pdf/2312.11458.pdf)] [[Website](https://lynl7130.github.io/gaufre/index.html)]
* Spacetime Gaussian Feature Splatting for Real-Time Dynamic View Synthesis, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2312.16812.pdf)] [[Website](https://oppo-us-research.github.io/SpacetimeGaussians-website/)] [[Code](https://github.com/oppo-us-research/SpacetimeGaussians)]
* SWinGS: Sliding Windows for Dynamic 3D Gaussian Splatting, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2312.13308.pdf)] [[Website](https://arxiv.org/abs/2312.13308)] [[Code](https://github.com/tyhuang0428/DreamPhysics)]
* DreamGaussian4D: Generative 4D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2312.17142.pdf)] [[Website](https://jiawei-ren.github.io/projects/dreamgaussian4d/)] [[Code](https://github.com/jiawei-ren/dreamgaussian4d)]
* 4DGen: Grounded 4D Content Generation with Spatial-temporal Consistency, *arXiv*. [[Paper](https://arxiv.org/pdf/2312.17225.pdf)] [[Website](https://github.com/VITA-Group/4DGen)] [[Code](https://www.youtube.com/watch?v=-bXyBKdpQ1o)]
* Neural Parametric Gaussians for Monocular Non-Rigid Object Reconstruction, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2312.01196.pdf)]
* CoGS: Controllable Gaussian Splatting, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2312.05664.pdf)] [[Website](https://cogs2023.github.io/)]
* MD-Splatting: Learning Metric Deformation from 4D Gaussians in Highly Deformable Scenes, *arXiv*. [[Paper](https://arxiv.org/pdf/2312.00583)] [[Website](https://md-splatting.github.io/)] [[Code](https://github.com/momentum-robotics-lab/md-splatting)]
* 3DGStream: On-the-Fly Training of 3D Gaussians for Efficient Streaming of Photo-Realistic Free-Viewpoint Videos, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2403.01444.pdf)] [[Website](https://sjojok.github.io/3dgstream/)] [[Code](https://github.com/SJoJoK/3DGStream)]
* Dynamic Gaussian Splatting from Markerless Motion Capture can Reconstruct Infants Movements, **WACV, 2024**. [[Paper](https://arxiv.org/pdf/2310.19441)]
* GaussianPrediction: Dynamic 3D Gaussian Prediction for Motion Extrapolation and Free View Synthesis, **SIGGRAPH, 2024**. [[Paper](https://arxiv.org/pdf/2405.19745)] [[Website](https://arxiv.org/abs/2405.19745)] [[Code](https://github.com/BoMingZhao/GaussianPrediction)
* VEGS: View Extrapolation of Urban Scenes in 3D Gaussian Splatting using Learned Priors, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2407.02945)] [[Code](https://github.com/deepshwang/vegs)]
* Neural Parametric Gaussians for Monocular Non-Rigid Object Reconstruction, **CVPR, 2024**. [[Paper](https://arxiv.org/abs/2312.01196)]
* Gaussian Splatting LK, *arXiv*. [[Paper](https://arxiv.org/pdf/2407.11309)]
* HDRSplat: Gaussian Splatting for High Dynamic Range 3D Scene Reconstruction from Raw Images, *arXiv*. [[Paper](https://arxiv.org/pdf/2407.16503)]
* Reality Fusion: Robust Real-time Immersive Mobile Robot Teleoperation with Volumetric Visual Data Fusion, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.01225)]
* HDRGS: High Dynamic Range Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.06543)]
* S4D: Streaming 4D Real-World Reconstruction with Gaussians and 3D Control Points, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.13036)]
* DynOMo: Online Point Tracking by Dynamic Online Monocular Gaussian Reconstruction, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.02104)]
* DENSER: 3D Gaussians Splatting for Scene Reconstruction of Dynamic Urban Environments, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.10041)]
* SplatFields: Neural Gaussian Splats for Sparse 3D and 4D Reconstruction, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.11211)]
* DN-4DGS: Denoised Deformable Network with Temporal-Spatial Aggregation for Dynamic Scene Rendering, *arXiv*. [[Paper](https://arxiv.org/pdf/2410.13607)]
* MEGA: Memory-Efficient 4D Gaussian Splatting for Dynamic Scenes, *arXiv*. [[Paper](https://arxiv.org/pdf/2410.13613)]
* DriveDreamer4D: World Models Are Effective Data Machines for 4D Driving Scene Representation, *arXiv*. [[Paper](https://arxiv.org/pdf/2410.13571)]
* SpectroMotion: Dynamic 3D Reconstruction of Specular Scenes, *arXiv*. [[Paper](https://arxiv.org/pdf/2410.17249)]
* Fully Explicit Dynamic Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2410.15629)]
* Grid4D: 4D Decomposed Hash Encoding for High-fidelity Dynamic Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2410.20815)]
* 3DGS-CD: 3D Gaussian Splatting-based Change Detection for Physical Object Rearrangement, *arXiv*. [[Paper](https://arxiv.org/abs/2411.03706)]
* HiCoM: Hierarchical Coherent Motion for Streamable Dynamic Scene with 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2411.07541)]
* Adaptive and Temporally Consistent Gaussian Surfels for Multi-view Dynamic Reconstruction, *arXiv*. [[Paper](https://arxiv.org/abs/2411.06602)]
* 4D Gaussian Splatting in the Wild with Uncertainty-Aware Regularization, *arXiv*. [[Paper](https://arxiv.org/abs/2411.08879)]
* TimeFormer: Capturing Temporal Relationships of Deformable 3D Gaussians for Robust Reconstruction, *arXiv*. [[Paper](https://arxiv.org/abs/2411.11941)]
* 4D Scaffold Gaussian Splatting for Memory Efficient Dynamic Scene Reconstruction, *arXiv*. [[Paper](https://arxiv.org/abs/2411.17044)]
* Event-boosted Deformable 3D Gaussians for Fast Dynamic Scene Reconstruction, *arXiv*. [[Paper](https://arxiv.org/abs/2411.16180)]
* SplatFlow: Self-Supervised Dynamic Gaussian Splatting in Neural Motion Flow Field for Autonomous Driving, *arXiv*. [[Paper](https://arxiv.org/abs/2411.15482)]
* DynSUP: Dynamic Gaussian Splatting from An Unposed Image Pair, *arXiv*. [[Paper](https://arxiv.org/abs/2412.00851)]
* Deformable Radial Kernel Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2412.11752)]
* Template-free Articulated Gaussian Splatting for Real-time Reposable Dynamic View Synthesis, *arXiv*. [[Paper](https://arxiv.org/abs/2412.05570)]
* 4D Gaussian Splatting with Scale-aware Residual Field and Adaptive Optimization for Real-time Rendering of Temporally Complex Dynamic Scenes, *arXiv*. [[Paper](https://arxiv.org/abs/2412.06299)]
* SplineGS: Robust Motion-Adaptive Spline for Real-Time Dynamic 3D Gaussians from Monocular Video, *arXiv*. [[Paper](https://arxiv.org/abs/2412.09982)]
* RelayGS: Reconstructing Dynamic Scenes with Large-Scale and Complex Motions via Relay Gaussians, *arXiv*. [[Paper](https://arxiv.org/abs/2412.02493)]
* Monocular Dynamic Gaussian Splatting is Fast and Brittle but Smooth Motion Helps, *arXiv*. [[Paper](https://arxiv.org/abs/2412.04457)]
* Urban4D: Semantic-Guided 4D Gaussian Splatting for Urban Scene Reconstruction, *arXiv*. [[Paper](https://arxiv.org/abs/2412.03473)]
* KeyGS: A Keyframe-Centric Gaussian Splatting Method for Monocular Image Sequences, *arXiv*. [[Paper](https://arxiv.org/abs/2412.20767)]
* 4D Gaussian Splatting: Modeling Dynamic Scenes with Native 4D Primitives, *arXiv*. [[Paper](https://arxiv.org/abs/2412.20720)]
* DAS3R: Dynamics - Aware Gaussian Splatting for Static Scene Reconstruction, *arXiv*. [[Paper](https://arxiv.org/abs/2412.19518)]
* GS-LIVO: Real-Time LiDAR, Inertial, and Visual Multi-sensor Fused Odometry with Gaussian Mapping, *arXiv*. [[Paper](https://arxiv.org/abs/2501.08672)]
* MapGS: Generalizable Pretraining and Data Augmentation for Online Mapping via Novel View Synthesis, *arXiv*. [[Paper](https://arxiv.org/abs/2501.06660)]
* DreamDrive: Generative 4D Scene Modeling from Street View Images, *arXiv*. [[Paper](https://arxiv.org/abs/2501.00601)]
* GaussianVideo: Efficient Video Representation via Hierarchical Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2501.04782)]
* GS-DiT: Advancing Video Generation with Pseudo 4D Gaussian Fields through Efficient Dense 3D Point Tracking, *arXiv*. [[Paper](https://arxiv.org/abs/2501.02690)]
* Micro-macro Wavelet-based Gaussian Splatting for 3D Reconstruction from Unconstrained Images, *arXiv*. [[Paper](https://arxiv.org/abs/2501.14231)]
* OG-Gaussian: Occupancy Based Street Gaussians for Autonomous Driving, *arXiv*. [[Paper](https://arxiv.org/abs/2502.14235)]


### 2.8 Foundation Model<a id="2.8-Foundation-Model></a>
- CUT3R: Continuous 3D Perception Model with Persistent State, **CVPR, 2025**. [[Paper](https://arxiv.org/pdf/2501.12387)]
- Pow3R: Empowering Unconstrained 3D Reconstruction with Camera and Scene Priors, **CVPR, 2025**. [[Paper](https://openaccess.thecvf.com/content/CVPR2025/papers/Jang_Pow3R_Empowering_Unconstrained_3D_Reconstruction_with_Camera_and_Scene_Priors_CVPR_2025_paper.pdf)]
- MASt3R: Grounding Image Matching in 3D with MASt3R, **CVPR, 2025**. [[Website](https://arxiv.org/abs/2406.09756)]
- MUSt3R: Multi-view Network for Stereo 3D Reconstruction, **CVPR, 2025**. [[Website](https://arxiv.org/abs/2503.01661)]
- VGGT: Visual Geometry Grounded Transformer, **CVPR, 2025**. [[Website](https://arxiv.org/abs/2503.11651v1)]
- Spann3R: 3D Reconstruction with Spatial Memory, **CVPR, 2025**. [[Paper](https://hengyiwang.github.io/projects/spanner/spann3r.pdf)]
- π3: Permutation-Equivariant Visual Geometry Learning, **arxiv**. [[Website](https://arxiv.org/abs/2507.13347)]
- DUSt3R: Geometric 3D Vision Made Easy, **CVPR, 2024**. [[Paper](https://openaccess.thecvf.com/content/CVPR2024/papers/Wang_DUSt3R_Geometric_3D_Vision_Made_Easy_CVPR_2024_paper.pdf)]

## 3.Localization<a id="localization></a>

### 3.1 Point Cloud<a id="3.1-Point-Cloud"></a>
- F-LOAM : Fast LiDAR Odometry and Mapping, **IROS, 2021**. [[Paper](https://arxiv.org/pdf/2107.00822)]
- ORB-SLAM2: an Open-Source SLAM System for Monocular, Stereo and RGB-D Cameras, **IEEE Transactions on Robotics, 2016**. [[Website](https://arxiv.org/abs/1610.06475)]
- DROID-SLAM: Deep Visual SLAM for Monocular, Stereo, and RGB-D Cameras, **NeurIPS, 2021**. [[Code](https://github.com/princeton-vl/DROID-SLAM。)]
- TEASER: Fast and Certifiable Point Cloud Registration, **IEEE Transactions on Robotics, 2021**. [[Website](https://ieeexplore.ieee.org/document/9286491)]
- KISS-ICP: In Defense of Point-to-Point ICP -- Simple, Accurate, and Robust Registration If Done the Right Way, **Robotics, 2022**. [[Website](https://arxiv.org/abs/2209.15397)]
- MonoSLAM: Real-Time Single Camera SLAM, **IEEE Transactions on Pattern Analysis and Machine Intelligence, 2007**. [[Website](https://ieeexplore.ieee.org/document/4160954)]

### 3.2 Voxel Grid<a id="3.2-Voxel-Grid"></a>
- Voxel-Based Localization and Mapping for Multirobot System in GPS-Denied Environments, **IEEE Transactions on Industrial Electronics, 2022**. [[Website](https://ieeexplore.ieee.org/abstract/document/9724114)]
- 6-DOF localization for a mobile robot using outdoor 3D voxel maps, **IEEE/RSJ International Conference on Intelligent Robots and Systems, 2010**. [[Website](https://ieeexplore.ieee.org/abstract/document/5652983)]


### 3.3 Signed Distance Field (SDF)<a id="3.3-Signed-Distance-Field(SDF)"></a>
- Free-Space Features: Global Localization in 2D Laser SLAM Using Distance Function Maps, **IROS, 2019**. [[Website](https://ieeexplore.ieee.org/document/8967683)]
- Freetures: Localization in Signed Distance Function Maps, **IEEE Robotics and Automation Letters**. [[Website](https://ieeexplore.ieee.org/document/9327493)]


### 3.4 Mesh<a id="3.4-Mesh"></a>

### 3.5 Scene Graph<a id="3.5-Scene-Graph"></a>
- X-View: Graph-Based Semantic Multi-View Localization, **IEEE Robotics and Automation Letters, 2018**. [[Website](https://ieeexplore.ieee.org/abstract/document/8281068)]
- SG-Reg: Generalizable and Efficient Scene Graph Registration, **IEEE Transactions on Robotics, 2025**. [[Website](https://ieeexplore.ieee.org/abstract/document/11024207)]

### 3.6 Neural Radiance Fields (NeRF)<a id="3.6-Neural-Radiance-Fields(NeRF)"></a>

* Loc-NeRF: Monte Carlo Localization using Neural Radiance Fields, *ICRA, 2023*. [[Paper](https://arxiv.org/pdf/2209.09050.pdf)] [[Code](https://github.com/MIT-SPARK/Loc-NeRF)]
* NeRF-Loc: Visual Localization with Conditional Neural Radiance Field, *ICRA, 2023*. [[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10161420&casa_token=xvxGsiWymY0AAAAA:K21qxl7O2Uef-4Gfzqsu_TiA_2GE7EY5Q9iJyawRGZ8sWMKfsxTuANCC7pOcAByT45rS-XIk&tag=1)] [[Code](https://github.com/TencentYoutuResearch/NeRF-Loc)]
* LocNDF: Neural Distance Field Mapping for Robot Localization, *RAL, 2023*. [[Paper](https://ieeexplore.ieee.org/document/10168941/)] [[Code](https://github.com/PRBonn/LocNDF)]
* Leveraging Neural Radiance Fields for Uncertainty-Aware Visual Localization, *ICRA, 2024*. [[Paper](https://arxiv.org/pdf/2310.06984.pdf)] [[Video](https://drive.google.com/file/d/1YUMlngGFvYY_iPNu9wMA1woxw8432qXh/view?usp=sharing)]
* The NeRFect Match: Exploring NeRF Features for Visual Localization, *ECCV, 2024*. [[Paper](https://arxiv.org/pdf/2403.09577.pdf)] [[Website](https://nerfmatch.github.io/)] [[Code](https://github.com/nv-dvl/nerfmatch)]
* Leveraging Neural Radiance Fields for Uncertainty-Aware Visual Localization, *ICRA, 2024*. [[Paper](https://arxiv.org/pdf/2310.06984)]
* NuRF: Nudging the Particle Filter in Radiance Fields for Robot Visual Localization, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2406.00312)]
* Fast Global Localization on Neural Radiance Field, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2406.12202)] [[Code](https://github.com/kmk97/Fast-Loc-NeRF)]
* Matching Query Image Against Selected NeRF Feature for Efficient and Scalable Localization, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2406.11766)]
* Visual Localization in 3D Maps: Comparing Point Cloud, Mesh, and NeRF Representations, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2408.11966)]
* Camera Relocalization in Shadow-Free Neural Radiance Fields, *ICRA, 2024*. [[Paper](https://arxiv.org/pdf/2405.14824)]
* MULAN-WC: Multi-Robot Localization Uncertainty-aware Active NeRF with Wireless Coordination, *IROS, 2024*. [[Paper](https://arxiv.org/pdf/2403.13348)]
* VRS-NeRF: Visual Relocalization with Sparse Neural Radiance Field, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2404.09271)] [[Code](https://github.com/feixue94/vrs-nerf)]
* WSCLoc: Weakly-Supervised Sparse-View Camera Relocalization via Radiance Field, *IROS, 2024*. [[Paper](https://arxiv.org/pdf/2403.15272)]
* CROSSFIRE: Camera Relocalization On Self-Supervised Features from an Implicit Representation, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2403.15272)]
* NeuraLoc: Visual Localization in Neural Implicit Map with Dual Complementary Features, *ICRA, 2025*. [[Paper](https://arxiv.org/pdf/2503.06117)]
* Improving Indoor Localization Accuracy by Using an Efficient Implicit Neural Map Representation, *arXiv, 2025*. [[Paper](https://arxiv.org/pdf/2503.23480)] [[Code](https://arxiv.org/pdf/2503.23480)]

### 3.7 3D Gaussian Splatting (3DGS)<a id="3.7-3D-Gaussian-Splatting(3DGS)"></a>



* HGSLoc: 3DGS-based Heuristic Camera Pose Refinement, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2409.10925)]
* GSLoc: Efficient Camera Pose Refinement via 3D Gaussian Splatting, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2408.11085)] [[Website](https://gsloc.active.vision/)]
* GSplatLoc: Grounding Keypoint Descriptors into 3D Gaussian Splatting for Improved Visual Localization, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2409.16502)] [[Website](https://gsplatloc.github.io/)] [[Code](https://github.com/haksorus/gsplatloc)]
* GSLoc: Visual Localization with 3D Gaussian Splatting, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2410.06165)]
* LoGS: Visual Localization via Gaussian Splatting with Fewer Training Images, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2410.11505)] [[Code](https://github.com/YuzhouCheng66/LoGS-experiment)]
* SplatLoc: 3D Gaussian Splatting-based Visual Localization for Augmented Reality, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2409.16502)] [[Website](https://zju3dv.github.io/splatloc/)] [[Code](https://github.com/zhaihongjia/SplatLoc)]
* Multi-robot autonomous 3D reconstruction using Gaussian splatting with Semantic guidance, *RAL, 2025*. [[Paper](https://arxiv.org/pdf/2412.02249)]
* GSplatLoc : Ultra-Precise Camera Localization via 3D Gaussian Splatting, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2412.20056)] [[Code](https://github.com/AtticusZeller/GsplatLoc)]
* GeomGS: LiDAR-Guided Geometry-Aware Gaussian Splatting for Robot Localization, *arXiv, 2025*. [[Paper](https://arxiv.org/pdf/2501.13417)]
* 3D Gaussian Splatting aided Localization for Large and Complex Indoor-Environments, *arXiv, 2025*. [[Paper](https://arxiv.org/pdf/2502.13803)]
* GS-EVT: Cross-Modal Event Camera Tracking based on Gaussian Splatting, *ICRA, 2025*. [[Paper](https://arxiv.org/pdf/2409.19228v1)] [[Code](https://github.com/ChillTerry/GS-EVT)]
* GSFeatLoc: Visual Localization Using Feature Correspondence on 3D Gaussian Splatting, *arXiv, 2025*. [[Paper](https://arxiv.org/pdf/2504.20379)]
* STDLoc: From Sparse to Dense: Camera Relocalization with Scene-Specific Detector from Feature Gaussian Splatting, *CVPR, 2025*. [[Paper](https://arxiv.org/pdf/2503.19358)][[Website](https://zju3dv.github.io/STDLoc/)] [[Code](https://github.com/zju3dv/STDLoc)]
* SGLoc: Semantic Localization System for Camera Pose Estimation from 3D Gaussian Splatting Representation, *IROS, 2025*. [[Paper](https://arxiv.org/pdf/2507.12027)]
* 3DGS-Loc: 3D Gaussian Splatting for Map Representation and Visual Localization, *Journal of Autonomous Vehicles and Systems, 2025*. [[Paper](https://asmedigitalcollection.asme.org/autonomousvehicles/article-abstract/doi/10.1115/1.4069346/1220059/3DGS-Loc-3D-Gaussian-Splatting-for-Map?redirectedFrom=fulltext)]
* GSVisLoc: Generalizable Visual Localization for Gaussian Splatting Scene Representations, *arXiv, 2025*. [[Paper](https://arxiv.org/pdf/2508.18242)]
* Camera Pose Refinement via 3D Gaussian Splatting, *arXiv, 2025*. [[Paper](https://arxiv.org/pdf/2508.17876)]
* 3DGS-ReLoc: 3D Gaussian Splatting for Map Representation and Visual ReLocalization, *ICCV, 2023*. [[Paper](https://openaccess.thecvf.com/content/ICCV2023/papers/Moreau_CROSSFIRE_Camera_Relocalization_On_Self-Supervised_Features_from_an_Implicit_Representation_ICCV_2023_paper.pdf)]
* GauLoc: 3D Gaussian Splatting-based Camera Relocalization, *Computer Graphics Forum, 2024*. [[Paper](https://onlinelibrary.wiley.com/doi/abs/10.1111/cgf.15256)] [[Code](https://github.com/xinzhe11/GauLoc)]
* GS-Loc: A Vision Foundation Model-Driven 3D Gaussian Splatting Framework for Robust Visual Relocalization, *RAL, 2025*. [[Paper](https://ieeexplore.ieee.org/document/11260953)]

  
### 3.8 Foundation Model<a id="3.8-Foundation-Model<"></a>
- SLAM3R:Real-Time Dense Scene Reconstruction from Monocular RGB Videos, **CVPR, 2025**. [[Paper](https://openaccess.thecvf.com/content/CVPR2025/papers/Liu_SLAM3R_Real-Time_Dense_Scene_Reconstruction_from_Monocular_RGB_Videos_CVPR_2025_paper.pdf)]
- MASt3R-SLAM: Real-Time Dense SLAM with 3D Reconstruction Priors, **CVPR, 2025**. [[Paper](https://openaccess.thecvf.com/content/CVPR2025/papers/Murai_MASt3R-SLAM_Real-Time_Dense_SLAM_with_3D_Reconstruction_Priors_CVPR_2025_paper.pdf)]
- ViSTA-SLAM: Visual SLAM with Symmetric Two-view Association, **3DV, 2026**. [[Paper](https://arxiv.org/abs/2509.01584)]
- VGGT-SLAM: Dense RGB SLAM Optimized on the SL(4) Manifold, *arXiv*. [[Website](https://arxiv.org/abs/2505.12549)]

## 4.Navigation<a id="navigation"></a>

### 4.1 Geometric Representations<a id="4.1-Geometric-Representations"></a>

* Navigation on point-cloud-a riemannian metric approach, **ICRA, 2014**. [[Paper](https://ieeexplore.ieee.org/document/6907453)]
* Localization and navigation of a mobile robot using natural point landmarks extracted from sonar data, **Robotics and Autonomous Systems, 2000**. [[Paper](https://www.sciencedirect.com/science/article/abs/pii/S0921889099000858)]
* OctoMap: An Efficient Probabilistic 3D Mapping Framework Based on Octrees, **Autonomous Robots, 2013**. [[Paper](https://link.springer.com/article/10.1007/s10514-012-9321-0)] [[Code](https://github.com/OctoMap/octomap)]
* Fast-Planner: Robust and Efficient Quadrotor Trajectory Generation for Fast Autonomous Flight, **IEEE Robot. Autom. Lett., 2019**. [[Paper](https://ieeexplore.ieee.org/document/8758904)] [[Code](https://github.com/HKUST-Aerial-Robotics/Fast-Planner)]
* Voxblox: Incremental 3d euclidean signed distance fields for on-board mav planning, **IROS, 2017**. [[Paper](https://ieeexplore.ieee.org/abstract/document/8202315)] [[Code](https://github.com/ethz-asl/voxblox)]
* FIESTA: Fast Incremental Euclidean Distance Fields for Online Motion Planning of Aerial Robots, **IROS, 2019**. [[Paper](https://ieeexplore.ieee.org/abstract/document/8968199)] [[Code](https://github.com/HKUST-Aerial-Robotics/FIESTA)]

### 4.2 NeRF-based Representations<a id="4.2-NeRF-based-Representations"></a>
* Vision-only robot navigation in a neural radiance world (NeRF-Navigation), **IEEE Robot. Autom. Lett., 2022**. [[Paper](https://ieeexplore.ieee.org/document/9712211)] [[Website](https://m-adamkiewicz.github.io/nerf_navigation/)]
* NFOMP: Neural field for optimal motion planner of differential drive robots with nonholonomic constraints, **IEEE Robot. Autom. Lett., 2022**. [[Paper](https://ieeexplore.ieee.org/document/9851532)]
* CATNIPS: Collision Avoidance Through Neural Implicit Probabilistic Scenes, **IEEE Trans. Robot., 2024**. [[Paper](https://ieeexplore.ieee.org/document/10494911)]
* RNR-Map: Renderable Neural Radiance Map for Visual Navigation, **CVPR, 2023**. [[Paper](https://openaccess.thecvf.com/content/CVPR2023/html/Kwon_Renderable_Neural_Radiance_Map_for_Visual_Navigation_CVPR_2023_paper.html)] [[Website](https://obin-kwon.github.io/rnr-map/)]
* Enhancing Exploratory Capability of Visual Navigation Using Uncertainty of Implicit Scene Representation, **IROS, 2024**. [[Paper](https://ieeexplore.ieee.org/document/10801778)]

### 4.3 3DGS-based Representations<a id="4.3-3DGS-based-Representations"></a>

#### Path Planning
* GaussNav: Gaussian Splatting for Visual Navigation, **IEEE Trans. Pattern Anal. Mach. Intell., 2025**. [[Paper](https://ieeexplore.ieee.org/document/10870413)] [[Code](https://github.com/XiaohanLei/GaussNav)]
* Splat-Nav: Safe Real-Time Robot Navigation in Gaussian Splatting Maps, **IEEE Trans. Robot., 2025**. [[Paper](https://ieeexplore.ieee.org/document/10930696)]
* BEINGS: Bayesian Embodied Image-goal Navigation with Gaussian Splatting, **arXiv, 2024**. [[Paper](https://arxiv.org/abs/2409.10216)]

#### Exploration
* GS-Planner: A Gaussian-Splatting-based Planning Framework for Active High-Fidelity Reconstruction, **IROS, 2024**. [[Paper](https://arxiv.org/abs/2405.10142)]
* Beyond Uncertainty: Risk-Aware Active View Acquisition for Safe Robot Navigation and 3D Scene Understanding with FisherRF, **arXiv, 2024**. [[Paper](https://arxiv.org/abs/2403.11396)]

### 4.4 Foundation Model<a id="4.4-Foundation-Model"></a>
* NLMap: Open-vocabulary queryable scene representations for real world planning, **ICRA, 2023**. [[Paper](https://ieeexplore.ieee.org/document/10160679)] [[Website](https://nlmap-saycan.github.io/)] [[Code](https://github.com/apple/ml-nlmap)]
* LM-Nav: Robotic navigation with large pre-trained models of language, vision, and action, **CoRL, 2023**. [[Paper](https://proceedings.mlr.press/v205/shah23b.html)] [[Website](https://sites.google.com/view/lmnav)] [[Code](https://github.com/blazejosinski/lm_nav)]
* VLN-BERT: Improving vision-and-language navigation with image-text pairs from the web, **ECCV, 2020**. [[Paper](https://link.springer.com/chapter/10.1007/978-3-030-58539-6_16)] [[Code](https://github.com/arjunmajum/VLN-BERT)]
* SayCan: Do As I Can, Not As I Say: Grounding Language in Robotic Affordances, **CoRL, 2022**. [[Paper](https://proceedings.mlr.press/v205/ahn23a.html)] [[Website](https://say-can.github.io/)]
* VLP: Vision language planning for autonomous driving, **CVPR, 2024**. [[Paper](https://openaccess.thecvf.com/content/CVPR2024/html/Pan_VLP_Vision_Language_Planning_for_Autonomous_Driving_CVPR_2024_paper.html)] [[Code](https://github.com/CH3COOK/VLP)]
* Reasoned Explorer: Reasoning about the unseen for efficient outdoor object navigation, **arXiv, 2023**. [[Paper](https://arxiv.org/abs/2309.10103)] [[Website](https://qiexie.com/reasoned_explorer/)]
* VoxPoser: Composable 3D Value Maps for Robotic Manipulation with Language Models, **CoRL, 2023**. [[Paper](https://arxiv.org/abs/2307.05973)] [[Website](https://voxposer.github.io/)]
* SayTap: Language to Quadrupedal Locomotion, **arXiv, 2023**. [[Paper](https://arxiv.org/abs/2306.07580)] [[Website](https://saytap.github.io/)]

## 5.Manipulation<a id="manipulation"></a>
### 5.1 Point Cloud<a id="5.1-Point-Cloud"></a>
* PointNetGPD: Detecting Grasp Configurations from Point Sets, **ICRA, 2019**. [[Paper](https://ieeexplore.ieee.org/document/8794435)][[Code](https://github.com/lianghongzhuo/PointNetGPD)]
* Contact-GraspNet: Efficient 6-DoF Grasp Generation in Cluttered Scenes, **ICRA, 2021**. [[Paper](https://ieeexplore.ieee.org/document/9561877)][[Code](https://github.com/NVlabs/contact_graspnet)][[Website](https://research.nvidia.com/publication/2021-03_contact-graspnet-efficient-6-dof-grasp-generation-cluttered-scenes)]
### 5.2 Voxel Grid<a id="5.2-Voxel-Grid"></a>
* Shape Completion Enabled Robotic Grasping, **IROS, 2017**. [[Paper](https://www.cs.columbia.edu/~allen/PAPERS/varley_iros_2017.pdf)][[Code](http://shapecompletiongrasping.cs.columbia.edu)][[Website](https://rhys-newbury.github.io/bibliography/varley2017shape.html)]
* VoxelNet: End-to-End Learning for Point Cloud Based 3D Object Detection, **CVPR, 2018**. [[Paper](https://openaccess.thecvf.com/content_cvpr_2018/papers/Zhou_VoxelNet_End-to-End_Learning_CVPR_2018_paper.pdf)][[Code](https://github.com/ModelBunker/VoxelNet-PyTorch)]
* Volumetric Grasping Network: Real-time 6 DOF Grasp Detection in Clutter, **CoRL, 2020**. [[Paper](https://proceedings.mlr.press/v155/breyer21a.html)][[Code](https://github.com/ethz-asl/vgn)]
* Fast Task Planning with Neuro-Symbolic Relaxation, *arXiv*. [[Paper](https://arxiv.org/abs/2507.15975)][[Website](https://sairlab.org/flax/)]
### 5.3 Signed Distance Field (SDF)<a id="5.3-Signed-Distance-Field(SDF)"></a>
### 5.4 Mesh<a id="5.4-Mesh"></a>
### 5.5 Scene Graph<a id="5.5-Scene-Graph"></a>
* Neural Descriptor Fields:SE(3)-Equivariant Object Representations for Manipulation, **ICRA, 2022**. [[Paper](https://arxiv.org/abs/2112.05124)] [[Code](https://github.com/anthonysimeonov/ndf_robot)] [[Website](https://yilundu.github.io/ndf/)]
* Sequential Manipulation Planning on Scene Graph, **IROS, 2022**. [[Website](https://ieeexplore.ieee.org/document/9981735)]
* RoboEXP: Action-Conditioned Scene Graph via Interactive Exploration for Robotic Manipulation, **CoRL, 2024**. [[Paper](https://openreview.net/forum?id=UHxPZgK33I)][[Code](https://github.com/Jianghanxiao/RoboEXP)][[Website](https://jianghanxiao.github.io/roboexp-web/)]
* Dynamic Open-Vocabulary 3D Scene Graphs for Long-Term Language-Guided Mobile Manipulation, **IRAL, 2025**. [[Paper](https://ouci.dntb.gov.ua/en/works/4grdOgwW/)][[Code](https://github.com/BJHYZJ/DovSG)][[Website](https://bjhyzj.github.io/dovsg-web/)]
### 5.6 Neural Radiance Fields (NeRF)<a id="5.6-Neural-Radiance-Fields(NeRF)"></a>
* Dex-NeRF: Using a Neural Radiance Field to Grasp Transparent Objects, **CoRL, 2021**. [[Paper](https://proceedings.mlr.press/v164/ichnowski22a/ichnowski22a.pdf)][[Website](https://sites.google.com/view/dex-nerf)]
* Evo-NeRF: Evolving NeRF for Sequential Robot Grasping of Transparent Objects, **CoRL, 2022**. [[Paper](https://openreview.net/forum?id=Bxr45keYrf)][[Website](https://sites.google.com/view/evo-nerf)]
* GraspNeRF: Multiview-based 6-DoF Grasp Detection for Transparent and Specular Objects Using Generalizable NeRF, **ICRA, 2023**. [[Paper](https://arxiv.org/abs/2210.06575)][[Code](https://github.com/PKU-EPIC/GraspNeRF)][[Website](https://pku-epic.github.io/GraspNeRF/)]
* Radiance Fields for Robotic Teleoperation, **IROS, 2024**. [[Paper](https://ieeexplore.ieee.org/abstract/document/10801345)][[Code](https://github.com/leggedrobotics/radiance_field_ros)]
### 5.7 3D Gaussian Splatting (3DGS)<a id="5.7-3D-Gaussian-Splatting(3DGS)"></a>
* Grasping Field: Learning Implicit Representations for Human Grasps, **3DV, 2020**. [[Paper](https://arxiv.org/pdf/2008.04451.pdf)] [[Code](https://github.com/korrawe/grasping_field)] [[Video](https://youtu.be/J8x5i1FCgTQ)]
* GIGA: Synergies Between Affordance and Geometry: 6-DoF Grasp Detection via Implicit Representations, **RSS, 2021**. [[Paper](https://arxiv.org/abs/2104.01542)] [[Code](https://github.com/UT-Austin-RPL/GIGA)] [[Website](https://sites.google.com/view/rpl-giga2021)]
* Neural Motion Fields: Encoding Grasp Trajectories as Implicit Value Functions, **RSS, 2022**. [[Paper](https://arxiv.org/pdf/2206.14854.pdf)]  [[Video](https://youtu.be/B-pEhT1pi-Q)]
* ObjectFolder: A Dataset of Objects with Implicit Visual, Auditory, and Tactile Representations, **CVPR, 2022**. [[Paper](https://arxiv.org/pdf/2109.07991.pdf)] [[Code](https://github.com/rhgao/ObjectFolder)] [[Website](https://ai.stanford.edu/~rhgao/objectfolder/)]
* Relational-NDF:SE(3)-Equivariant Relational Rearrangement with Neural Descriptor Fields, **CoRL, 2022**. [[Paper](https://arxiv.org/pdf/2211.09786.pdf)] [[Code](https://github.com/anthonysimeonov/relational_ndf)] [[Website](https://anthonysimeonov.github.io/r-ndf/)]
* Local Neural Descriptor Fields: Locally Conditioned Object Representations for Manipulation, **ICRA, 2023**. [[Paper](https://arxiv.org/pdf/2302.03573.pdf)] [[Code](https://github.com/elchun/lndf_robot)] [[Website](https://elchun.github.io/lndf/)]
* Equivariant Descriptor Fields: SE(3)-Equivariant Energy-Based Models for End-to-End Visual Robotic Manipulation Learning, **ICLR, 2023**. [[Paper](https://openreview.net/forum?id=dnjZSPGmY5O)] [[Code](https://github.com/tomato1mule/edf)]
* Point'n Move: Interactive scene object manipulation on Gaussian splatting radiance fields, **IET, 2024**.  [[Paper](https://ietresearch.onlinelibrary.wiley.com/doi/10.1049/ipr2.13190?af=R)][[Code](https://github.com/jhuangBU/pnm)]
* Reinforcement Learning with Generalizable Gaussian Splatting, **IROS, 2024**. [[Paper](https://arxiv.org/abs/2404.07950)]
* MANUS: Markerless Grasp Capture using Articulated 3D Gaussians, **CVPR, 2024**. [[Paper](https://openaccess.thecvf.com/content/CVPR2024/papers/Pokhariya_MANUS_Markerless_Grasp_Capture_using_Articulated_3D_Gaussians_CVPR_2024_paper.pdf)][[Code](https://github.com/brown-ivl/manus)][[Website](https://ivl.cs.brown.edu/research/manus.html)]
* ManiGaussian: Dynamic Gaussian Splatting for Multi-task Robotic Manipulation, **ECCV, 2024**. [[Paper](https://arxiv.org/abs/2403.08321)][[Code](https://github.com/GuanxingLu/ManiGaussian)][[Website](https://guanxinglu.github.io/ManiGaussian/)]
* GaussianGrasper: 3D Language Gaussian Splatting for Open-Vocabulary Robotic Grasping, **RAL, 2024**. [[Paper](https://ieeexplore.ieee.org/document/10607869)][[Code](https://github.com/MrSecant/GaussianGrasper)][[Website](https://mrsecant.github.io/GaussianGrasper/)]
* 3D-Aware Manipulation with Object-Centric Gaussian Splatting, **ICRA, 2024**. [[Paper](https://object-aware-gaussian.github.io/assets/pdf/corl.pdf)] [[Website](https://object-aware-gaussian.github.io/)]
* Radiance Fields for Robotic Teleoperation, **IROS, 2024**. [[Paper](https://arxiv.org/pdf/2407.20194)][[Website](https://rffr.leggedrobotics.com/works/teleoperation/)][[Video](https://www.youtube.com/watch?v=NR-X1FETJj8&feature=youtu.be)]
* GraspSplats: Efficient Manipulation with 3D Feature Splatting, **CoRL, 2024**. [[Paper](https://openreview.net/forum?id=pPhTsonbXq)][[Code](https://github.com/jimazeyu/GraspSplats)][[Website](https://graspsplats.github.io/)]
* Object-Aware Gaussian Splatting for Robotic Manipulation, **ICRA, 2024**. [[Paper](https://openreview.net/forum?id=gdRI43hDgo)][[Website](https://object-aware-gaussian.github.io/)]
* Dynamic 3D Gaussian Tracking for Graph-Based Neural Dynamics Modeling, **CoRL, 2024**. [[Paper](https://arxiv.org/abs/2410.18912)][[Code](https://github.com/robo-alex/gs-dynamics)][[Website](https://gs-dynamics.github.io/)]
* HGS-Planner: Hierarchical Planning Framework for Active Scene Reconstruction Using 3D Gaussian Splatting, **ICRA, 2025**. [[Paper](https://arxiv.org/abs/2409.17624)][[Website](https://zijunfdu.github.io/HGS-Planner/)]
* SplatSim: Zero-Shot Sim2Real Transfer of RGB Manipulation Policies Using Gaussian Splatting, **ICRA, 2025**. [[Paper](https://ieeexplore.ieee.org/document/11128339)][[Code](https://github.com/qureshinomaan/SplatSim)][[Website](https://splatsim.github.io/)]
* Gaussian Splatting to Real World Flight Navigation Transfer with Liquid Networks, *arXiv*. [[Paper](https://arxiv.org/pdf/2406.15149)][[Website](https://sites.google.com/view/gs2real-flight/home)]
* MSGField: A Unified Scene Representation Integrating Motion, Semantics, and Geometry for Robotic Manipulation, *arXiv*. [[Paper](https://arxiv.org/abs/2410.15730)][[Code](https://github.com/ShengYu724/MSGField)][[Website](https://shengyu724.github.io/MSGField.github.io/)]
* Physically Embodied Gaussian Splatting: A Realtime Correctable World Model for Robotics, *arXiv*, [[Paper](https://arxiv.org/abs/2406.10788)][[Code](https://github.com/bdaiinstitute/embodied_gaussians)][[Website](https://embodied-gaussians.github.io/)]

### 5.8 Foundation Model<a id="5.8-Foundation-Model"></a>
* Ditto: Building Digital Twins of Articulated Objects from Interaction, **CVPR, 2022**. [[Paper](https://arxiv.org/abs/2202.08227)] [[Code](https://github.com/UT-Austin-RPL/Ditto)] [[Website](https://ut-austin-rpl.github.io/Ditto/)]
* LERF: Language Embedded Radiance Fields, **ICCV, 2023**. [[Paper](https://openaccess.thecvf.com/content/ICCV2023/papers/Kerr_LERF_Language_Embedded_Radiance_Fields_ICCV_2023_paper.pdf)][[Code](https://github.com/kerrj/lerf)][[Website](https://www.lerf.io/)]
* Distilled Feature Fields Enable Few-Shot Language-Guided Manipulation, **CoRL, 2023**. [[Paper](https://openreview.net/forum?id=Rb0nGIt_kh5)][[Code](https://github.com/f3rm/f3rm)][[Website](https://f3rm.csail.mit.edu)]
* GNFactor: Multi-Task Real Robot Learning with Generalizable Neural Feature Fields, **CORL, 2023**. [[Paper](https://openreview.net/forum?id=b1tl3aOt2R2)][[Code](https://github.com/YanjieZe/GNFactor)][[Website](https://yanjieze.com/GNFactor/)]
* Code as Policies: Language Model Programs for Embodied Control, **ICRA, 2023**. [[Paper](https://ieeexplore.ieee.org/document/10160591)][[Code](https://github.com/google-research/google-research/tree/master/code_as_policies)][[Website](https://code-as-policies.github.io/)]
* Open-vocabulary Queryable Scene Representations for Real World Planning, **ICRA, 2023**. [[Paper](https://www.academia.edu/114475447/Open_vocabulary_Queryable_Scene_Representations_for_Real_World_Planning)][[Code](https://github.com/ericrosenbrown/nlmap_spot)][[Website](https://nlmap-saycan.github.io/)]
* CATNIPS: Collision Avoidance Through Neural Implicit Probabilistic Scenes, **TRO, 2024**. [[Paper](https://msl.stanford.edu/papers/chen_catnips_2024.pdf)][[Code](https://github.com/chengine/catnips)][[Website](https://chengine.github.io/catnips/)]
* Enhancing Exploratory Capability of Visual Navigation Using Uncertainty of Implicit Scene Representation, **IROS, 2024**. [[Paper](https://ieeexplore.ieee.org/document/10801778)][[Code](https://github.com/IRMVLab/NUE-NeRF-nav)]
* DreamHOI: Subject-Driven Generation of 3D Human-Object Interactions with Diffusion Priors, **ICCVW, 2025**. [[Paper](https://openaccess.thecvf.com/content/ICCV2025W/HiGen/papers/Zhu_DreamHOI_Subject-Driven_Generation_of_3D_Human-Object_Interactions_with_Diffusion_Priors_ICCVW_2025_paper.pdf)][[Code](https://github.com/hanwenzhu/dreamhoi)][[Website](https://dreamhoi.github.io/)]
* EnerVerse: Envisioning Embodied Future Space for Robotics Manipulation，*arXiv*. [[Paper](https://arxiv.org/abs/2501.01895)][[Website](https://sites.google.com/view/enerverse)]
* Do As I Can, Not As I Say: Grounding Language in Robotic Affordances, *arXiv*. [[Paper](https://proceedings.mlr.press/v205/ichter23a.html)][[Code](https://github.com/google-research/google-research/tree/master/saycan)][[Website](https://say-can.github.io/)]

## 6.Simulation<a id="simulation"></a>
* Control4D: Efficient 4D Portrait Editing with Text, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2305.20082.pdf)] [[Website](https://control4darxiv.github.io/)]
* Comp4D: LLM-Guided Compositional 4D Scene Generation, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.16993.pdf)] [[Website](https://vita-group.github.io/Comp4D/)] [[Code](https://github.com/VITA-Group/Comp4D)]
* GALA3D: Towards Text-to-3D Complex Scene Generation via Layout-guided Generative Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2402.07207.pdf)] [[Website](https://gala3d.github.io/)] [[Code](https://github.com/VDIGPKU/GALA3D)]
* Controllable Text-to-3D Generation via Surface-Aligned Gaussian Splatting, *arXiv*. [[Paper](https://lizhiqi49.github.io/MVControl/assets/paper.pdf)] [[Website](https://lizhiqi49.github.io/MVControl/)] [[Code](https://github.com/WU-CVGL/MVControl-threestudio)]
* Hyper-3DG:Text-to-3D Gaussian Generation via Hypergraph, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.09236.pdf)] [[Website](https://arxiv.org/abs/2403.09236)] [[Code](https://github.com/yjhboy/Hyper3DG)]
* DreamScene: 3D Gaussian-based Text-to-3D Scene Generation via Formation Pattern Sampling, *arXiv*. [[Paper](https://arxiv.org/pdf/2404.03575.pdf)] [[Website](https://dreamscene-project.github.io/)] [[Code](https://github.com/DreamScene-Project/DreamScene)]
* BrightDreamer: Generic 3D Gaussian Generative Framework for Fast Text-to-3D Synthesis, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.11273)] [[Website](https://vlislab22.github.io/BrightDreamer/)] [[Code](https://github.com/lutao2021/BrightDreamer)]
* GVGEN: Text-to-3D Generation with Volumetric Representation, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.12957)] [[Website](https://gvgen.github.io/)] [[Code](https://github.com/GVGEN/GVGEN)]
* DreamPolisher: Towards High-Quality Text-to-3D Generation via Geometric Diffusion, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.17237)] [[Website](https://yuanze-lin.me/DreamPolisher_page/)] [[Code](https://github.com/yuanze-lin/DreamPolisher)]
* DreamScene360: Unconstrained Text-to-3D Scene Generation with Panoramic Gaussian Splatting, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2404.06903)] [[Website](https://dreamscene360.github.io/)]
* RealmDreamer: Text-Driven 3D Scene Generation with Inpainting and Depth Diffusion, *arXiv*. [[Paper](https://arxiv.org/pdf/2404.07199)] [[Website](https://realmdreamer.github.io/)]
* Text-to-3D using Gaussian Splatting, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2309.16585.pdf)] [[Website](https://gsgen3d.github.io/)] [[Code](https://github.com/gsgen3d/gsgen)]
* DreamGaussian: Generative Gaussian Splatting for Efficient 3D Content Creation, *arXiv*. [[Paper](https://arxiv.org/pdf/2309.16653.pdf)] [[Website](https://dreamgaussian.github.io/)] [[Code](https://github.com/dreamgaussian/dreamgaussian)]
* GaussianDreamer: Fast Generation from Text to 3D Gaussian Splatting with Point Cloud Priors, *arXiv*. [[Paper](https://arxiv.org/pdf/2310.08529.pdf)] [[Website](https://taoranyi.com/gaussiandreamer/)] [[Code](https://github.com/hustvl/GaussianDreamer)]
* GaussianDiffusion: 3D Gaussian Splatting for Denoising Diffusion Probabilistic Models with Structured Noise, *arXiv*. [[Paper](https://arxiv.org/pdf/2311.11221.pdf)] [[Website](https://arxiv.org/abs/2311.11221)]
* LucidDreamer: Towards High-Fidelity Text-to-3D Generation via Interval Score Matching, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2311.11284.pdf)] [[Website](https://arxiv.org/abs/2311.11284)] [[Code](https://github.com/EnVision-Research/LucidDreamer)]
* CG3D: Compositional Generation for Text-to-3D, *arXiv*. [[Paper](https://arxiv.org/pdf/2311.17907.pdf)] [[Website](https://asvilesov.github.io/CG3D/)]
* Align Your Gaussians: Text-to-4D with Dynamic 3D Gaussians and Composed Diffusion Models, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2304.08818.pdf)] [[Website](https://research.nvidia.com/labs/toronto-ai/AlignYourGaussians/)]
* Text2Immersion: Generative Immersive Scene with 3D Gaussian, *arXiv*. [[Paper](https://arxiv.org/pdf/2312.09242.pdf)] [[Website](https://ken-ouyang.github.io/text2immersion/index.html)]
* GSEdit: Efficient Text-Guided Editing of 3D Objects via Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.05154.pdf)]
* GaussCtrl: Multi-View Consistent Text-Driven 3D Gaussian Splatting Editing, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.08733.pdf)]
* View-Consistent 3D Editing with Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.11868.pdf)]
* Gaussian Frosting: Editable Complex Radiance Fields with Real-Time Rendering, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.14554)] [[Website](https://anttwo.github.io/frosting/)] [[Code](https://github.com/Anttwo/Frosting)]
* ICE-G: Image Conditional Editing of 3D Gaussian Splats, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2406.08488)] [[Website](https://ice-gaussian.github.io/)]
* GaussianEditor: Swift and Controllable 3D Editing with Gaussian Splatting, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2311.14521.pdf)] [[Website](https://buaacyw.github.io/gaussian-editor/)] [[Code](https://github.com/buaacyw/GaussianEditor)]
* GaussianEditor: Editing 3D Gaussians Delicately with Text Instructions, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2311.16037.pdf)] [[Website](https://gaussianeditor.github.io/)]
* Gaussian Grouping: Segment and Edit Anything in 3D Scenes, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2312.00732.pdf)] [[Code](https://github.com/lkeab/gaussian-grouping)]
* StyleGaussian: Instant 3D Style Transfer with Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.07807.pdf)] [[Website](https://kunhao-liu.github.io/StyleGaussian/)] [[Code](https://github.com/Kunhao-Liu/StyleGaussian)]
* Gaussian Splatting in Style, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.08498)]
* StylizedGS: Controllable Stylization for 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2404.05220)]
* 3DEgo: 3D Editing on the Go!, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2407.10102.pdf)]
* GScream: Learning 3D Geometry and Feature Consistent Gaussian Splatting for Object Removal, **ECCV, 2024**. [[Paper](https://arxiv.org/abs/2404.13679)]
* Gaussian Splatting with Localized Points Management, *arXiv, 2024*. [[Paper](https://arxiv.org/abs/2406.04251)]
* Localized Gaussian Splatting Editing with Contextual Awareness, *arXiv, 2024*. [[Paper](https://arxiv.org/abs/2408.00083)]
* 3D Gaussian Editing with A Single Image, *arXiv*. [[Paper](https://arxiv.org/abs/2408.07540)]
* G-Style: Stylized Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2408.15695)]
* AGG: Amortized Generative 3D Gaussians for Single Image to 3D, *arXiv*. [[Paper](https://arxiv.org/pdf/2401.04099.pdf)] [[Website](https://ir1d.github.io/AGG/)]
* Repaint123: Fast and High-quality One Image to 3D Generation with Progressive Controllable 2D Repainting, *arXiv*. [[Paper](https://arxiv.org/pdf/2312.13271.pdf)] [[Website](https://pku-yuangroup.github.io/repaint123/)] [[Code](https://github.com/PKU-YuanGroup/repaint123)]
* GaussianPU: A Hybrid 2D-3D Upsampling Framework for Enhancing Color Point Clouds via 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2409.01581)]
* WaSt-3D: Wasserstein-2 Distance for Scene-to-Scene Stylization on 3D Gaussians, *arXiv*. [[Paper](https://arxiv.org/abs/2409.17917)]
* Generative Object Insertion in Gaussian Splatting with a Multi-View Diffusion Model, *arXiv*. [[Paper](https://arxiv.org/abs/2409.16938)]
* TIP-Editor: An Accurate 3D Editor Following Both Text-Prompts And Image-Prompts, *arXiv*. [[Paper](https://arxiv.org/pdf/2401.14828.pdf)] [[Website](https://zjy526223908.github.io/TIP-Editor/)]
* DreamScene4D: Dynamic Multi-Object Scene Generation from Monocular Videos, *arXiv*. [[Paper](https://arxiv.org/pdf/2405.02280)] [[Website](https://dreamscene4d.github.io/)] [[Code](https://github.com/dreamscene4d/dreamscene4d)]
* Connecting Consistency Distillation to Score Distillation for Text-to-3D Generation, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2407.13584)] [[Code](https://github.com/LMozart/ECCV2024-GCS-BEG)]
* DreamMapping: High-Fidelity Text-to-3D Generation via Variational Distribution Mapping, *arXiv*. [[Paper](https://arxiv.org/abs/2409.05099)]
* DreamMesh: Jointly Manipulating and Texturing Triangle Meshes for Text-to-3D Generation, *arXiv*. [[Paper](https://arxiv.org/abs/2409.07454)]
* Hi3D: Pursuing High-Resolution Image-to-3D Generation with Video Diffusion Models, *arXiv*. [[Paper](https://arxiv.org/abs/2409.07452)]
* SceneTeller: Language-to-3D Scene Generation, **ECCV 2024**. [[Paper](https://arxiv.org/pdf/2407.20727.pdf)]
* HoloDreamer: Holistic 3D Panoramic World Generation from Text Descriptions, *arXiv*. [[Paper](https://arxiv.org/pdf/2407.15187.pdf)]
* SV4D: Dynamic 3D Content Generation with Multi-Frame and Multi-View Consistency, *arXiv*. [[Paper](https://arxiv.org/pdf/2407.17470.pdf)]
* ART3D: 3D Gaussian Splatting for Text-Guided Artistic Scenes Generation, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2405.10508.pdf)]
* 3D-Adapter: Geometry-Consistent Multi-View Diffusion for High-Quality 3D Generation, *arXiv*. [[Paper](https://arxiv.org/pdf/2410.18974.pdf)]
* ProEdit: Simple Progression is All You Need for High-Quality 3D Scene Editing, *arXiv*. [[Paper](https://arxiv.org/pdf/2411.05006)]
* Baking Gaussian Splatting into Diffusion Denoiser for Fast and Scalable Single-stage Image-to-3D Generation, *arXiv*. [[Paper](https://arxiv.org/abs/2411.14384)]
* Generating 3D-Consistent Videos from Unposed Internet Photos, *arXiv*. [[Paper](https://arxiv.org/abs/2411.13549)]
* Direct and Explicit 3D Generation from a Single Image, *arXiv*. [[Paper](https://arxiv.org/abs/2411.10947)]
* PhyCAGE: Physically Plausible Compositional 3D Asset Generation from a Single Image, *arXiv*. [[Paper](https://arxiv.org/abs/2411.18548)]
* Neural Surface Priors for Editable Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2411.18311)]
* SplatFlow: Multi-View Rectified Flow Model for 3D Gaussian Splatting Synthesis, *arXiv*. [[Paper](https://arxiv.org/abs/2411.16443)]
* Distractor-free Generalizable 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2411.17605)]
* Text-to-3D Gaussian Splatting with Physics-Grounded Motion Generation, *arXiv*. [[Paper](https://arxiv.org/abs/2412.05560)]
* Diffusion-Based Attention Warping for Consistent 3D Scene Editing, *arXiv*. [[Paper](https://arxiv.org/abs/2412.07984)]
* ProGDF: Progressive Gaussian Differential Field for Controllable and Flexible 3D Editing, *arXiv*. [[Paper](https://arxiv.org/abs/2412.08152)]
* EditSplat: Multi-View Fusion and Attention-Guided Optimization for View-Consistent 3D Scene Editing with 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2412.11520)]
* 3DSceneEditor: Controllable 3D Scene Editing with Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2412.01583)]
* Instant3dit: Multiview Inpainting for Fast Editing of 3D Objects, *arXiv*. [[Paper](https://arxiv.org/abs/2412.00518)]
* ZDySS -- Zero-Shot Dynamic Scene Stylization using Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2501.03875)]
* Drag Your Gaussian: Effective Drag-Based Editing with Score Distillation for 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2501.18672)]

---
## Citation

If you find this repository useful, please consider citing this list:

```
@article{deng2025best,
  title={What Is The Best 3D Scene Representation for Robotics? From Geometric to Foundation Models},
  author={Deng, Tianchen and Pan, Yue and Yuan, Shenghai and Li, Dong and Wang, Chen and Li, Mingrui and Chen, Long and Xie, Lihua and Wang, Danwei and Wang, Jingchuan and others},
  journal={arXiv preprint arXiv:2512.03422},
  year={2025}
}
```
