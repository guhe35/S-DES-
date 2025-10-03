# S-DES 算法实现

## 简介
本项目是 S-DES (Simplified Data Encryption Standard) 算法的完整实现，提供加密、解密、UTF-8 文本处理和密钥暴力破解功能。

## 核心功能
- **图形化界面**: 简单易用的操作界面
- **S-DES 核心算法**: 实现完整的加密与解密逻辑
- **UTF-8 文本支持**: 可加密/解密包括中文在内的任意文本
- **暴力破解**: 内置多线程工具，可快速破解10位密钥
- **完整测试**: 包含5个测试关卡，确保算法的正确性

## 快速开始

### 环境要求
- Python 3.6+
- Tkinter (通常随 Python 一起安装)

### 安装依赖
```bash
pip install -r requirements.txt
```

### 运行程序
```bash
# 启动主程序
python sdes_main.py

# 直接运行测试
python sdes_tests.py
```

## 使用指南
程序启动后，界面包含四个主要功能：
1. **基本加解密**: 对8位二进制数据进行加密和解密
2. **文本处理**: 加密和解密任意 UTF-8 文本字符串
3. **暴力破解**: 输入已知的明文和密文，程序将自动找出所有可能的密钥
4. **算法信息**: 查看 S-DES 算法的内部参数

## 项目结构
```
作业/
├── sdes_algorithm.py  # S-DES 核心算法
├── sdes_gui.py        # 图形用户界面
├── sdes_tests.py      # 单元测试与验证
├── sdes_main.py       # 主程序入口
├── requirements.txt   # 项目依赖
└── README.md          # 项目文档
```

## 测试
项目包含一个全面的测试套件，用于验证算法的正确性和性能。可直接运行 `sdes_tests.py` 来执行所有测试。