## 大雕 QWRT 月经问题汇总备忘

---
**Q：为什么我刷了QWRT看不到那些奇怪的插件？**

A：在ssh输入以下命令，然后web界面就显示了
```bash
echo 0xDEADBEEF > /etc/config/google_fu_mode
```
---
**Q: 固件文件名中带**factory**固件和带**sysupgrade**固件分别用在什么地方？**

A：文件名中带**factory**固件一般是通过uboot web刷入；文件名中带**sysupgrade**固件一般是在QWRT系统内升级适用，有些uboot也可以使用**sysupgrade**刷机具体看机型。

---
**Q：我能自己安装缺失的kmod依赖包吗？**

A：一般情况下是不能的，kmod的包需要和内核匹配才行，开源固件一般可以通过自行编译加入需要的kmod，闭源需要大雕提供固件对应的kmod文件才能手动安装。

---
**Q：如何进入uboot（不死）web界面？**

A：路由器断电，用卡针灯按住reset 5-10s，通电开机，电脑配置IP192.168.1.10掩码255.255.255.0，访问http://192.168.1.1。
