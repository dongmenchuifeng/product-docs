# 状态

## 视频示例

<video controls height='100%' width='100%' src="https://encooacademy.oss-cn-shanghai.aliyuncs.com/activity/State.mp4"></video>

## 概述

**状态** 组件是状态机中使用的组件，是状态机工作流的基础组成部分。

> **说明：**
>“状态”组件必须放置在“状态机”组件中。

“状态”组件包括三个可编辑区域：
- Entry 区域：包含在 Entry 区域的组件会在工作流进入该 *状态* 组件时被执行；
- Exit 区域：包含在 Exit 区域的组件会在工作流离开该 *状态* 组件时被执行；
- Transition 区域：通过设定 Transition 中的内容，你可以实现多个状态之间的转换。

## 属性

### 基本

参见 [通用配置项](../../Appendix/CommonConfigurationItems.md)。

## 使用示例

一般与 **状态机** 组件搭配使用，操作样例可参见 [状态机](activity/../StateMachine.md)。
