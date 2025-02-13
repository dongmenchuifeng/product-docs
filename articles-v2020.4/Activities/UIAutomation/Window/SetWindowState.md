# 设置窗口

## 视频示例

<video controls height='100%' width='100%' src="https://encooacademy.oss-cn-shanghai.aliyuncs.com/activity/SetWindow.mp4"></video>

## 概述

实现更改窗口显示状态。支持的窗口状态包括最大化、最小化、还原。

## 属性

### 基本

参见 [通用配置项](../../Appendix/CommonConfigurationItems.md)。

### 目标

- **控件元素**：接收变量作为点击的目标元素。此项和**选择器**二选一填入。
- **匹配超时（毫秒）**：限定查找目标元素时间，超出指定时间后将不再等待，1000ms = 1s。
- **[选择器](../../Appendix/Selector.md?_v=v2020.4)** ：用于指示要点击的目标位置。可通过点击**指定元素**自动生成。

### 可选项

- **窗口置顶**：选择运行时的桌面窗口是否置顶，部分界面窗口置顶时无法获取到窗口内的内容，这时需要将此属性设置为不置顶。
- **窗口状态**：选择欲实现的窗口状态，包括还原、最大化、最小化。

## 使用示例

**此流程执行逻辑**：指定固定窗口，实现其最小化。

![配置设置窗口组件](https://docimages.blob.core.chinacloudapi.cn/images/Activities/setwindowstate20210723.png)
