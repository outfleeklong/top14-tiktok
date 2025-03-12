# 如何在 Racknerd VPS 上启用或禁用 IPv6 的方法详解

使用 IPv6 网络为现代应用带来了更多的便利和效率。如果你最近在 [Racknerd](https://bit.ly/Rack_Nerd) 购买了 VPS，却发现默认没有启用 IPv6，那么这篇指南将帮助你完成相关设置。

---

## 前言

最近购买了 Racknerd 的 512 MB KVM VPS，并注意到 IPv6 并未默认启用。不过，通过简单的一些配置，就可以顺利开启 IPv6 的支持。以下是具体的操作步骤：

---

## 开启 IPv6 的设置方法

### 1. 修改 sysctl.conf 文件
通过 SSH 登录至你的服务器后，编辑 `sysctl.conf` 文件。在文件末尾添加以下内容：

bash
net.ipv6.conf.all.autoconf = 0
net.ipv6.conf.all.accept_ra = 0
net.ipv6.conf.eth0.autoconf = 0
net.ipv6.conf.eth0.accept_ra = 0


然后执行以下命令来应用新配置：

bash
sysctl -p


### 2. 重启网络服务
使用以下命令重新启动网络服务：

bash
systemctl restart networking


重启后，可以通过 `ping6` 测试 IPv6 连接：

bash
ping6 google.com


### 3. 如果仍然无效
如果重启网络后 IPv6 仍然无法生效，可以尝试重启 VPS 后再次测试。

👉 [【建议收藏】2025年Racknerd最新优惠套餐整理汇总 - 每日更新可用活动优惠](https://bit.ly/Rack_Nerd)

---

## 验证和测试 IPv6

安装 Hysteria2 后，可以前往 [Test IPv6](https://test-ipv6.com/) 网站，查看你的 IPv6 使用情况。

还可以通过以下命令检查 VPS 的具体 IPv6 信息：

bash
curl ipv6.ip.sb


### 重新启用 IPv6 的方法
如果曾手动禁用过 IPv6，可以使用以下命令重新启用：

bash
sysctl -w net.ipv6.conf.all.disable_ipv6=0
sysctl -w net.ipv6.conf.default.disable_ipv6=0


最后，重新加载 sysctl 配置以确保更改生效：

bash
sysctl --system


至此，你的 IPv6 网络配置已完成设置。

---

## 总结

按照以上步骤配置后，你的 VPS 应该已经能够成功使用 IPv6 网络。如果在过程中遇到问题，建议仔细检查配置文件是否正确修改并确保用户权限足够，或者尝试重启 VPS 再次测试 IPv6。

通过开启 IPv6，为你的网络体验增添更多可能性！