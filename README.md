# Awesome Correspondence Pruning

A curated collection of papers and code on two-view correspondence pruning and mismatch removal, with a focus on coordinate-based methods.

The main collection focuses on conference papers, with selected journal papers and preprints included for their relevance. Journal extensions are linked alongside their conference versions.

## Scope

The core task is to filter or weight tentative two-view correspondences, typically represented as an `N × 4` array of coordinate pairs `(x, y, x′, y′)`, for geometric estimation. Some included methods also use visual information. Related learning techniques, applications, surveys, and benchmarks are listed separately.


## Contents

- [Awesome Correspondence Pruning](#awesome-correspondence-pruning)
  - [Scope](#scope)
  - [Contents](#contents)
  - [Learning-based Methods](#learning-based-methods)
  - [Traditional Motion Coherence Methods](#traditional-motion-coherence-methods)
  - [Related Methods and Applications](#related-methods-and-applications)
  - [Surveys and Benchmarks](#surveys-and-benchmarks)

## Learning-based Methods

- [PointCN] Learning to Find Good Correspondences — [CVPR 2018](https://arxiv.org/pdf/1711.05971) · [Code](https://github.com/vcg-uvic/learned-correspondence-release)
- Deep fundamental matrix estimation — [ECCV 2018](https://openaccess.thecvf.com/content_ECCV_2018/papers/Rene_Ranftl_Deep_Fundamental_Matrix_ECCV_2018_paper.pdf) · [Code](https://github.com/isl-org/DFE)
- NM-Net: Mining Reliable Neighbors for Robust Feature Correspondences — [CVPR 2019 Oral](https://openaccess.thecvf.com/content_CVPR_2019/papers/Zhao_NM-Net_Mining_Reliable_Neighbors_for_Robust_Feature_Correspondences_CVPR_2019_paper.pdf) · [Code](https://github.com/sailor-z/NM-Net)
- [OANet] Learning Two-View Correspondences and Geometry Using Order-Aware Network — [ICCV 2019](https://arxiv.org/pdf/1908.04964) · [TPAMI 2020](https://ieeexplore.ieee.org/document/9310246) · [Code](https://github.com/zjhthu/OANet)
- ACNe: Attentive context normalization for robust permutation-equivariant learning — [CVPR 2020](https://arxiv.org/pdf/1907.02545) · [Code](https://github.com/vcg-uvic/acne) · [line_fitting](https://github.com/acne/line-fitting)
- [GLHA] Cascade Network with Guided Loss and Hybrid Attention for Finding Good Correspondences — [AAAI 2021](https://cdn.aaai.org/ojs/16198/16198-13-19692-1-2-20210518.pdf) · [Code](https://github.com/wenbingtao/GLHA)
- [LMCNet] Learnable motion coherence for correspondence pruning — [CVPR 2021](https://arxiv.org/pdf/2011.14563) · [Supplement](https://liuyuan-pal.github.io/LMCNet/supp.pdf) · [Code](https://github.com/liuyuan-pal/LMCNet)
- [CLNet] Progressive correspondence pruning by consensus learning — [ICCV 2021](https://arxiv.org/pdf/2101.00591) · [Code](https://github.com/sailor-z/CLNet)
- T-Net: Effective permutation-equivariant network for two-view correspondence learning — [ICCV 2021](https://openaccess.thecvf.com/content/ICCV2021/papers/Zhong_T-Net_Effective_Permutation-Equivariant_Network_for_Two-View_Correspondence_Learning_ICCV_2021_paper.pdf) · [TPAMI 2024](https://ieeexplore.ieee.org/document/10637773) · [Code](https://github.com/guobaoxiao/T-Net)
- MS2DGNet: Progressive correspondence learning via multiple sparse semantics dynamic graph — [CVPR 2022](https://openaccess.thecvf.com/content/CVPR2022/papers/Dai_MS2DG-Net_Progressive_Correspondence_Learning_via_Multiple_Sparse_Semantics_Dynamic_Graph_CVPR_2022_paper.pdf) · [Code](https://github.com/changcaiyang/MS2DG-Net)
- ConvMatch: Rethinking Network Design for Two-View Correspondence Learning — [AAAI 2023 Oral](https://openreview.net/pdf?id=DnaHIVXRzmh) · [TPAMI 2024](https://ieeexplore.ieee.org/document/10323178) · [Code](https://github.com/SuhZhang/ConvMatch)
- [ANA-Net] Learning second-order attentive context for efficient correspondence pruning — [AAAI 2023 Oral](https://arxiv.org/pdf/2303.15761) · [Code](https://github.com/DIVE128/ANANet)
- LGCNet: Feature Enhancement and Consistency Learning Based on Local and Global Coherence Network for Correspondence Selection — [ICRA 2023](https://ieeexplore.ieee.org/document/10160290)
- [NCMNet] Progressive Neighbor Consistency Mining for Correspondence Pruning — [CVPR 2023](https://openaccess.thecvf.com/content/CVPR2023/papers/Liu_Progressive_Neighbor_Consistency_Mining_for_Correspondence_Pruning_CVPR_2023_paper.pdf) · [TPAMI 2024](https://ieeexplore.ieee.org/document/10705098) · [Code](https://github.com/xinliu29/NCMNet)
- [LCT] Local Consensus Transformer for Correspondence Learning — [ICME 2023](https://ieeexplore.ieee.org/document/10219942) · [TNNLS 2024](https://ieeexplore.ieee.org/document/10750907) · [Code](https://github.com/gwang-cv/LCT)
- U-Match: Two-view Correspondence Learning with Hierarchy-aware Local Context Aggregation — [IJCAI 2023](https://www.ijcai.org/proceedings/2023/0130.pdf) · [TPAMI 2024](https://ieeexplore.ieee.org/document/10643351) · [Code](https://github.com/ZizhuoLi/U-Match)
- Local Consensus Enhanced Siamese Network with Reciprocal Loss for Two-view Correspondence Learning — [MM 2023](https://dl.acm.org/doi/pdf/10.1145/3581783.3612458)
- [GCT-Net] Graph Context Transformation Learning for Progressive Correspondence Pruning — [AAAI 2024](https://arxiv.org/pdf/2312.15971) · [Code](https://github.com/JunwenGuo/GCT-Net)
- BCLNet: Bilateral Consensus Learning for Two-View Correspondence Pruning — [AAAI 2024](https://arxiv.org/pdf/2401.03459) · [Code](https://github.com/guobaoxiao/BCLNet)
- MGNet: Learning Correspondences via Multiple Graphs — [AAAI 2024](https://arxiv.org/pdf/2401.04984) · [Code](https://github.com/Dailuanyuan2024/MGNet2024AAAI)
- VSFormer: Visual-Spatial Fusion Transformer for Correspondence Pruning — [AAAI 2024](https://arxiv.org/pdf/2312.08774.pdf) · [Code](https://github.com/sugar-fly/VSFormer)
- DeMatch: Deep Decomposition of Motion Field for Two-View Correspondence Learning — [CVPR 2024](https://openaccess.thecvf.com/content/CVPR2024/papers/Zhang_DeMatch_Deep_Decomposition_of_Motion_Field_for_Two-View_Correspondence_Learning_CVPR_2024_paper.pdf) · [Supplement](https://openaccess.thecvf.com/content/CVPR2024/supplemental/Zhang_DeMatch_Deep_Decomposition_CVPR_2024_supplemental.pdf) · [Code](https://github.com/SuhZhang/DeMatch) · [TPAMI 2025](https://ieeexplore.ieee.org/abstract/document/11119297) · [Code: DeMatch++](https://github.com/SuhZhang/DeMatchPlus)
- TrGa: Reconsidering the Application of Graph Neural Networks in Two-View Correspondence Pruning — [MM 2024](https://openreview.net/forum?id=c9I9NAbkpz) · [Code](https://github.com/Dailuanyuan2024/TrGa2024)
- CorrAdaptor: Adaptive Local Context Learning for Correspondence Pruning — [ECAI 2024](https://arxiv.org/pdf/2408.08134) · [Code](https://github.com/TaoWangzj/CorrAdaptor)
- [NACNet] Consensus Learning with Deep Sets for Essential Matrix Estimation — [NeurIPS 2024](https://proceedings.neurips.cc/paper_files/paper/2024/file/b7f09d26f9b64b5430402860158c2e19-Paper-Conference.pdf) · [Code](https://github.com/drormoran/NACNet)
- [DeMo] Deep Motion Field Consensus with Learnable Kernels for Two-view Correspondence Learning — [AAAI 2025](https://ojs.aaai.org/index.php/AAAI/article/view/32622) · [Code](https://github.com/JiajunLe/DeMo)
- NCNet: Learning to Find Non-Consistent Correspondence Using Learnable Frequency Response Function — [ICASSP 2025](https://ieeexplore.ieee.org/document/10887571) · [Code](https://github.com/Livsdjo/NCNet-Code)
- MGCA-Net: Multi-Graph Contextual Attention Network for Two-View Correspondence Learning — [IJCAI 2025](http://www.linshuyuan.com/papers/IJCAI25-MGCANET.pdf) · [Code](https://github.com/shuyuanlin/MGCANET)
- CorrNeXt: Making the ConvNet-Style Correspondence Pruner Stronger for Two-View Geometry — [MM 2025](https://dl.acm.org/doi/pdf/10.1145/3746027.3755350)
- [CSBCNet] Two-View Correspondence Pruning via Channel-Spatial Interaction and Bidirectional Consensus Interaction — [MM 2025](https://dl.acm.org/doi/pdf/10.1145/3746027.3755581) · [Code](https://github.com/jiaowohxg/CSBCNet)
- HAT-Match: Graph Transformer with Hybrid Attention for Two-View Correspondence Pruning — [ECAI 2025](https://ebooks.iospress.nl/volumearticle/75746) · [Code](https://github.com/gwang-cv/HAT-Match)
- CorrMoE: Mixture of Experts with De-stylization Learning for Cross-Scene and Cross-Domain Correspondence Pruning — [ECAI 2025](https://arxiv.org/pdf/2507.11834) · [Code](https://github.com/peiwenxia/CorrMoE)
- GeoMoE: Divide-and-Conquer Motion Field Modeling with Mixture-of-Experts for Two-View Geometry — [AAAI 2026](https://arxiv.org/pdf/2508.00592) · [Code](https://github.com/JiajunLe/GeoMoE)
- SC-Net: Robust correspondence learning via spatial and cross-channel context — [AAAI 2026](https://ojs.aaai.org/index.php/AAAI/article/view/37632)
- BAG-Net: Bidirectional Receptive-Field Graph Network for Two-View Correspondence Pruning — [IJCAI 2026](https://www.ijcai.org/proceedings/2026/193) · [Code](https://github.com/LeyiWang13/BAG-Net)
- Boosting Correspondence Learning with Structure-Aware Estimator — [ECCV 2026](https://media.eventhosts.cc/Conferences/ECCV2026/pdfs/7836.pdf) · [Code](https://github.com/Tianyu-Yan/SAE)
- [CorrMAE / GeneralPruner] Scalable and Generalizable Correspondence Pruning via Geometry-Consistent Pre-training — [TPAMI 2026](https://ieeexplore.ieee.org/document/11478731) · [arXiv](https://arxiv.org/abs/2406.05773) · [Code](https://github.com/sugar-fly/GeneralPruner)

## Traditional Motion Coherence Methods

- Robust Non-parametric Data Fitting for Correspondence Modeling — [ICCV 2013](https://openaccess.thecvf.com/content_iccv_2013/papers/Lin_Robust_Non-parametric_Data_2013_ICCV_paper.pdf)
- Bilateral Functions for Global Motion Modeling — [ECCV 2014](https://mftp.mmcheng.net/Papers/CoherentModelingS.pdf) · [Project](https://mmcheng.net/bfun/)
- RepMatch: Robust Feature Matching and Pose for Reconstructing Modern Cities — [ECCV 2016](https://publish.illinois.edu/visual-modeling-and-analytics/files/2016/08/RepMatch.pdf) · [Project](https://www.kind-of-works.com/RepMatch.html)
- GMS: Grid-based Motion Statistics for Fast, Ultra-robust Feature Correspondence — [CVPR 2017](https://openaccess.thecvf.com/content_cvpr_2017/html/Bian_GMS_Grid-based_Motion_CVPR_2017_paper.html) · [IJCV 2020](https://link.springer.com/content/pdf/10.1007/s11263-019-01280-3.pdf) · [Code](https://github.com/JiawangBian/GMS-Feature-Matcher) · [Video](https://www.bilibili.com/video/BV1Yx411h7Fe/?from=search&seid=3432739276377622963&spm_id_from=333.337.0.0&vd_source=fbdb8b9103236c54bad042c207465e2f)
- CODE: Coherence Based Decision Boundaries for Feature Correspondence — [TPAMI 2018](https://ora.ox.ac.uk/objects/uuid:0e5a62ab-fb69-472f-a1e1-49d49595db62/download_file?safe_filename=matching.pdf&file_format=application%2Fpdf&type_of_work=Journal+article) · [Project](https://www.kind-of-works.com/CODE_matching.html)

## Related Methods and Applications

- Eigen decomposition-free Training of Deep Networks with Zero Eigenvalue-based Losses — [ECCV 2018](https://openaccess.thecvf.com/content_ECCV_2018/papers/Zheng_Dang_Eigendecomposition-free_Training_of_ECCV_2018_paper.pdf) · [Code](https://github.com/Dangzheng/Eig-Free-release)
- [N3Net] Neural Nearest Neighbors Networks — [NeurIPS 2018](https://proceedings.neurips.cc/paper_files/paper/2018/file/f0e52b27a7a5d6a1a87373dffa53dbe5-Paper.pdf) · [Code](https://github.com/visinf/n3net/)
- High-dimensional Convolutional Networks for Geometric Pattern Recognition — [CVPR 2020 Oral](https://arxiv.org/pdf/2005.08144) · [Code](https://github.com/chrischoy/HighDimConvNets)
- Neural3D: Light-weight Neural Portrait Scanning via Context-aware Correspondence Learning — [MM 2020](https://qianghu-huber.github.io/qianghuhomepage/paper/MM1.pdf)

## Surveys and Benchmarks

- Deep Learning Reforms Image Matching: A Survey and Outlook — [arXiv 2025](https://arxiv.org/pdf/2506.04619)
