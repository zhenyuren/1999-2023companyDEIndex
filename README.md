# 上市公司数字化转型指数查询系统

## 项目介绍

这是一个基于Streamlit框架开发的上市公司数字化转型指数查询系统，支持查询1999-2023年上市公司的数字化转型指数数据。用户可以通过股票代码或企业名称进行查询，并可视化展示企业历年数字化转型指数的变化趋势。

## 功能特性

- 支持通过股票代码或企业名称进行查询
- 可选择特定年份查看数据
- 交互式折线图展示企业历年数字化转型指数趋势
- 详细的数据表格展示
- 提供统计分析（最高、最低、平均指数和增长情况）
- 现代化的用户界面，包含数据概览

## 项目结构

```
├── 1999-2023年数字转型指数总表.xlsx  # 原始数据文件
├── digital_economy_app.py          # 主要的Streamlit应用程序
├── explore_data.py                 # 数据探索脚本
├── .gitignore                      # Git忽略文件配置
└── README.md                       # 项目说明文档
```

## 快速开始

### 1. 环境准备

确保您的系统已安装以下软件：

- Python 3.7+
- pip (Python包管理工具)

### 2. 安装依赖

```bash
pip install pandas openpyxl streamlit plotly
```

### 3. 运行应用

```bash
streamlit run digital_economy_app.py
```

应用将在浏览器中打开，默认地址为：http://localhost:8501

## 使用指南

1. 在侧边栏选择搜索方式（股票代码或企业名称）
2. 选择对应的股票代码或企业名称
3. 可选：选择特定年份进行查询
4. 点击'执行查询'按钮
5. 查看企业历年数字化转型指数趋势图和详细数据

## Git仓库同步指南

### 首次设置（已完成）

当前目录已配置为Git仓库，并连接到GitHub远程仓库：
```
https://github.com/zhenyuren/1999-2023companyDEIndex.git
```

### 设置Git用户信息

请先设置您的Git用户信息：

```bash
git config user.name "您的GitHub用户名"
git config user.email "您的GitHub邮箱"
```

### 提交更改到GitHub

1. 查看修改的文件：
   ```bash
   git status
   ```

2. 添加修改的文件：
   ```bash
   git add .
   ```

3. 提交更改：
   ```bash
   git commit -m "您的提交信息"
   ```

4. 首次推送：
   ```bash
   git push -u origin main
   ```

5. 后续推送：
   ```bash
   git push origin main
   ```

### 从GitHub拉取更新

```bash
git pull origin main
```

### 常见问题解决

- 如果推送失败：先执行 `git pull --rebase origin main` 解决冲突
- 权限问题：确保您有仓库的写入权限，可能需要配置SSH密钥
- 分支问题：使用 `git branch -a` 查看所有分支

## 数据说明

数据来源于1999-2023年数字转型指数总表，包含以下字段：
- 股票代码：上市公司的股票代码
- 企业名称：上市公司的名称
- 年份：数据所属年份（1999-2023）
- 数字化转型指数：企业的数字化转型指数值

## 技术栈

- Python 3.7+
- Streamlit：用于构建交互式Web应用
- Pandas：用于数据处理和分析
- Plotly：用于数据可视化

## 注意事项

1. 数据文件较大，建议定期清理缓存以提高性能
2. 首次加载数据可能需要一些时间，请耐心等待
3. 如果遇到内存不足的问题，可以考虑分批加载数据

## 许可证

本项目仅供学习和研究使用。

## 联系方式

如有问题或建议，请通过GitHub Issues联系。