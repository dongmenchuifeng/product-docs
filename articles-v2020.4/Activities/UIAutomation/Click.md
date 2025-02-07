# 点击

## 视频示例

<video controls height='100%' width='100%' src="https://encooacademy.oss-cn-shanghai.aliyuncs.com/activity/Click.mp4"></video>

## 概述

模拟鼠标的点击操作，支持桌面端和浏览器。同时支持桌面端图像识别指定元素。

## 属性

### 基本

参见[通用配置项](../Appendix/CommonConfigurationItems.md)。

### 目标

- **控件元素** ：接收变量作为点击的目标元素。此项和**选择器**二选一填入。
- **[选择器](../Appendix/Selector.md?_v=v2020.4)** ：用于指示要点击的目标位置。可通过点击**指定元素**自动生成。
- **匹配超时(毫秒)** ：限定查找目标元素时间，超出指定时间后将不再等待，1000ms = 1s。

### 点击

- **点击类型** ：下拉选择模拟鼠标点击的类型。
- **光标位置** ：从 **横坐标偏移** 和 **纵坐标偏移** 属性添加偏移量的光标的起点。
- **鼠标键** ：选择模拟鼠标点击的按键。
- **横坐标偏移** ：根据 **光标位置**字段中选择的选项，光标位置的水平位移像素量。例如填写“10”，则代表以**光标位置**为开始，向右偏移10个像素。计算坐标时，以屏幕左上角为原点。
- **纵坐标偏移** ：根据**光标位置**字段中选择的选项，光标位置的垂直位移像素量。例如填写“10”，则代表以**光标位置**为开始，向下偏移10个像素。计算坐标时，以屏幕左上角为原点。
- **横坐标百分比** ：根据**光标位置**进行百分比移动。以点击所指定矩形框的长度为基数，乘以此属性值，结果和**光标位置**的横坐标相加，得到最终的点击横坐标。
例如填写"0.5",光标位置选择"中心"，最终点击位置的计算过程：取指定元素的矩形框长度，乘以0.5，结果为矩形框长度的一半；后和光标位置"中心"执行相加计算，最终得到的数字为点击的横坐标，即为矩形框的右边框中心处。
- **纵坐标百分比** ：根据**光标位置**进行百分比移动。以点击所指定矩形框的宽度为基数，乘以此属性值，结果和 **光标位置**的纵坐标相加，得到最终的点击纵坐标。
例如填写"0.5",光标位置选择"中心"，最终点击位置的计算过程：取指定元素的矩形框宽度，乘以0.5，结果为矩形框宽度的一半；后和光标位置"中心"执行相加计算，最终得到的数字为点击的纵坐标，即为矩形框的下边框中心处。

### 可选项

- **窗口置顶**：选择运行时的桌面窗口是否置顶，部分界面窗口置顶时无法获取到窗口内的内容，这时需要将此属性设置为不置顶。
- **点击方式** ：选择模拟鼠标点击时使用何种方法。此属性默认值为**默认**，实现的是根据用户指定元素的类型(即桌面端或浏览器)，自动适用最佳的点击方式。
当有部分场景使用默认属性值无法成功执行时，可手动修改此属性值为**模拟鼠标**或**设置控件**，以适应少数特殊场景使其成功执行。

    >**说明：**
    >
    >- 当指定一个桌面元素时。**点击方式**属性选择“设置控件”后，仅支持**左键单击**。不支持**光标位置、横(纵)坐标偏移、横(纵)坐标百分比**的设置。
    > - 当指定一个浏览器元素时。**点击方式**属性选择“设置控件”后，仅支持所选择元素所支持的JS事件；当有场景无法覆盖时，可更改属性值为**模拟鼠标**。

- **辅助键** ：实现在点击时同时按下辅助键的效果。仅当点击方式为模拟鼠标时生效，设置控件不生效。

## 使用示例

**此流程执行逻辑**：使用**点击**组件，并指定元素后，打开选择器窗口，点击“未验证”按钮，验证是否识别指定元素。

![属性配置](https://docimages.blob.core.chinacloudapi.cn/images/Activities/check-2.png)

**执行结果**：
![执行结果](https://docimages.blob.core.chinacloudapi.cn/images/Activities/check-3.png)

>更多花式点击，请点击[链接](https://academy.encoo.com/learn/unit-detail/33) 查看云扩学院高级课程。
