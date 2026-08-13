# 数据文件夹

结构：
- `./dataset/` -> 实际数据集（通常很大，用软链接指向外部存储，这里默认 .gitignore）
- `./preprocess/` -> 预处理脚本
- `./utils/` -> 数据加载、变换工具函数
- `./visualize/` -> 相机/点云/BEV 可视化脚本

## 支持数据集

- [ ] nuScenes （3D检测，BEV）
- [ ] WAYMO Open （大规模自动驾驶数据集）
- [ ] Argoverse 2 （轨迹预测）
- [ ] KITTI （入门经典）
- [ ] BDD100K （2D检测/分割）
