# 获取邮件(Exchange)

## 视频示例

<video controls height='100%' width='100%' src="https://encooacademy.oss-cn-shanghai.aliyuncs.com/activity/GetExchangeMail.mp4"></video>

## 概述

获取 Exchange 服务账号中的邮件。

## 属性

### 服务器

- **Exchange 版本** ：选择 Exchange 版本。
- **服务器** ：输入收件人邮箱所属服务器地址。如，“<https://×××.outlook.cn>”。

### 基本

参见 [通用配置项](../../Appendix/CommonConfigurationItems.md)。

### 输出

- **邮件** ：将获取到的邮件存储在此变量，变量类型为 List <System.Net.Mail.MailMessage>;

### 邮件

- **共享账号** ：指定共享邮箱账号地址。
- **获取封数** ：获取邮件的封数。默认为 1
- **密码** ：输入收件人邮箱密码。
- **邮件文件夹** ：指定获取邮件的文件夹。获取收件箱下邮件需填写英文 "inbox"; 若获取 inbox 下子级文件夹邮件，需使用 "/" 分隔，例如: "inbox/客户邮件"
- **邮箱地址** ：输入收件人邮箱地址。
- **域名** ：输入域名；若为空则使用默认域名。

### 可选项

- **标记为已读** ：指定检测加密方法，默认为自动。
- **超时**：指定此组件的执行时间。若超出此时间，组件还未执行，会抛出错误。
- **获取附件** ：选择是否获取附件，默认为勾选即不获取附件。 勾选后则在获取邮件时同时获取附件。
- **仅获取未读邮件** ：默认获取所有类型邮件。若勾选，则仅获取未读邮件。

## 使用示例

**此流程执行逻辑**：获取 Exchange 服务账号中“收件箱”中的邮件。

![配置获取 Exchange 邮件组件](https://docimages.blob.core.chinacloudapi.cn/images/Activities/GetMailExchange2020122302.png)
