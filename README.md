# LANGUAGE MODELING WITH NN.TRANSFORMER AND TORCHTEXT

[Language Modeling with nn.Transformer and TorchText — PyTorch Tutorials 2.0.0+cu117 documentation](https://pytorch.org/tutorials/beginner/transformer_tutorial.html)

#
 
## Environment

- CPU

  直接安裝 torchtext 即可

  ```
  pip install torchtext
  ```

- GPU 

  需要先確認說他是 torch 跟 torchtext 的版本是對應的

  ![version 對照表](/res/markdown/torchtext_version.png)

  例如我執行的 torch 版本為 'torch-1.13.1+cu117'，

  ```
  pip install torch==1.13.1+cu117 torchvision==0.14.1+cu117 torchaudio==0.13.1 --extra-index-url https://download.pytorch.org/whl/cu117
  ```
  
  我就應該要安裝 '0.14.1' 的 torchtext
  
  ```
  pip install torchtext==0.14.1
  ```
  
  - https://pypi.org/project/torchtext/

# 

## Dataset

- 使用 WikiText2
  - Word level: For the datasets
    - Each file contains wiki.train.tokens, wiki.valid.tokens, and wiki.test.tokens. No processing is needed other than replacing newlines with <eos> tokens.
    - The raw tokens before the addition of <unk> tokens. They should only be used for character level work or for creating newly derived datasets.
  - https://paperswithcode.com/dataset/wikitext-2
  - https://blog.salesforceairesearch.com/the-wikitext-long-term-dependency-language-modeling-dataset/

#

## Execute

- 直接 Run main.py 即可

```
python main.py
```

#

## Git Principle Git使用原則

- 修改**.gitignore**要跟大家說一下
  註解一定要寫，註解格式

  ```
  + : add 新增功能
  ~ : fix 修復bug
  - : rm 移除檔案或者功能
  # : 修改既有功能
  ```