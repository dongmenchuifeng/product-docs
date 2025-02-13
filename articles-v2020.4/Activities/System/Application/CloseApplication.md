# 关闭程序

## 视频示例

<video controls height='100%' width='100%' src="https://encooacademy.oss-cn-shanghai.aliyuncs.com/activity/CloseProgram.mp4"></video>

## 概述

关闭指定UI元素相对于的应用程序（包括桌面程序和浏览器）。

## 属性

### 基本

参见 [通用配置项](../../Appendix/CommonConfigurationItems.md)。

### 目标

- **选择器** ：用于指示要关闭的目标程序。可通过点击“指定程序”自动生成。
- **匹配超时(毫秒)** ：默认为5000毫秒，可配置超时时间。
- **控件元素** ：传入“打开程序”的输出变量，作为目标程序执行关闭操作。此项和上述字段二选一填入。

### 可选项

- **窗口置顶**：选择运行时的桌面窗口是否置顶，部分界面窗口置顶时无法获取到窗口内的内容，这时需要将此属性设置为不置顶。

## 使用示例

**此流程执行逻辑**：用选择器指定关闭新的记事本程序

![配置关闭程序组件](https://docimages.blob.core.chinacloudapi.cn/images/Activities/closeApp-2.png)
