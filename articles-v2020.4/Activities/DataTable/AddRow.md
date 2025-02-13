# 添加数据行

## 视频示例

<video controls height='100%' width='100%' src="https://encooacademy.oss-cn-shanghai.aliyuncs.com/activity/AddDataRow.mp4"></video>

## 概述

向数据表中添加一行数据，并自动保存同步至指定数据表。

## 属性

### 基本

参见 [通用配置项](../Appendix/CommonConfigurationItems.md)。

### 输入

- **数据表** ：将数据行添加到此表。
- **数组** ：添加到数据表的数组。数组内的数据类型应和数据表中对应列的类型一致。和“数据表行”属性两者互斥，只能且必需填入一项。
- **数据表行** ：添加到数据表的数据表行对象。和“数组”属性两者互斥，只能且必需填入一项。

## 使用示例

**前置必要条件**：已有一个已搭建的数据表，可参见 [搭建数据表](../DataTable/BuildDataTable.md)。

**此流程执行逻辑**：将已搭建的数据表 `table` 中添加一行数据 `"David","50","男"`。

![配置添加数据行组件](https://docimages.blob.core.chinacloudapi.cn/images/Activities/AddRow20201228.png)
