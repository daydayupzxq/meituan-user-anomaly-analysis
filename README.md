# 美团用户异常检测与画像分析

基于订单、领券和访问行为特征的用户异常检测、聚类与画像分析。

## 仓库内容

- `notebooks/`：按原文件名保存的 Notebook；为控制仓库体积，已清除嵌入式运行输出，代码和 Markdown 说明均保留。
- `results/`：原项目中可直接展示且小于 10 MB 的图表/汇总结果。
- `requirements.txt`：根据 Notebook import 语句自动整理的依赖候选列表。

## Notebook 索引

| Notebook | 代码单元 | Markdown 单元 | 清理前输出数 |
|---|---:|---:|---:|
| `Untitled.ipynb` | 3 | 0 | 2 |
| `异常检测.ipynb` | 87 | 2 | 59 |

## 已保留结果

- `results/cluster_stats.xlsx`
- `results/user_portrait_with_features.png`
- `results/不同群体特征雷达图.jpg`
- `results/异常用户指标差异倍数值雷达图.jpg`
- `results/特征均值条形图.jpg`
- `results/特征相关性热力图.jpg`
- `results/特征相关性热力图对比.jpg`
- `results/特征雷达图.jpg`
- `results/雷达图优化版.jpg`

## 数据说明

原目录包含大量原始和中间 CSV/TXT 数据，部分文件超过 GitHub 100 MB 单文件限制，且行为或用户明细数据可能不适合公开发布。因此本仓库不提交这些数据。运行 Notebook 前，请将合法取得的数据放入本地数据目录，并按 Notebook 中的路径配置进行调整。

## 运行方式

```bash
python -m venv .venv
# Windows
.venv\Scripts\activate
pip install -r requirements.txt
jupyter notebook
```

建议按 Notebook 中的数据处理顺序运行。由于原始数据未包含在仓库中，完整复现需要自行准备数据并修正本地绝对路径。

## 整理说明

- 未包含 `.ipynb_checkpoints`、IDE 配置和缓存文件。
- 未包含大体积原始/中间数据。
- Notebook 的历史输出已清空，避免仓库过大；关键外部图表保存在 `results/`。
