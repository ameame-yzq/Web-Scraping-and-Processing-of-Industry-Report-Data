# Web-Scraping-and-Processing-of-Industry-Report-Data
# 工信部行业报告数据爬取与处理

## 项目简介

这个项目旨在从中国工业和信息化部（工信部）的官方网站爬取并处理行业报告数据。该脚本可以自动获取最新的行业数据，包括原材料工业、装备工业、消费品工业、通信业、电子信息制造业、软件业、互联网和网络安全等领域的报告。

## 功能特性

- 从工信部网站自动爬取最新行业报告数据
- 对数据进行分类和处理
- 提取报告内容、图片和PDF文件
- 保存数据为多种格式（TXT、Markdown、JSON）
- 实现了自动重试和错误处理机制
- 使用随机User-Agent和延时来避免被封IP

## 依赖库

- requests
- BeautifulSoup
- urllib
- re
- json
- os
- base64
- time
- random

## 使用方法

1. 确保已安装所有依赖库
2. 运行Jupyter Notebook中的代码单元格
3. 脚本将自动创建`miit_data`目录并保存所有提取的数据

## 输出文件

- `miit_urls.txt`: 包含所有爬取的URL
- `miit_data.md`: Markdown格式的数据表格，包含行业、标题和日期
- `miit_extracted_data.json`: 提取的详细数据（不包含base64编码的图片）
- `miit_extracted_data_with_base64.json`: 完整的提取数据，包含base64编码的图片

## 注意事项

- 请遵守网站的使用条款和robots.txt文件
- 建议适当调整爬取频率，避免对目标网站造成过大压力
- 该脚本仅用于学习和研究目的，请勿用于商业用途

## 贡献

欢迎提交问题和改进建议。如果您想为这个项目做出贡献，请提交pull request。

