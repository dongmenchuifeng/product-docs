# 证照识别

## 视频示例

<video controls height='100%' width='100%' src="https://encooacademy.oss-cn-shanghai.aliyuncs.com/activity/LicenseRecognition.mp4"> </video>

## 概述

使用控制台账号登录编辑器（暂不支持私有化企业版），识别证照信息。

> **说明:**
>
> 若用户未配置相应服务账号，用户只可使用当日免费服务次数。若想继续使用该服务需前往云扩 [AI HUB](https://aihub.encoo.com/serviceAccount) 配置使用配额，具体参见 [AIHub 设置](../../AIHub/AIHubSetting.md)。

## 属性

### 基本

参见 [通用配置项](../Appendix/CommonConfigurationItems.md)。

### 输入

- **参数**：点击组件【设置参数】按钮，可配置如下参数：
    - 服务：可识别的证照的种类，目前支持身份证、行驶证、营业执照、银行卡、车牌、车辆合格证。
    - 平台：第三方 AI 平台，目前支持云扩 AI、阿里云、腾讯 AI 、百度 AI 、讯飞 AI 、华为云。
    - 图片文件：指定欲识别的图片路径，可接变量，建议使用常用的 jpg、jpeg 和 png 图片格式，如，"D:\\测试图片.jpg"。
    - 图片对象：指定欲识别的图片对象，与“图片文件”两者选一填写。
    - AIHub Key：预先在 [AIHub Key 授权管理](https://aihub.encoo.com/apikeyManager) 中设定的值，可以允许非云扩 Saas 用户（私有化部署 Saas 用户、许可证激活用户等）调用 AIHub 的 AI 服务。

### 输出

- **识别结果**：输出识别后的原始数据（JSON），仅支持变量。

## 使用示例

**此流程执行逻辑**：指定识别的图片、服务及平台，查看识别结果。

![配置证照识别组件](https://docimages.blob.core.chinacloudapi.cn/images/Activities/IdentificationOfCredentials20210805.png)
