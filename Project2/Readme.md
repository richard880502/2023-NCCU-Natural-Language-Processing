#  Chinese Word Segmentation 模型修改

請修改 Code Lab 提供的 Chinese Word Segmentation 模型，使得 F1 高於 90%，且越高越好。

https://colab.research.google.com/drive/1ctn94PEX-WjhX8btMyh07oC7SV2_1HxE?usp=sharing

注意，只能修改 Assignment II 的那一格，

可以調整 tagging scheme、feature extraction 的方式，以及 CRF 模型的超參數。不要更動 Code Lab 其他部份。此外，必須手動修改程式，不能偷渡其他分類器。

可以嘗試的方向包含但不限於以下幾項，請自行發揮創意。

- 不同於 LMRS 的 tagging scheme
- 特徵設計（bigrams, trigrams, ...） 
- 特徵挑選（去除低頻特徵、無鑑別力的特徵等）
- 特徵轉換（中文部首、字元類型、聲音）
- 加入字典資訊作為特徵

# solution
我使用以下的方法
- 將特徵設計修改成bigram
- 新增字典資訊作為特徵
- 修改模型參數 (min_freq={20 -> 10}, max_iterations={300 -> 400})

最終結果
- Recall: 0.9419975832326347
- Precision: 0.9315789907447852
- F1: 0.9367593191122604
