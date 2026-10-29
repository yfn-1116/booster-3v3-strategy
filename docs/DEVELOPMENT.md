# Booster 3V3 development workflow

Official Baseline → VS Code / Codex 修改策略 → Booster Studio Build / Deploy / Simulation → 记录结果 → Git commit → Git push

1. **Official Baseline:** 以 `upstream` 的官方完整项目为基线。开始实验前确认当前分支和提交，保留可回退的基线。
2. **VS Code / Codex 修改策略:** 在本仓库中进行后续策略开发；每次实验记录具体改动和参数。初始化工作区时不修改官方足球策略。
3. **Booster Studio Build / Deploy / Simulation:** 在 Booster Studio 中打开本仓库根目录，构建、部署并运行 3V3 仿真。
4. **记录结果:** 在 [`EXPERIMENTS.md`](EXPERIMENTS.md) 按模板记录版本、提交、仿真设置、比分统计、问题和结论。截图、视频及原始指标可保存在 `results/` 对应目录；这些生成文件默认不纳入 Git。
5. **Git commit:** 检查 `git diff` 和 `git status`，确认只提交需要版本管理的策略、配置与实验结论，然后提交。
6. **Git push:** 推送到自己的 `origin` 仓库。需要同步官方更新时，从 `upstream` 获取更新并单独检查合并结果。

本地仓库：`~/Booster3V3/booster-3v3-strategy`。
