# 截取文本

## 视频示例

<video controls height='100%' width='100%' src="https://encooacademy.oss-cn-shanghai.aliyuncs.com/activity/InterceptText.mp4"></video>

## 概述

支持截取指定文本内容中符合条件(开始位置和结束位置)的第一个结果。

## 属性

### 基本

参见 [通用配置项](../../Appendix/CommonConfigurationItems.md)。

### 输入

- **源文本** ：欲被截取的源文本数据。
- **开始位置** ：指定截取的开始位置，若为空或 0 则从第一个字符开始。
- **结束位置** ：指定截取的结束位置，若为空或 0 则从第一个字符开始。

### 输出

- **截取结果**：截取的文本数据。

## 使用示例

**此流程执行逻辑**：截取 `test` 字符串变量值中，开始位置为 `0` 且结束位置为 `1` 的文本，结果保存至变量 `result` 中。

![配置截取文本组件](https://docimages.blob.core.chinacloudapi.cn/images/Activities/GetSubstringActivity2021010501.png)
