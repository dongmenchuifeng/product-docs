# 复制/移动文件

## 视频示例

<video controls height='100%' width='100%' src="https://encooacademy.oss-cn-shanghai.aliyuncs.com/activity/MoveOrCopyFile.mp4"></video>

## 概述

对目标文件进行复制或移动至特定位置。效果实现同系统对文件的复制和剪切操作，同时支持目标路径的文件名更改。

## 属性

### 基本

参见 [通用配置项](../../Appendix/CommonConfigurationItems.md)。

### 输入

- **源路径** ：复制或移动的目标文件。支持相对和绝对路径。可在组件面板点击弹出对话框，选择目标文件；亦支持手动输入路径，若路径不存在，则运行失败。
- **目标路径** ：目标文件放置的目标位置。支持两种写法：仅填写目录，不提供具体文件名和后缀，此时目标位置将使用默认源文件名；填写详细文件名和后缀，此时目标位置将使用提供的文件名。
- **复制/移动** ：下拉框选择对文件进行复制或移动操作。选择复制，实现将源文件副本复制到目路径；选择移动，实现将源文件在源文件位置删除，移动放置在目标路劲，此时仅存在一个文件。两者差别在于源文件路径是否存留源文件。

### 可选项

- **文件同名替换** ：当目标路径中含有同名文件时的解决方案。勾选后，实现删除同名文件，放入复制/移动的文件；不勾选时，当有同名文件则运行失败。

## 使用示例

**此流程执行逻辑**：将E盘下的文档复制到D盘的“移动文件”的目录下面。

![配置复制/移动文件组件](https://docimages.blob.core.chinacloudapi.cn/images/Activities/moveFile-2.png)
