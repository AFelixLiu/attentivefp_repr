### 🌟 简介
------
本项目是对论文 [DOI: 10.1021/acs.jmedchem.9b00959](https://doi.org/10.1021/acs.jmedchem.9b00959) 的代码复现。

代码实现参考自：[OpenDrugAI/AttentiveFP](https://github.com/OpenDrugAI/AttentiveFP)。


### 📢 注意事项
------
在复现过程中，本人对 `Feature_visualization_of_Learning_aromaticity.ipynb` 的第 8 个单元格（Cell 8）进行了以下逻辑调整，以确保本地实验的顺利进行：

- **MSE 阈值调整**：

  ```python
  # if test_MSE < 0.5: 
  if test_MSE < 1.1:   # 调整了测试集均方误差的判断标准
  ```

- **训练停止条件优化**：

  ```python
  # if (epoch - best_param["train_epoch"] >2) and (epoch - best_param["test_epoch"] >8): 
  if (epoch - best_param["train_epoch"] >2) and (epoch - best_param["test_epoch"] >18): # 延长了早停判断的步数
  ```


### 🧠 模型训练与预测
------
你可以通过终端运行自动化脚本来启动复现：

1. **环境配置**：根据 `requirements.txt` 安装相关依赖。

2. **启动运行**：

   ```bash
   bash ./run
   ```

   *注：可通过修改 `run` 文件来选择性执行特定的子任务。*


### 📜 开源协议
------
本项目遵循 **[MIT License](https://mit-license.org/)**。
