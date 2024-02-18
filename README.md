# 大雕 QWRT 月经问题汇总备忘

---
Q：为什么我刷了QWRT看不到那些奇怪的插件？

A：在ssh输入以下命令，然后web界面就显示了
```bash
echo 0xDEADBEEF > /etc/config/google_fu_mode
```
---
