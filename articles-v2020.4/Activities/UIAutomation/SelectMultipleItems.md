# 选择多个项目

## 视频示例

<video controls height='100%' width='100%' src="https://encooacademy.oss-cn-shanghai.aliyuncs.com/activity/SelectMultipleItem.mp4"></video>

## 概述

实现多个项目的同时选择，此组件仅当原页面支持多选时生效。

## 属性

### 基本

参见 [通用配置项](../Appendix/CommonConfigurationItems.md)。

### 输入

- **项目文本** ：指要选择的多个项目文本。仅支持字符串变量和字符串

### 目标

- **控件元素** ：接收变量作为目标元素。属性**控件元素**和**选择器**二者必填其一且互斥。
- **[选择器](../Appendix/Selector.md?_v=v2020.4)** ：用于指示要下拉框目标元素。可通过点击**指定元素**自动生成。
- **匹配超时(毫秒)** ：限定查找目标元素时间，超出指定时间后将不再等待，1000ms = 1s。

### 可选项

- **窗口置顶**：选择运行时的桌面窗口是否置顶，部分界面窗口置顶时无法获取到窗口内的内容，这时需要将此属性设置为不置顶。
- **清空已选** ：勾选后，将先清空已选项目后执行勾选；不勾选时，将不清空已选项目直接执行勾选。

## 使用示例

**此流程执行逻辑**：指定网页端或桌面端有多个选项的元素，实现选择多个项目文本。

![配置选择多个项目组件](https://docimages.blob.core.chinacloudapi.cn/images/Activities/selectMultipleItems1.png)
