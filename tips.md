# tips

> 将手机上的 app 导出方法

首先确定要导出的 app 包名，这里以拼多多为例：在 `adb shell pm list packages | grep duoduo` 可以看到包名称为 `com.xunmeng.pinduoduo`，通过 `pm path` 找到包具体路径信息，然后 pull 即可

```bash
$ adb shell pm list packages | grep pin
package:com.xunmeng.pinduoduo
package:com.hpbr.bosszhipin

$ adb shell pm path com.xunmeng.pinduoduo
package:/data/app/~~3vIZREgua2WwO6TKe7fj7A==/com.xunmeng.pinduoduo-isuccz5pAU-MgkpF0nqtcw==/base.apk

$ adb pull /data/app/~~3vIZREgua2WwO6TKe7fj7A==/com.xunmeng.pinduoduo-isuccz5pAU-MgkpF0nqtcw==/base.apk ./pinduoduo.apk
/data/app/~~3vIZREgua2WwO6TKe7fj7A==/com.xunmeng.pinduoduo...le pulled, 0 skipped. 37.8 MB/s (28709344 bytes in 0.724s)
```