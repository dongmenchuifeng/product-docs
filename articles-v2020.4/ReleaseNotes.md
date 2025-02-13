# 云扩 RPA 产品发版说明

本文介绍了云扩产品的的功能发布和对应的文档动态，欢迎体验。

> **提示：**
>
> 关于社区版与企业版的差异说明，请参见 [常见问题](./FAQ/QA.md)。


## 2022.05.27 发版说明

2022.05.27 发布了云扩 RPA , 本次发布的产品及版本号为：

|         | 版本号      |
| -----:  | -----:     |
| 控制台   |V 4.1.76096|


### 【控制台】

1. [流程编排](./Console/rpa-center/flowSequence/aboutFlowSequence.md)，可自动执行多个流程部署，支持顺序调整和定时开始
2. SaaS控制台社区版开放vicode V2版
3. [流程状态](./Console/rpa-center/job/manageJob.md)优化，同时状态文案处增加tooltip效果，以及仪表盘状态统计同步
4. [流程包管理](./Console/rpa-center/packages/aboutPackages.md)，主列表新增下载入口，默认下载最新版本
5. [机器人管理](./Console/rpa-center/robot/manageRobot.md)，创建机器人时，关闭弹框，老用户可在详情页面获取连接字符串
6. [定时任务](./Console/rpa-center/workflow/trigger.md)，Cron表达式限制不低于10分钟
7. 数据队列，支持批量删除
8. 任务队列，交互优化，插入不合法的消息时，提示用户

## 2022.04.10 发版说明

2022.04.10 发布了云扩 RPA , 本次发布的产品及版本号为：

|         | 版本号      |
| -----:  | -----:     |
| 编辑器   |1.1.2204.9|
| 机器人   |1.1.2204.9|
| 控制台   |V 4.1.73689|

### 【编辑器】

1. 支持发布最高 2GB 的大流程文件至控制台

### 【组件】

1. 新增 [屏保运行](./Activities/System/Screen/screensaver.md) 组件，支持流程在设置的屏保后运行
2. 新增 [加入任务](./Activities/Console/task-queue/AddtoTaskQueue.md) 组件，实现向任务队列中添加消息
3. 新增 [消费任务](./Activities/Console/task-queue/OperateQueue.md) 组件，实现消费任务队列中的消息
4. 原 WPS 类组件合并至 OfficeExcel 类组件中
5. 支持未安装 Excel 和 WPS 时也可使用部分 Excel 组件
6. 将 删除数据 组件拆分为 [清除单元格](./Activities/AppAutomation/OfficeExcel/clear-cell.md)、[清除区域](./Activities/AppAutomation/OfficeExcel/clear-area.md)、[清除行](./Activities/AppAutomation/OfficeExcel/clear-row.md)、[清除列](./Activities/AppAutomation/OfficeExcel/clear-row.md) 四个组件

### 【机器人】

1. 扩展，增加描述、详情入口，降低用户使用门槛
2. 支持在控制台查看运行中的实时日志
3. 定时任务，增加版本号，增强产品可读性
4. 产品更新，增加发版说明文档入口，优化交互体验

### 【控制台】

1. [定时任务](./Console/rpa-center/workflow/trigger.md)，支持时区、指定一个时间、动态提示
2. 审计日志，支持“操作模块”过滤
3. 文件服务，支持列表排序和分页
4. [流程包](./Console/rpa-center/packages/aboutPackages.md)，支持批量上传，最大 2G 的文件

## 2022.02.25 发版说明

2022.02.25 发布了云扩 RPA , 本次发布的产品及版本号为：

|         | 版本号      |
| -----:  | -----:     |
| 控制台   | V 4.1.71227|

### 改进与增强

#### 【控制台】

1. 支持控制台列表界面显示每页数据量、总计数据量, 便于用户快速统计
2. 支持数据队列按部门管理
3. 优化执行记录列表中的启动方式来源，支持任务队列
4. 支持在执行记录的任务详情页中显示等待状态的资源，便于用户快速定位
5. 优化资产加密方式

## 2022.01.27 发版说明

2022.01.27 发布了云扩 RPA , 本次发布的产品及版本号为：

|         | 版本号      |
| -----:  | -----:     |
| 编辑器   | 1.1.2201.3 |
| 机器人   | 1.1.2201.3 |
| 控制台   | V 4.1.70206|
| ViCode   | - |

### 新增功能

#### 【编辑器】

1. 支持第三方企业微信登录
2. 支持在变量/参数面板中复制和粘贴变量/参数
3. 升级 `.net` 至 4.6.2

#### 【机器人】

1. 升级 `.net` 至 4.6.2

#### 【控制台】

1. 用户头像支持自定义
2. 注册社区版控制台时，“公司”字段支持重名
3. 支持在流程包的“版本信息”选项页中，查看当前流程是否以管理员运行
4. 支持单击“机器人管理”列表中的“计算机”，查看该计算机的基本信息
5. "RPA 中心 > 设备管理" 菜单改名为“RPA 中心 > [计算机管理](./Console/rpa-center/device-management/device-management.md)”

#### 【ViCode】

1. 新建”应用“时，支持上传本地图标
2. 支持阿里云 OSS、腾讯云 COS 类的文件类连接器
3. 支持 Ctrl+鼠标选择的形式多选动作流，以帮助快速拖动或删除动作流
4. 支持在”连接管理“列表页面筛选连接类型
5. 在“数据模型”中，支持 SQL 批量更新

### 改进与增强

#### 【编辑器】

1. 优化加载市场列表的性能
2. 优化项目中流程文件名称的显示长度
3. 优化编辑器启动和打开时的性能
4. 优化当打开控制台流程库中流程时再次发布到控制台时默认发布至该项目所在的部门
5. 优化单独运行子流程时在“输出面板”中的日志显示形式
6. 优化在“输出面板”中复制日志时提示框样式
7. 优化编辑器最大化时的整体尺寸样式
8. 优化发布项目时默认选择组织架构的根目录部门

#### 【控制台】

1. 优化个人信息账户体系，支持通过已绑定的手机号登录
2. 优化手机短信验证码模板，支持验证码有效期为 10 分钟
3. 优化企业微信扫描登录时的用户界面
4. 优化私有化控制台的账密安全性问题
5. 优化下载流程包到本地时流程包的显示名称
6. 优化流程包管理的搜索功能，支持按流程包名称、创建人、标签字段模糊搜索
7. 优化日志详情中日志展示样式
8. 优化流程部署名称的长度
9. 优化“RPA 中心 > 执行记录”页，支持在执行记录列表中过虑“任务来源”字段
10. 优化“RPA 中心”的部分页面，支持勾选多选框时在“批量操作”按钮中显示选中的数量

#### 【ViCode】

1. 优化”输入类组件“的”标题“属性默认填充并展示
2. 优化模拟编辑区域为横向方向时的布局样式
3. 优化分享”我的应用“功能，支持以短链接的形式分享
4. 优化动作流组件中的块相关的组件，不支持调换顺序
