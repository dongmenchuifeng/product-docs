# 写入单元格

## 视频示例

<video controls height='100%' width='100%' src="https://encooacademy.oss-cn-shanghai.aliyuncs.com/activity/WriteCell.mp4"></video>

## 概述

使用组件，写入数据到 Excel 文件中的指定单元格。

## 属性

### 基本

参见 [通用配置项](../../Appendix/CommonConfigurationItems.md)。

### 输入

- **数据** ：写入单元格内的数据。

    >**说明：**
    >
    >可传入“读取单元格” 的输出变量，实现复制粘贴效果，同时保持复制源的数据格式。

### 目标

- **单元格** ：写入数据的目标单元格地址。当输入区域时，则在指定区域每一个单元格内输入相同数据。如，`"A1"`或`"A1:C3"`。
- **工作表** ：写入数据的目标工作表。若指定工作表不存在，则在 Excel 文件中新建该工作表。如，`"Sheet1"`。

## 使用示例

**前置必要组件**：[读取单元格](../OfficeExcel/ReadCell.md)

**此流程执行逻辑**：将读取到的Excel的"Sheet1"工作表中"A1"单元格的内容写入到"Sheet2"工作表中"A1"单元格中。

![配置写入单元格组件](https://docimages.blob.core.chinacloudapi.cn/images/Activities/ReadCell2.png)
