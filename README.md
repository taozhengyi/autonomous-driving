# 自动驾驶 · 基于 VLM 与世界模型

> 系统学习自动驾驶（感知 → 预测 → 规划 → 控制 → 端到端 → 世界模型/数据引擎），
> 并逐步复现经典模型（BEV、端到端、世界模型）的学习仓库。
>
📚 配套学习路线文档见 `study_docs/Autonomous Driving/`。

## 🎯 仓库定位

- **方向**：端到端自动驾驶 + 世界模型 + 数据引擎
- **目标**：读懂论文 → 复现项目 → 验证结果

## 🗺️ 学习路线总览（精简版）

```
感知(看懂环境) → 预测(他人动向) → 规划(轨迹决策) → 控制(执行)
        ↓            ↓                 ↓              ↓
   2D/3D检测     轨迹预测         行为/轨迹规划      PID/MPC
    车道线/分割      (LSTM/Transformer)  (A*/Lattice)
        ↓
   BEV 多传感器融合 (BEVFormer)
        ↓
   端到端自动驾驶 (UniAD / VAD / SparseDrive / DriveVLM)
        ↓
   世界模型 + 数据引擎 (GAIA / DriveDreamer / 数据闭环)
```

## ✅ 阶段产出清单

| 阶段 | 内容 | 交付物 |
|------|------|--------|
| 0 | 软件/数学基础 | 点云+图像可视化 |
| 1 | 深度学习 | 目标检测小模型 (YOLO) |
| 2 | 感知 | 2D 检测 + LiDAR 3D 检测 demo |
| 3 | BEV 与多传感融合 | BEVFormer 思路/可视化 |
| 4 | 轨迹预测 | Argoverse 未来轨迹 demo |
| 5 | 规划控制 | 路径规划 + 跟踪 demo |
| 6 | 端到端 | 理解/复现 UniAD 层级概念 |
| 7 | 世界模型/数据 | 世界模型 + 数据引擎思路 |
| 8 | 仿真闭环 | CARLA 自车闭环 + 论文复现 |

## 🔧 环境与依赖

- Python 3.8+ · PyTorch 2.x · CUDA 11/12
- 检测：MMDetection / Ultralytics YOLO
- 3D/点云：OpenMMLab3D、PointPillars、open3d
- 数据：nuScenes、WAYMO Open、Argoverse 2、KITTI
- 仿真：CARLA、L5Kit、SMARTS

## 🐾 进度追踪

- [ ] 读懂点云/图像，能预处理传感器数据
- [ ] 训练过 2D 检测 + 看过 LiDAR 3D 检测 demo
- [ ] 跑通 CARLA 一个闭环（自车自动跟车道）
- [ ] 实现路径规划 + 轨迹预测 demo
- [ ] 讲清 UniAD 端到端架构
- [ ] 说明 BEV 是什么、为什么统一到 BEV
- [ ] 复现一篇感知 / 端到端论文
- [ ] 打通「世界模型 → 生成数据 → 再训练」的数据飞轮思路

## 📌 里程碑

- 第 1-2 周：环境 + 传感器可视化
- 第 3-6 周：2D 检测 + LiDAR 3D 检测
- 第 7-8 周：BEV + nuScenes
- 第 9-10 周：轨迹预测 / 规划 demo
- 第 11-12 周：CARLA 闭环
- 第 13-15 周：复现一个端到端（VAD / 看 UniAD）
