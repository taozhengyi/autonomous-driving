# 仿真 - CARLA / SMARTS

仿真环境代码：
- `carla_agent/` -> CARLA 客户端代码，自车控制
- `data_collection/` -> 从仿真采集数据脚本
- `planning_control/` -> PID / MPC / 学习式规划实现
- `closed_loop/` -> 端到端闭环测试脚本

## 计划

- [ ] 跑通 CARLA 基础闭环
- [ ] 实现 PID 车道保持
- [ ] 实现简单路径规划
- [ ] 采集仿真数据用于训练
