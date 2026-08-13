# BEV 鸟瞰图 - 多传感器融合

包含：
- BEV 投影算法
- 相机+LiDAR融合
- Transformer 方法

## 经典论文

| 论文 | 核心贡献 | 链接 |
|------|----------|------|
| BEVFormer | 时空Transformer BEV | https://arxiv.org/abs/2203.17270 |
| PETR | 位置嵌入变换 | https://arxiv.org/abs/2206.01256 |
| BEVDet | 纯视觉高效BEV | https://arxiv.org/abs/2112.11015 |
| Lift-Splat-Shoot | 几何投影BEV | https://arxiv.org/abs/2008.05711 |

## 计划

- [ ] 实现相机到 BEV 投影
- [ ] 理解视锥注意力机制
- [ ] 在 nuScenes 上可视化 BEV 结果
