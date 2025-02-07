# 写入行/列数据

## 视频示例

<video controls height='100%' width='100%' src="https://encooacademy.oss-cn-shanghai.aliyuncs.com/activity/WriteRowOrColumnData.mp4"></video>

## 概述

横向或纵向写入数据到工作表中，支持自定义起始单元格地址执行写入。

## 属性

### 基本

参见 [通用配置项](../../Appendix/CommonConfigurationItems.md)。

### 输入

- **工作表** ：写入数据的目标工作表。若指定工作表不存在则自动新建。
- **起始单元格** ：写入数据的开始单元格地址。
- **数据** ：写入工作表内的数据，例如：new object []{"value1", "value2", "value3"} 向指定的行/列插入 3 个值 value1, value2, value3
- **写入方式** ：写入数据的模式选择（横向写入数据或纵向写入数据）。选择“横向写入数据”后，则取用户指定的起始单元格地址，开始横向写入数据；选择“纵向写入数据”后，则取用户指定的起始单元格地址，开始纵向写入数据。

## 使用示例

**前置必要组件**：[打开/新建](../OfficeExcel/OpenExcel.md)

**此流程执行逻辑**：读取 Excel 中“sheet1”工作表中“A1”行“A1”列的内容写入至“sheet2”工作表中的“A1”行“A1”列中。

- 写入行数据

![配置写入行数据组件](https://docimages.blob.core.chinacloudapi.cn/images/Activities/WriteRowOrColumn1.png)

- 写入列数据

![配置定稿列数据组件](https://docimages.blob.core.chinacloudapi.cn/images/Activities/WriteRowOrColumn2.png)

## 常见问题

1. **Q：使用“写入行/列数据”组件时，报错“[错误] 写入行/列数据失败，详细错误信息：类型不匹配。(Exception from HRESULT: 0x80020005(DISP_E_TYPEMISMATCH))”**

    **A：** 读取行数据是输出的格式默认是 `Object[]`，可转为 `string[]` 变量类型，具体可参见 [c#怎样将 object[] 转换为 string []](https://www.cnblogs.com/panjinzhao/p/10495794.html)。
