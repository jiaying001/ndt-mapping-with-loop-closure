# NDT mapping with loop closure
## Overview
This is the extraction of the mapping pacakge from the [Autoware](https://github.com/autowarefoundation/autoware).
The license is in accordance with Autoware.
The loop-closure method implemented in this package referes to LIO-SAM. 

这是个基于NDT mapping（参考 Autoware）和 回环检测 （参照 LIO-SAM）的建图包。
NDT mapping 原理可参考 [ndt_mapping 算法与代码对应及运行](https://www.notion.so/ndt_mapping-6c8e00266fd1441bab2026fb474b66f6)。 
LIO-SAM 回环检测部分可参考 [LIO-SAM源码解析(四)：MapOptimization](https://zhuanlan.zhihu.com/p/352148894) 。

## Dependency
- [PCL](https://pointclouds.org/)
- [GSTAM](https://gtsam.org/get_started/)

## Usage
 ### Input
  - Point Cloud (/velodyne_points)
 ### Output
  - /ndt_map
  - /keyposes
  - /current_pose
 ### Run the packge
 `` roslaunch lidar_localizer ndt_mapping.launch  ``
   

