# 截屏

## 视频示例

<video controls height='100%' width='100%' src="https://encooacademy.oss-cn-shanghai.aliyuncs.com/activity/Screenshot.mp4"></video>

## 概述

实现截图，并将结果保存在指定位置或变量中。

## 属性

### 基本

参见 [通用配置项](../Appendix/CommonConfigurationItems.md)。

### 保存

- **路径**：截屏图片的保存位置。

    > **说明**：
    >
    >- 此项可为空，当不填写时，默认不保存截屏。
    >- 支持相对路径和绝对路径，路径需指明文件名和后缀；支持的后缀为：PNG, BMP, JPEG, JPG。如，`E:\Screenshot.jpg`。

- **同名覆盖** ：当按照上述 **路径** 保存截屏，且出现同名文件时，如果此项勾选则不报错，执行替换保存操作；如果此项未勾选，则报错运行失败。

### 输出

- **图片**：将截屏保存到此变量，此项可为空。

### 目标

- **控件元素** ：接收变量作为点击的目标元素。此项和 **选择器** 二选一填入。
- **[选择器](../Appendix/Selector.md)** ：用于指示要点击的目标位置。可通过点击 **指定元素** 自动生成。
- **匹配超时(毫秒)** ：限定查找目标元素时间，超出指定时间后将不再等待，1000ms = 1s。

### 可选项

- **窗口置顶**：选择运行时的桌面窗口是否置顶，部分界面窗口置顶时无法获取到窗口内的内容，这时需要将此属性设置为不置顶。
- **图片宽度** ：截屏所得图片的长度。此项可为空。仅支持整型变量和整型
- **图片高度** ：截屏所得图片的宽度。此项可为空。仅支持整型变量和整型
- **横坐标偏移** ：根据指定元素所得的图片位置，进行水平位移像素量。例如填写“10”，则代表向右偏移 10 个像素。计算坐标时，以指定元素所得图片的左上角为原点。仅支持整型变量和整型
- **纵坐标偏移** ：根据指定元素所得的图片位置，光标位置的垂直位移像素量。例如填写“10”，则代表向下偏移 10 个像素。计算坐标时，以指定元素所得图片的左上角为原点。仅支持整型变量和整型
- **横坐标百分比** ：根据指定元素所得的图片位置进行百分比移动。以指定元素所得的图片长度为基数，乘以此属性值，结果和原图的横坐标相加，得到最终的点击横坐标。
例如填写 "0.5", 最终截屏位置的计算过程：取指定元素的矩形框长度，乘以 0.5，结果为矩形框长度的一半；将指定元素的矩形框长度和计算所得长度相加，最终得到的数字为截屏开始的横坐标，即为矩形框长的中心处
- **纵坐标百分比** ：根据指定元素所得的图片位置进行百分比移动。以指定元素所得的图片宽度为基数，乘以此属性值，结果和原图的纵坐标相加，得到最终的点击纵坐标。
例如填写 "0.5", 最终点击位置的计算过程：取指定元素的矩形框宽度，乘以 0.5，结果为矩形框宽度的一半；将指定元素的矩形框宽度和计算所得宽度相加，最终得到的数字为截屏开始的纵坐标，即为矩形框宽的中心处

> **说明：**
>
> 上述可选项属性均可不填，仅当需要进行偏移进行截屏时才需要填写。并且，在计算偏移时均以指定元素作为基准来计算。

## 使用示例

**此流程执行逻辑**：指定需要截屏的图片，实现自动截屏。

![配置截屏组件](https://docimages.blob.core.chinacloudapi.cn/images/Activities/screenShot2.png)

## 常见问题

1. **Q：使用截屏组件报错“[错误]截屏失败。详细错误信息：图像格式不支持”**。

    ![截屏报错](https://docimages.blob.core.chinacloudapi.cn/images/Activities/screenshots20210825.png)

    **A：** 验证码路径应当是文件路径，图中填写的为文件夹。

    ![文件路径](https://docimages.blob.core.chinacloudapi.cn/images/Activities/filepath20210825.png)
