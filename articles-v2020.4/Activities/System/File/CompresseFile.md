# 压缩文件/文件夹

## 视频示例

<video controls height='100%' width='100%' src="https://encooacademy.oss-cn-shanghai.aliyuncs.com/activity/CompressFileOrFolder.mp4"> </video>

## 概述

该组件实现对指定的文件/文件夹压缩成 ZIP 文件。

## 属性

### 基本

参见 [通用配置项](../../Appendix/CommonConfigurationItems.md)。

### 输入

- **列表模式**：选择需要压缩的类型，支持文件和文件夹类型。
- **路径列表**：需要压缩的文件/文件夹路径，支持相对路径和绝对路径。
- **压缩文件路径**：压缩后的文件/文件夹需保存的路径，文件名需以 zip 结尾。

### 可选项

- **密码**：输入压缩密码，可接变量。可与 **设置密码** 组件配合使用。
- **同名替换**：有同名文件是否替换。

## 使用示例

**此流程执行逻辑**：将桌面上的 `test.xlsx` 文件压缩成 `test.zip` 文件保存至桌面上。
  
![配置压缩文件属性](https://docimages.blob.core.chinacloudapi.cn/images/Activities/compressefile20210224.png)

**执行结果**：

![运行结果](https://docimages.blob.core.chinacloudapi.cn/images/Activities/compressfileresult20210224.png)

## 常见问题

1. **Q：压缩文件/文件夹组件的【路径列表】属性，使用变量时怎么设置值？**

    **A：**【路径列表】的数据类型是 List，变量值设置格式为 new List <string>(){"路径 1", "路径 2", "路径 3"}，其中的路径 1、路径 2 和路径 3 为你需要压缩的具体文件/文件夹路径。
