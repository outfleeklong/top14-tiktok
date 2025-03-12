# RackNerd双十一优惠与VPS特性详解：促销、流量翻倍、迁移和邮箱管理

RackNerd提供的促销特价VPS迎来了双十一优惠活动，购买后流量还可翻倍。以下是相关的操作指南及信息汇总，帮助用户更好地管理其服务。

---

## 开通VPS后的账号密码管理

VPS开通后，可通过邮件记录快速获取 root 密码以及控制面板的账户名和密码：

1. 登录 RackNerd 用户中心，访问邮件记录页面：  
👉 [邮件记录查看地址](https://my.racknerd.com/clientarea.php?action=emails)

2. 在邮件列表中找到主题为 `KVM VPS Login Information` 的邮件，所需的登录信息均包含在邮件中。

---

## 如何将流量翻倍？

购买 RackNerd VPS 后，用户可以尝试以下方法为其服务流量翻倍：

### 方法1：在论坛回帖申请
在知名论坛 LET (LowEndTalk) 的指定贴文下发表评论，可有效申请到流量翻倍。新购的 VPS 使用此方法成功率较高。

- 访问 LET 的贴文地址：[点此访问相关论坛贴](https://lowendtalk.com/discussion/182232/story-time-one-one-dot-one-one-nvm-just-check-this-out#latest)
- 评论模板如下：
  
  Hello, I would like to double the bandwidth.
  Order Number: 邮件记录中获取
  Invoice ID: 邮件记录中获取
  Thanks!
  
- 如何获取相关信息：  
  - **Order Number** 和 **Invoice ID** 可从上述邮件记录页面找到。

注：若没有 LET 账号，可注册并遵守论坛规定。注册时需要提供简短的英文理由，如“学习 VPS 相关知识”。通过邮箱验证后即可使用账号。

### 方法2：发工单申请
部分用户通过提交工单申请流量翻倍，成功率不稳定，具体取决于工单内容和售后处理态度。

---

👉 [【建议收藏】2025年Racknerd最新优惠套餐整理汇总 - 每日更新可用活动优惠](https://bit.ly/Rack_Nerd)

---

## 机房选择与迁移

### 机房介绍
RackNerd目前主要使用两类数据中心：
1. **CC机房 (ColoCrossing)**：包括圣何塞、西雅图、新泽西、芝加哥等多地。这些机房的IP曾经会触发 Google 验证，但现状有所改善。
2. **MC机房 (Multacom Corporation)**：仅洛杉矶 DC2 机房属于此类别，虽然网络质量在晚高峰表现略差，但其 IP 不会触发 Google 验证，支持 IPv6（需发工单申请）。

用户可根据需要选择机房，通常推荐洛杉矶或圣荷塞，但具体取决于使用体验。

#### 网络测试地址
以下是部分机房的测速地址：
- 洛杉矶 DC02 IP：204.13.154.3  
测速文件：[点此测速](http://lg-lax02.racknerd.com/1000MB.test)
- 西雅图 IP：192.3.253.2  
测速文件：[点此测速](http://lg-sea.racknerd.com/1000MB.test)
- 新泽西 IP：192.3.165.30  
测速文件：[点此测速](http://lg-nj.racknerd.com/1000MB.test)
- 亚特兰大 IP：107.173.164.160  
测速文件：[点此测速](http://lg-atl.racknerd.com/1000MB.test)

### 机房迁移
购买支持多机房选择的套餐可免费迁移；若为固定机房，迁移可能需支付额外费用（一般为5美元）。迁移时需要注意以下几点：
1. 迁移后 IP 会改变，数据可能丢失。因此迁移前务必做好备份。
2. 翻倍的流量可能恢复为默认值，可尝试通过工单申请重新调整。

此外，迁往洛杉矶 DC2 的用户若需 IPv6，可发工单申请。

---

## 邮箱修改与 push 操作说明

### 邮箱更改
虽然更改账户邮箱需支付费用以减少黄牛转售，但目前可通过提交工单进行免费修改。

### Push 账户转移
RackNerd 支持 Push（账户内服务转移），每次操作需支付 8 美元，无论转移 VPS 的数量。若需将 VPS 转移至其他账户即可通过工单提交申请。

---