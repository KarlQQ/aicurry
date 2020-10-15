## 智慧來找碴

### 目錄
1. [前言](#前言)
2. [所需環境](#所需環境)
3. [執行步驟](#執行步驟)
4. [參考](#參考)

### 前言
我們試了yolov4與yolov4 tiny
因學校hub環境權限的關係
darknet無法在學校hub使用
最後使用yolov4 run on tensorflow的套件

在project目錄裡會看到兩個資料夾
```python
yolov4-tf2
yolov4-tiny-tf2
```
都是一樣的[訓練步驟](#訓練步驟)

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
#### 1. Open main.ipynb
```python=
jupyter notebook main.ipynb
```

#### 2. 按照順序執行cell
```gherkin
    每個cell執行之前請參考上方的註解
```

### 參考
https://github.com/LeonLok/Deep-SORT-YOLOv4
https://github.com/theAIGuysCode/yolov4-deepsort