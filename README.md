# Point Cloud Registration for LiDAR and Photogrammetric Data: a Critical Synthesis and Performance Analysis on Classic and Deep Learning Algorithms
Ningli Xu, Rongjun Qin, Shuang Song  

ISPRS Open Journal of Photogrammetry and Remote Sensing (2023)  

[[arxiv]](https://arxiv.org/abs/2302.07184)  

Three-dimensional (3D) point cloud registration is a fundamental step for many 3D modeling and mapping applications. Existing approaches are highly disparate in the data source, scene complexity, and application, therefore the current practices in various point cloud registration tasks are still ad-hoc processes. Recent advances in computer vision and deep learning have shown promising performance in estimating rigid/similarity transformation between unregistered point clouds of complex objects and scenes. However, their performances are mostly evaluated using a limited number of datasets from a single sensor (e.g. Kinect or RealSense cameras), lacking a comprehensive overview of their applicability in photogrammetric 3D mapping scenarios. In this work, we provide a comprehensive review of the state-of-the-art (SOTA) point cloud registration methods, where we analyze and evaluate these methods using a diverse set of point cloud data from indoor to satellite sources. The quantitative analysis allows for exploring the strengths, applicability, challenges, and future trends of these methods. In contrast to existing analysis works that introduce point cloud registration as a holistic process, our experimental analysis is based on its inherent two-step process to better comprehend these approaches including feature/keypoint-based initial coarse registration and dense fine registration through cloud-to-cloud (C2C) optimization. More than ten methods, including classic hand-crafted, deep-learning-based feature correspondence, and robust C2C methods were tested. We observed that the success rate of most of the algorithms are fewer than 40% over the datasets we tested and there are still are large margin of improvement upon existing algorithms concerning 3D sparse corresopondence search, and the ability to register point clouds with complex geometry and occlusions. With the evaluated statistics on three datasets, we conclude the best-performing methods for each step and provide our recommendations, and outlook future efforts.


# Awesome registration methods
## - 3D Non-Rigid Registration
- Feature preserving non-rigid iterative weighted closest point and semi-curvature registration. TIP. 2022
- Accurate Point Cloud Registration with Robust Optimal Transport. NIPS. 2021
- Quasi-Newton Solver for Robust Non-Rigid Registration. CVPR 2020.


## - 3D Rigid Registration
### Learning Based
- Correspondence-Free Point Cloud Registration with SO(3)-Equivariant Implicit Shape Representations. PMLR 2022.
- PREDATOR: Registration of 3D Point Clouds with Low Overlap. CVPR2021  
- RPM-Net: Robust Point Matching using Learned Features. CVPR2020  
- Robust Point Cloud Registration Framework Based on Deep Graph Matching. CVPR2021  
- SpinNet: Learning a General Surface Descriptor for 3D Point Cloud Registration. CVPR2021  
- PointDSC: Robust Point Cloud Registration Using Deep Spatial Consistency. CVPR2021  
- UnsupervisedR&R: Unsupervised Point Cloud Registration via Differentiable Rendering. CVPR2021  
- End-to-End Learning Local Multi-view Descriptors for 3D Point Clouds. CVPR2020  

### Detector/Descriptor
- (MeshDOG)Keypoints and Local Descriptors of Scalar Functions on 2D Manifolds. IJCV 2012
- Scale-invariant features for 3-D mesh models." TIP 2012
- On the Repeatability and Quality of Keypoints for Local Feature-based 3D Object Retrieval from Cluttered Scenes. IJCV 2009.

### Fine Registration 
- DICP: Doppler Iterative Closest Point Algorithm. arxiv 2022
- Stein ICP for Uncertainty Estimation in Point Cloud Matching. ICRA. 2022
- Sparse point cloud registration and aggregation with mesh‐based generalized iterative closest point. 2021
- Registration of 3D Point Sets Using Correntropy Similarity Matrix. 2021
- Provably Approximated Point Cloud Registration. ICCV'2021
- Scale-Adaptive ICP. PR. 2021.  
- LSG-CPD: Coherent Point Drift with Local Surface Geometry for Point Cloud Registration. ICCV'2021  
- Fast and Robust Iterative Closest Point. TPAMI 2021  
- Estimating Motion Uncertainty with Bayesian ICP. ICRA. 2020
- Analysis of robust functions for registration algorithms.ICRA 2019.   
- FilterReg: Robust and Efficient Probabilistic Point-Set Registration using Gaussian Filter and Twist Parameterization. CVPR'2019  
- Analysis of Robust Functions for Registration Algorithms. ICRA 2019.
- Quality-based registration refinement of airborne LiDAR and photogrammetric point clouds.ISPRS 2019  
- A symmetric objective function for ICP."ACM Transactions on Graphics. TOG 2019  
- Effective scaling registration approach by imposing the emphasis on the scale factor. 2019  
- Correntropy based scale ICP algorithm for robust point set registration. 2019  
- https://opals.geo.tuwien.ac.at/html/stable/ModuleStripAdjust.html
- CICP: Cluster Iterative Closest Point for sparse–dense point cloud registration. 2018 RAS.
- AA-ICP: Iterative closest point with Anderson acceleration.ICRA, 2018.
- Multi-Channel Generalized-ICP: A robust framework for multi-channel scan registration. 2017. RAS
- GOGMA: Globally-Optimal Gaussian Mixture Alignment. 2016 CVPR.
- A GMM based uncertainty model for point clouds registration. 2016. RAS
- Multi channel generalized-ICP. ICRA, 2014.
- Sparse iterative closest point. CGF 2013  
- Toward mutual information based automatic registration of 3D point clouds. 2012 ICIRS
- Point set registration: Coherent point drift. TPAMI 2010  
- [GMMReg]Robust point set registration using gaussian mixture models. TPAMI 2011.
- A scale stretch method based on ICP for 3D data registration. 2009  
- [KC] A correlation-based approach to robust point set registration." ECCV 2004.
- [Hiearchical ICP] A multi-resolution ICP with heuristic closest point search for fast and robust 3D registration of range images. 2003
- The normal distributions transform: A new approach to laser scan matching. IROS 2003  
- ICP registration using invariant features. TPAMI 2002.
- Multi-scale EM-ICP: A Fast and Robust Approach for Surface Registration. ECCV 2002.
- Efficient variants of the ICP algorithm. IC3DIM 2001  
- Object modelling by registration of multiple range images. IVC 1992  
- Method for registration of 3-D shapes. ICOP 1992.  

### Coarse Registration
- Fast Semantic-Assisted Outlier Removal for Large-scale Point Cloud Registration. arxiv'2022
- Robust global registration of point clouds by closed-form solution in the frequency domain. ISPRS Journal. 2021
- [4plane PCS] 4-Plane congruent sets for automatic registration of as-is 3D point clouds with 3D BIM models. 2018  
- [V4PCS] V4PCS: Volumetric 4PCS algorithm for global registration. 2017
- [Plane2Plane] Efficient and Accurate Registration of Point Clouds With Plane to Plane Correspondences. ICCV 2017  
- Go-ICP. TPAMI 2016
- [Scale 4PCS]Fully Automatic Registration of Image Sets on Approximate Geometry. IJCV 2013
- Robust global registration." SGP 2005.  
- Least-Squares Fitting of Two 3-D Point Sets. TPAMI 1987  
- Closed-form solution of absolute orientation using unit quaternions. JOSA 1987  

## Robust Estimation  
- A Single Correspondence Is Enough: Robust Global Registration to Avoid Degeneracy in Urban Environments. ICRA'2022
- SC^2-PCR: A Second Order Spatial Compatibility for Efficient and Robust Point Cloud Registration. CVPR'2022
- A Practical O (N2) Outlier Removal Method for Point Cloud Registration. TPAMI 2021.
- A review on robust M-estimators for regression analysis. 2021
- Graduated Non-Convexity for Robust Spatial Perception: From Non-Minimal Solvers to Global Outlier Rejection. ICRA 2020.  
- TEASER: Fast and Certifiable Point Cloud Registration. T-RO'2020  
- A Practical Maximum Clique Algorithm for Matching with Pairwise Constraints. 2019
- GORE: Guaranteed Outlier Removal for Point Cloud Registration with Correspondences. TPAMI'2018  
- FGR: Fast Global Registration. ECCV'2016
- On the Unification of Line Processes, Outlier Rejection, and Robust Statistics with Applications in Early Vision. IJCV 1996

### Survey  
- [Nonrigid] A survey of non-rigid 3D registration. arxiv. 2022
- [Descriptor design] Evaluating Local Geometric Feature Representations for 3D Rigid Data Matching. 2019 TIP  
- [Descriptor application scenario] A Comprehensive Performance Evaluation of 3D Local Feature Descriptors. 2016 IJCV.  
- [Descriptor for indoor,outdoor] Evaluation of 3D feature descriptors for multi-modal data registration. 2013 IC3DV
- [Descriptor with color]Influence of Colour and Feature Geometry on Multi-modal 3D Point Clouds Data Registration. 2014 IC3DV
- [Descriptor for large-scale scene]An Evaluation of Local Shape Descriptors in Probabilistic Volumetric Scenes. BMVC 2012
- [Detector] Performance Evaluation of 3D Keypoint Detectors. 2012 IJCV  
- [Robust Estimation] A Performance Evaluation of Correspondence Grouping Methods for 3D Rigid Data Matching. TPAMI'2019  
- [RANSAC-type] A Comparative Analysis of RANSAC Techniques Leading to Adaptive Real-Time Random Sample Consensus. ECCV 2008.  
- [ICP on slam] Comparing ICP variants on real-world data sets. 2013 Autonoumous Robots.  
- [Rigid Non-rigid] Registration of 3D point clouds and meshes: A survey from rigid to nonrigid. 2012 TVCG
- [LiDAR] Registration of Laser Scanning Point Clouds: A Review. 2018 Sensors. 
- [Defomable Correspondence]Recent advances in shape correspondence. 2019 Visual Computer  
- [Correspondence] A Survey on Shape Correspondence. CGF 2012
- [Corase and Fine Registration]A review of recent range image registration methodswith accuracy evaluation. IVC 2006.
- Recent developments and trends in point set registration methods。 2017

### Lecture
- [[SE2 SE3 Lie group](https://ethaneade.com/lie.pdf)]
- [[SE3 Lie group](https://jinyongjeong.github.io/Download/SE3/jlblanco2010geometry3d_techrep.pdf)]
- [[Recover euler angle from matrix](http://eecs.qmul.ac.uk/~gslabaugh/publications/euler.pdf)]
- [[CMU ICP-variant lecture](https://cs.gmu.edu/~kosecka/cs685/cs685-icp.pdf)]   
- [[Stanford Quaternion](http://graphics.stanford.edu/courses/cs348a-17-winter/Papers/quaternion.pdf)]  
- [[EM and GMM](https://stephens999.github.io/fiveMinuteStats/intro_to_em.html)]  
- [[EM and GMM](http://www.columbia.edu/~mh2078/MachineLearningORFE/EM_Algorithm.pdf)]  
- [[SIFT](https://aishack.in/tutorials/sift-scale-invariant-feature-transform-log-approximation/)]  
- [[ADMM](https://web.stanford.edu/~boyd/papers/pdf/admm_slides.pdf)]
- [[Wiki Point set registration](https://en.wikipedia.org/wiki/Point_set_registration)]
- [[Point-to-Point, SVD](https://igl.ethz.ch/projects/ARAP/svd_rot.pdf)]
- [[Point-to-Plane, lineear approximation](https://www.comp.nus.edu.sg/~lowkl/publications/lowk_point-to-plane_icp_techrep.pdf)]
- [[Point-to-Plane, Rodrigues approximation](https://dl.acm.org/doi/abs/10.1145/3306346.3323037)]
- [[Mutual Information](https://courses.cs.washington.edu/courses/cse577/11au/notes/Z5-Mutual-Information.pdf)]

## - 2D-3D Registration
- Phase-Congruency-Based Scene Abstraction Approach for 2D-3D Registration of Aerial Optical and LiDAR Images. AEORS 2020 
- DRMIME: Differentiable Mutual Information and Matrix Exponential for Multi-Resolution Image Registration. 2020

## - 2D-2D Registration
- Multimodal Remote Sensing Image Registration Methods and Advancements: A Survey. RS 2021
- Co-Attention for Conditioned Image Matching
- Automatic UAV image geo-registration by matching UAV images to georeferenced image data. Remote Sensing 2017  
- Universal correspondence network. arXiv 2016.
- Mutual-Information-Based Registration of Medical Images: A Survey. 2003
- (Optimization)Comparative evaluation of multiresolution optimization strategies for multimodality image registration by maximization of mutual information. 1999
- (classic) Alignment by Maximization of Mutual Information. 1997
## Dataset
- [[3DCSR, 2021, cross-source: Kinect_Lidar and Kinect_SFM ](http://multimediauts.org/3D_data_for_registration/)]  
- [[nuScenes, 2020, LiDAR like kitti](https://arxiv.org/abs/1903.11027#:~:text=Robust%20detection%20and%20tracking%20of,deployment%20of%20autonomous%20vehicle%20technology.&text=It%20has%207x%20as%20many,3D%20detection%20and%20tracking%20metrics.)]  
- [[WHU-TLS,2020, TLS](https://www.sciencedirect.com/science/article/pii/S0924271620300836)]  
- [[RESSO,2019, TLS](https://3d.bk.tudelft.nl/liangliang/publications/2019/plade/resso.html)]  
- [[ETH PRS TLS](https://prs.igp.ethz.ch/research/completed_projects/automatic_registration_of_point_clouds.html)]  
- [[ETH ASL](https://projects.asl.ethz.ch/datasets/doku.php?id=laserregistration:laserregistration)]  

## Citation
```bibtex
@article{xu2023point,
  title={Point cloud registration for LiDAR and photogrammetric data: A critical synthesis and performance analysis on classic and deep learning algorithms},
  author={Xu, Ningli and Qin, Rongjun and Song, Shuang},
  journal={ISPRS Open Journal of Photogrammetry and Remote Sensing},
  pages={100032},
  year={2023},
  publisher={Elsevier}
}
'''

