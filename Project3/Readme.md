# 立場偵測模型

請修改以下 Code Lab 提供的立場偵測模型，並且達成 Code Lab 中的目標1與目標2 。

https://colab.research.google.com/drive/1u5G_cNvquL9WZ9LhTgiiJ_FC0CqLVldo?usp=sharing

注意，只能修改「Assignment III 修改區」的那一格，

可以調整 Trainer、訓練參數、模型、loss function 等各種建模方式，但不要更動 Code Lab 其他部份。此外，必須手動修改程式，不能偷渡外部 API 如 ChatGPT。

可以嘗試的方向包含但不限於以下幾項，請自行發揮創意。

# solution
- 利用 scheduler 提供的動態調整學習率，給予 warm up 並逐步找到最佳的策略
- 並且保存最佳的訓練結果
  
最終 **F1** 分數約可以維持在０.６１~０.６２ (原始約０.58）

