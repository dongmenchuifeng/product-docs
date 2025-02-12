# 输入文本

## 视频示例

<video controls height='100%' width='100%' src="https://encooacademy.oss-cn-shanghai.aliyuncs.com/activity/InputText.mp4"> </video>

## 概述

模拟输入文本的操作，输入文本到指定位置，支持桌面端和浏览器。同时支持桌面端图像识别指定元素，浏览器端暂不支持

## 属性

### 基本

参见 [通用配置项](../Appendix/CommonConfigurationItems.md)。

### 可选项

- **窗口置顶**：选择运行时的桌面窗口是否置顶，部分界面窗口置顶时无法获取到窗口内的内容，这时需要将此属性设置为不置顶。
- **清空原文本** ：输入文本前先清空指定元素的原数据。仅当输入方式为设置控件时生效。
- **输入方式** ：选择输入文本时使用何种方法。此属性默认值为 **默认**，实现的是根据用户指定元素的类型(即桌面端或浏览器)，自动适用最佳的输入方式。
当有部分场景使用默认属性值无法成功执行时，可手动修改此属性值为 **模拟键盘** 或 **设置控件**，以适应少数特殊场景使其成功执行。
- **输入前行为**：选择在输入文本之前的操作行为，如，设置焦点、点击。

### 目标

- **控件元素** ：接收变量作为输入文本的目标元素。属性 **控件元素** 和 **选择器** 二者互斥
- **[选择器](../Appendix/Selector.md?_v=v2020.4)** ：用于指示要输入文本的目标元素。可通过点击 **指定元素** 自动生成。仅支持字符串变量和字符串
- **匹配超时(毫秒)** ：限定查找目标元素时间，超出指定时间后将不再等待。若超过此时间还未匹配到指定元素则会抛出错误。1000ms = 1s。

### 输入

- **文本** ：输入到选择器元素的内容。文本内容所见即所得，不支持转义。支持字符串变量和字符串

## 使用示例

**此流程执行逻辑**：使用 **输入文本** 组件，并指定元素后，检查元素是否识别成功，将在识别的该元素中输入指定的文本内容。

![输入文本配置](https://docimages.blob.core.chinacloudapi.cn/images/Activities/setTex-1.png)

**执行结果**：

![执行结果](https://docimages.blob.core.chinacloudapi.cn/images/Activities/setTex-2.png)

## 常见问题

1. **Q：使用“输入文本”组件，如何输入“年/月/日”这种日期格式？**

    ![日期格式](https://docimages.blob.core.chinacloudapi.cn/images/Activities/dateformat20210825.png)

    **A：** 在“输入文本”组件的“文本”属性框中输入，如 `"2000-01-01"`。

    ![输入文本日期](https://docimages.blob.core.chinacloudapi.cn/images/Activities/inputtext20210825.png)
