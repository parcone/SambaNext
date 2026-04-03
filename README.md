# SambaNext

## 📁 数据集集合

本文整理了 SambaNext 项目所使用的主要遥感语义分割数据集，包括 **LoveDA、ISPRS Potsdam、ISPRS Vaihingen**。

---

## 🏙️ 1. LoveDA - 城市与乡村土地覆盖数据集

### 1.1 数据集概述

* **全称**：Land-cover Dataset for Domain Adaptive Semantic Segmentation
* **用途**：领域自适应语义分割（Domain Adaptation Semantic Segmentation）
* **发布机构**：武汉大学等
* **论文**：LoveDA: A Remote Sensing Land-cover Dataset for Domain Adaptive Semantic Segmentation

### 1.2 数据结构

```
LoveDA/
├── Train/
│   ├── Urban/
│   │   ├── images/
│   │   └── masks_png/
│   └── Rural/
│       ├── images/
│       └── masks_png/
├── Val/
│   ├── Urban/
│   │   ├── images/
│   │   └── masks_png/
│   └── Rural/
│       ├── images/
│       └── masks_png/
└── Test/
    ├── Urban/
    │   ├── images/
    │   └── masks_png/
    └── Rural/
        ├── images/
        └── masks_png/
```

### 1.3 数据统计

* 城市样本：2542（Train）+ 1024（Val）+ 2542（Test）
* 农村样本：2542（Train）+ 1024（Val）+ 2542（Test）
* 图像分辨率：1024 × 1024
* 类别数：7 类
* 数据大小：约 9.5GB

### 1.4 类别说明

* 背景（Background）
* 建筑（Building）
* 道路（Road）
* 水体（Water）
* 植被（Vegetation）
* 农业用地（Agricultural）
* 未分类（Unknown）

### 1.5 下载方式

* 百度网盘：[https://pan.baidu.com/s/1bBQ5bx_cPRhFGWElEX5n1Q](https://pan.baidu.com/s/1bBQ5bx_cPRhFGWElEX5n1Q)
* 提取码：5prc

---

## 🏛️ 2. ISPRS Potsdam - 高分辨率遥感数据集

### 2.1 数据集概述

* 描述：德国波茨坦地区高分辨率遥感影像
* 用途：语义分割、遥感理解
* 发布机构：ISPRS
* 年份：2016

### 2.2 数据结构

```
ISPRS_Potsdam/
├── 1_DSM/
├── 1_DSM_normalisation/
├── 2_Ortho_RGB/
├── 3_Ortho_IRRG/
├── 4_Ortho_RGBIR/
├── 5_Labels_all/
├── 5_Labels_all_noBoundary/
├── 5_Labels_for_participants/
└── assess_classification_2D_ISPRS_web/
```

### 2.3 数据统计

* 影像数量：38 张
* 图像分辨率：6000 × 6000
* 地面分辨率：5 cm
* 数据模态：RGB / IRRG / RGBIR / DSM
* 类别数：6 类
* 数据大小：约 13.3GB

### 2.4 类别说明

* Surface（表面）
* Building（建筑）
* Low vegetation（低植被）
* Tree（树木）
* Car（车辆）
* Background（背景）

### 2.5 下载方式

* 百度网盘：[https://pan.baidu.com/s/1SgoM8-_JIMJbXyQ9i7eDtw](https://pan.baidu.com/s/1SgoM8-_JIMJbXyQ9i7eDtw)
* 提取码：lala

---

## 🏘️ 3. ISPRS Vaihingen - 航空遥感数据集

### 3.1 数据集概述

* 描述：德国瓦伊恩根航空影像数据
* 用途：语义分割 benchmark
* 发布机构：ISPRS
* 年份：2016

### 3.2 数据统计

* 影像数量：33 张
* 图像分辨率：约 3000 × 3000
* 地面分辨率：9 cm
* 数据模态：RGB / IRRG / DSM
* 类别数：6 类
* 数据大小：约 16GB

### 3.3 类别说明

* Surface（表面）
* Building（建筑）
* Low vegetation（低植被）
* Tree（树木）
* Car（车辆）
* Background（背景）

### 3.4 下载方式

* 百度网盘：[https://pan.baidu.com/s/1SA49cZGGuMvanqKmXvDk9w](https://pan.baidu.com/s/1SA49cZGGuMvanqKmXvDk9w)
* 提取码：lala

---

## 📥 数据获取指南

### 数据清单

| 数据集       | 提取码  | 数据大小   |
| --------- | ---- | ------ |
| LoveDA    | 5prc | 9.5GB  |
| Potsdam   | lala | 13.3GB |
| Vaihingen | lala | 16GB   |

---

## 🚀 快速开始

### 环境要求

* Python ≥ 3.7
* Conda（推荐）
* GPU（建议用于训练）

### 安装步骤

```bash
git clone https://github.com/parcone/SambaNext.git
cd SambaNext

conda create -n sambanext python=3.8
conda activate sambanext

pip install -r requirements.txt

mkdir data
cd data
```

---

## 📊 数据集对比

| 数据集       | 分辨率       | 类别数 | 样本数  | 数据大小   | 特点    |
| --------- | --------- | --- | ---- | ------ | ----- |
| LoveDA    | 1024×1024 | 7   | 10k+ | 9.5GB  | 领域自适应 |
| Potsdam   | 6000×6000 | 6   | 38   | 13.3GB | 多模态   |
| Vaihingen | 3000×3000 | 6   | 33   | 16GB   | 航空影像  |

---

## 📄 License

* LoveDA: MIT License
* ISPRS: 官方竞赛协议

---

## 🤝 贡献

欢迎提交 Issue 和 Pull Request

---

## 📞 联系方式

* 作者：parcone
* 邮箱：[p185358666@gmail.com](mailto:p185358666@gmail.com)
* GitHub：[https://github.com/parcone](https://github.com/parcone)
