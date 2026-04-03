# SambaNext

## 📁 数据集集合

### 🏙️ LoveDA - 城市与乡村土地覆盖数据集

#### 📊 数据集概述
- **描述**: Land-cover Dataset for Domain Adaptive Semantic Segmentation
- **用途**: 领域自适应语义分割研究
- **发布**: 武汉大学等机构
- **论文**: "LoveDA: A Remote Sensing Land-cover Dataset for Domain Adaptive Semantic Segmentation"

#### 🗂️ 数据结构
```
LoveDA/
├── Train/
│   ├── Urban/          # 城市区域训练数据
│   │   ├── images/     # 原始遥感影像
│   │   └── masks_png/  # 标注掩码
│   └── Rural/          # 农村区域训练数据
│       ├── images/     # 原始遥感影像  
│       └── masks_png/  # 标注掩码
├── Val/
│   ├── Urban/          # 城市区域验证数据
│   └── Rural/          # 农村区域验证数据
└── Test/
    ├── Urban/          # 城市区域测试数据
    └── Rural/          # 农村区域测试数据
```

#### 📈 数据统计
- **城市样本**: 训练集(2542张) + 验证集(1024张) + 测试集(2542张)
- **农村样本**: 训练集(2542张) + 验证集(1024张) + 测试集(2542张)
- **图像分辨率**: 1024×1024像素
- **类别数**: 7类 (背景、建筑、道路、水体、植被、农业用地、未分类)
- **数据大小**: ~3GB

#### 🔗 下载链接
- **百度网盘**: [LoveDA数据集](https://pan.baidu.com/s/1bBQ5bx_cPRhFGWElEX5n1Q)
- **提取码**: `5prc`

---

### 🏛️ ISPRS Potsdam - 德国波茨坦数据集

#### 📊 数据集概述
- **描述**: 德国波茨坦地区高分遥感影像数据集
- **用途**: 2D语义分割竞赛数据集
- **发布**: ISPRS (国际摄影测量与遥感学会)
- **年份**: 2016年

#### 🗂️ 数据结构
```
ISPRS_Potsdam/
├── 1_DSM/                    # 数字表面模型
├── 1_DSM_normalisation/      # 标准化DSM
├── 2_Ortho_RGB/              # RGB正射影像
├── 3_Ortho_IRRG/             # 红外-红-绿波段影像
├── 4_Ortho_RGBIR/            # RGB-红外波段影像
├── 5_Labels_all/             # 完整标注数据
├── 5_Labels_all_noBoundary/  # 无边界标注
├── 5_Labels_for_participants/        # 参赛者标注
└── assess_classification_2D_ISPRS_web/ # 评估脚本
```

#### 📈 数据统计
- **影像数量**: 38张高分辨率影像
- **图像分辨率**: 6000×6000像素 (5cm地面分辨率)
- **波段组合**: RGB、IRRG、RGBIR、DSM
- **类别数**: 6类 (表面、建筑、低植被、树木、汽车、背景)
- **数据大小**: ~15GB

#### 🔗 下载链接
- **百度网盘**: [Potsdam数据集](https://pan.baidu.com/s/1SgoM8-_JIMJbXyQ9i7eDtw)
- **提取码**: `lala`

---

### 🏘️ ISPRS Vaihingen - 德国瓦伊恩根数据集

#### 📊 数据集概述
- **描述**: 德国瓦伊恩根地区航空影像数据集
- **用途**: 2D语义分割竞赛数据集
- **发布**: ISPRS (国际摄影测量与遥感学会)
- **年份**: 2016年

#### 📈 数据统计
- **影像数量**: 33张高分辨率影像
- **图像分辨率**: 约3000×3000像素 (9cm地面分辨率)
- **波段组合**: RGB、IRRG、DSM
- **类别数**: 6类 (表面、建筑、低植被、树木、汽车、背景)
- **数据大小**: ~2GB

#### 🔗 下载链接
- **百度网盘**: [Vaihingen数据集](https://pan.baidu.com/s/1SA49cZGGuMvanqKmXvDk9w)
- **提取码**: `lala`

---

### 🌆 Toronto - 多伦多城市数据集

#### 📊 数据集概述
- **描述**: 加拿大多伦多城市遥感影像数据集
- **用途**: 城市地物分类和语义分割
- **特点**: 高分辨率城市遥感数据

#### 📈 数据统计
- **覆盖区域**: 多伦多市区
- **数据类型**: 高分辨率遥感影像
- **应用场景**: 城市规划、地物分类
- **数据大小**: ~1GB

#### 🔗 下载链接
- **百度网盘**: [Toronto数据集](https://pan.baidu.com/s/12KZ4yYpPSWDErF6xej0Abw)
- **提取码**: `lala`

## 📥 数据获取指南

### 🌐 百度网盘下载 (推荐)

| 数据集 | 链接 | 提取码 | 大小 |
|--------|------|--------|------|
| LoveDA | [下载](https://pan.baidu.com/s/1bBQ5bx_cPRhFGWElEX5n1Q) | `5prc` | ~3GB |
| Potsdam | [下载](https://pan.baidu.com/s/1SgoM8-_JIMJbXyQ9i7eDtw) | `lala` | ~15GB |
| Vaihingen | [下载](https://pan.baidu.com/s/1SA49cZGGuMvanqKmXvDk9w) | `lala` | ~2GB |
| Toronto | [下载](https://pan.baidu.com/s/12KZ4yYpPSWDErF6xej0Abw) | `lala` | ~1GB |

### 📚 原始数据源
- LoveDA: [官方下载页面](https://github.com/Junjue-Wang/LoveDA)
- ISPRS Potsdam: [ISPRS官方页面](http://www2.isprs.org/commissions/comm3/wg4/2d-sem-label-potsdam.html)

### 方法3: 分块下载脚本
```python
# 使用提供的下载脚本
python download_script.py
```

## 🚀 快速开始

### 📋 环境要求
- Python 3.7+
- 推荐使用Conda环境
- GPU支持 (可选，用于深度学习)

### 🛠️ 安装步骤

```bash
# 1. 克隆仓库
git clone https://github.com/parcone/SambaNext.git
cd SambaNext

# 2. 创建虚拟环境
conda create -py=3.8 sambanext
conda activate sambanext

# 3. 安装依赖
pip install -r requirements.txt

# 4. 下载数据集
mkdir data
cd data

# 5. 选择数据集下载
# LoveDA (城市与乡村土地覆盖)
wget -O LoveDA.zip "百度网盘链接"  # 或手动下载

# ISPRS Potsdam (德国波茨坦)
wget -O Potsdam.zip "百度网盘链接"

# ISPRS Vaihingen (德国瓦伊恩根)  
wget -O Vaihingen.zip "百度网盘链接"

# Toronto (多伦多城市)
wget -O Toronto.zip "百度网盘链接"

# 6. 解压数据集
unzip LoveDA.zip
unzip Potsdam.zip
unzip Vaihingen.zip
unzip Toronto.zip
```

### 🎯 数据集使用示例

```python
# LoveDA数据集加载示例
import os
import numpy as np
from PIL import Image

def load_loveda_data(data_path, split='train', domain='urban'):
    """加载LoveDA数据集"""
    image_dir = os.path.join(data_path, f'{split.capitalize()}/{domain.capitalize()}/images')
    mask_dir = os.path.join(data_path, f'{split.capitalize()}/{domain.capitalize()}/masks_png')
    
    images = []
    masks = []
    
    for img_name in sorted(os.listdir(image_dir)):
        # 加载图像
        img_path = os.path.join(image_dir, img_name)
        image = np.array(Image.open(img_path))
        
        # 加载掩码
        mask_path = os.path.join(mask_dir, img_name.replace('.png', '.png'))
        mask = np.array(Image.open(mask_path))
        
        images.append(image)
        masks.append(mask)
    
    return np.array(images), np.array(masks)

# 使用示例
# images, masks = load_loveda_data('./data/LoveDA', split='train', domain='urban')
print(f"加载完成: {len(images)} 张图像")
```

### 📊 数据集对比

| 数据集 | 分辨率 | 类别数 | 样本数 | 特点 |
|--------|--------|--------|--------|------|
| LoveDA | 1024×1024 | 7 | 10,000+ | 城市vs乡村，领域自适应 |
| Potsdam | 6000×6000 | 6 | 38 | 超高分辨率，多光谱 |
| Vaihingen | 3000×3000 | 6 | 33 | 高分辨率，航空影像 |
| Toronto | 变化 | 多种 | 变化 | 城市规划应用 |

## 📄 许可证

- LoveDA: MIT License
- ISPRS Potsdam: ISPRS License

## 🤝 贡献

欢迎提交Issue和Pull Request！

## 📞 联系方式

- 作者: parcone
- 邮箱: parcone@github.com
