# Tongji-3D: A Large-Scale Urban Outdoor Point Cloud Dataset

<p align="center">Spatial-Temporal Intellisense Laboratory, Tongji University</p>

# Introduction of the Tongji-3D datasets

The Tongji-3D dataset is a large-scale urban outdoor point cloud dataset built by Spatial-Temporal Intellisense Laboratory, Tongji University. Based on the analysis of the existing problems in the current TLS point cloud reference datasets, we aim to enrich the diversity of static point cloud datasets to improve the generalization ability of neural network algorithms effectively.

It is acquired by utilizing a high-accuracy FARO Focus3D X130 3D laser scanner in Tongji University in Shanghai, China. The collection area covers approximately 67,900 m2. This dataset includes ten scenes with over 500 million points.

This data is mainly used to test the performance of semantic segmentation algorithms for large-scale cities' scenes. The data acquisition area scenes are complex and varied, including parking lots, small squares, lawns, dormitory buildings, experimental buildings, and other scenes. The shape of each building is different, there is a certain degree of shielding between the building and the vegetation, and the density of the point cloud varies greatly. The Tongji-3D data collection area is located on the campus (**Figure 1**), which can better simulate the complex and dynamic environment of the city. The Tongji-3D dataset provides a new benchmark for testing the semantic segmentation algorithm and further enriches the diversity of the standard point cloud dataset.

![image-20210722162954388](https://i.loli.net/2021/07/22/3SN6ODfiAIjdcgr.png)

Figure 1 Data collection area of the Tongji-3D.

# **Data collection and semantic labeling** 

## Point cloud data collection

The TONGJI-3D dataset mainly uses a FOCUS 3D X130 terrestrial 3D LiDAR to collect data. The scanner has a high-resolution camera inside it to capture the color information of ground objects. It can quickly obtain high-precision point cloud data. In the data collection procedure, we set up 88 stations to obtain point cloud data of the whole region with high overlap.

## Point cloud data preprocessing

After the point cloud of the whole area is registered, the data is denoised and downsampled through the Statistical Outlier Removal (SOR) method.

The number of point clouds in the whole collection area is still significant after the downsampling. In order to facilitate processing, the collection area is divided into ten subareas, as shown in **Figure 2**.

![image-20210722163427632](https://i.loli.net/2021/07/22/Adx1CSe8mwWKIfB.png)

Figure 2 Divided subarea of the Tongji-3D coverage region.

## Point cloud semantic labeling

Data labeling is done manually with CloudCompare software. The basic principle of manual semantic annotation is that each category has a precise meaning and can be used for practical value, such as urban planning and asset management. According to the above essential criteria, ground objects are mainly divided into eight categories. These include building, vegetation, impervious surfaces, grassland, rod object, cars, bikes, and scanning artifacts. The detailed classification rules and the corresponding label values during classification are shown in Table 1.

Table 1 The classification categories of the and the corresponding ground features.

 ![image-20210722163517949](https://i.loli.net/2021/07/22/7AEzQhson593OTk.png)

![image-20210722163611649](https://i.loli.net/2021/07/22/rzCQc5uMABoIZwU.png)

Figure 3 Tongji-3D samples. (a) elevation colored point clouds; (b) colored visual point clouds; (c) manually labeled point clouds.

# Distribution of the scene categories

The Tongji-3D dataset consists primarily of buildings, vegetation, and impervious surface, which fits the characteristics of urban scenes. At the same time, the dataset also contains essential elements of urban scenes such as cars, bicycles, and pedestrians, which can better simulate the urban environment. The Tongji-3D dataset has certain advantages for point cloud semantic segmentation of city environments. From the semantic segmentation perspective of the large-scale point cloud, the Tongji-3D dataset can play an excellent complementary role in understanding the point cloud semantics of the city scenes.

![image-20210722164122381](https://i.loli.net/2021/07/22/eTcKPmh8UldowZF.png)

![image-20210722164147932](https://i.loli.net/2021/07/22/uXKjp1D6oFUwyxB.png)

# Download link

 coming soon...

# Reference

Chun Liu, Doudou Zeng, Akram Akbar, Hangbin Wu, Shoujun Jia, Zeran Xu, Han Yue. CAN: A Context-Aware Network for Semantic Segmentation Towards Large-Scale Point Clouds in Urban Environments.
