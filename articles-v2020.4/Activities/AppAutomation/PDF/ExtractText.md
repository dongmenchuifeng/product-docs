# 读取文本

## 视频示例

<video controls height='100%' width='100%' src="https://encooacademy.oss-cn-shanghai.aliyuncs.com/activity/ReadText.mp4"></video>

## 概述

可实现获取指定 PDF 文件中的文本。

## 属性

### 基本

参见 [通用配置项](../../Appendix/CommonConfigurationItems.md)。

### 输入

- **读取角度** ：指定读取时文件旋转的角度。
- **文件路径** ：输入欲被提取文本的 PDF 文件路径。

### 输出

- **结果**：输出读取的文本数据。

### 可选项

- **开始页码** ：输入被读取文本的 PDF 文件开始页码，若为空则从第一页开始读取。
- **结束页码** ：输入被读取文本的 PDF 文件结束页码，若为空则为最后一页。

## 使用示例

**此流程执行逻辑**：读取 "D:\\滴滴电子发票 (1).pdf" 文件的第一页中的文字，识别后的文字保存至 result 变量中。

![配置读取文本组件](https://docimages.blob.core.chinacloudapi.cn/images/Activities/ExtractText_2.png)
