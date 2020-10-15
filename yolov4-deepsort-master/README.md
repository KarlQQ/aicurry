---
title: '智慧來找碴'
disqus: hackmd
---

## 智慧來找碴

### 目錄
1. [前言](#前言)
2. [所需環境](#所需環境)
3. [執行步驟](#執行步驟)
4. [參考](#參考)

### 前言
AI 的時代來臨，我們希望透過 AI 來取代工作中需要耗費長時間人力的工作，畢竟時間就是金錢，『眼👀』也是我們最珍貴的東西，就讓我們透過 AI 幫忙辨識縮短工作時間吧!

本次作品資料來源為 youtube 透過抓取開源影片的方式取得資料集，主要利用 DeepSort 模型搭配最新的yolov4 技術進行辨識與追蹤，後續自行計算規則後預期成果能將影片時間壓縮但裡面的物件以原始的方式呈現，相信此成果可搭配規則包裝成可實用的產品，後續會於簡報中附上架構原理與可應用的場景。

### 所需環境
#### Run with CPU
```python=
pip install -r requirements.txt
```
```gherkin
opencv-python==4.1.1.26
lxml
tqdm
tensorflow==2.3.0rc0
absl-py
easydict
matplotlib
pillow
```

#### Run with GPU
```python=
pip install -r requirements-gpu.txt
```
```gherkin
tensorflow-gpu==2.3.0rc0
opencv-python==4.1.1.26
lxml
tqdm
absl-py
matplotlib
easydict
pillow
```

### 訓練步驟

#### 1. 下載YOLOv4 pre-train weight
[https://drive.google.com/open?id=1cewMfusmPjYWbrnuJRuKhPMwRe_b9PaT](https://drive.google.com/open?id=1cewMfusmPjYWbrnuJRuKhPMwRe_b9PaT)

並將yolov4.weights放在path: yolov4-deepsort-master/data/

#### 2. Open main.ipynb
```python
jupyter notebook main.ipynb
```

#### 2. 按照順序執行cell
```gherkin
    每個cell執行之前請參考上方的註解
```

### 參考
https://github.com/LeonLok/Deep-SORT-YOLOv4
https://github.com/theAIGuysCode/yolov4-deepsort