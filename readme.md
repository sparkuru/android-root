# android-root

Android devices root record

1. [root record](./root-record.md)
2. [mi-rom-flash](./mi-rom-flash.sh)
3. [flash-LineageOS-record](./flash-LineageOS-record.md)

## tool

1.   adb 调试工具，[SDK Platform-Tools](https://developer.android.com/tools/releases/platform-tools?hl=zh-cn)，解压备用（文件路径不能含有中文名）
2.   miui 解锁工具，[链接](https://www.miui.com/unlock/index.html)
3.   miui rom 下载，[xiaomirom](https://xiaomirom.com/series/)
4.   magisk 下载，[topjohnwu/Magisk](https://github.com/topjohnwu/Magisk)
5.   ~~magisk-delta 下载，[HuskyDG/magisk-files](https://github.com/HuskyDG/magisk-files/releases)~~

## magisk-support

1.   下载各类模块 MRepo，[MRepoApp/MRepo](https://github.com/MRepoApp/MRepo)
2.   提供更好的 root 授权服务，Shamiko，[Shamiko releases](https://github.com/LSPosed/LSPosed.github.io/releases)
3.   用于测试当前 root 环境，momo，[地址](https://t.me/s/magiskalpha/517)
4.   用于测试设备环境下的 apk 列表，ApplistDetector，[Dr-TSNG/ApplistDetector](https://github.com/Dr-TSNG/ApplistDetector.git)
5.   用于魔改系统行为，LSPosed，[LSPosed/LSPosed](https://github.com/LSPosed/LSPosed.git)
     1.   KTweak，[tytydraco/KTweak-Android-App](https://github.com/tytydraco/KTweak-Android-App.git)，优化手机省电
     2.   哔哩哔哩，[yujincheng08/BiliRoaming](https://github.com/yujincheng08/BiliRoaming.git)，软件优化
     3.   Telegram，[Sakion-Team/Re-Telegram](https://github.com/Sakion-Team/Re-Telegram.git)，软件优化
     4.   qq，[cinit/QAuxiliary](https://github.com/cinit/QAuxiliary.git)，软件优化
     5.   菜鸟，[duzhaokun123/FuckCainiao](https://github.com/duzhaokun123/FuckCainiao.git)，软件优化
     6.   知乎，[shatyuka/Zhiliao](https://github.com/shatyuka/Zhiliao.git)，软件优化
     7.   ChiMi，[yonghen/chimi-](https://github.com/yonghen/chimi-)，MIUI 13 界面定制信息等优化
     8.   Disable Flag Secure，[LSPosed/DisableFlagSecure](https://github.com/LSPosed/DisableFlagSecure.git)，解除安卓安全限制（可以强制截屏）
     9.   Fuck Shake，[pwh-pwh/fuck_shake](https://github.com/pwh-pwh/fuck_shake.git)，屏蔽摇一摇广告
     10.   TwiFucker，[Dr-TSNG/TwiFucker](https://github.com/Dr-TSNG/TwiFucker.git)，软件优化
     11.   Hide My Applist，[Dr-TSNG/Hide-My-Applist](https://github.com/Dr-TSNG/Hide-My-Applist.git)，应用喜欢侵犯隐私
     12.   PlayIntegrityFix，[chiteroman/PlayIntegrityFix](https://github.com/chiteroman/PlayIntegrityFix.git)，谷歌 play 完整性校验 1 绕过
     13.   safetynet-filx，[kdrag0n/safetynet-fix](https://github.com/kdrag0n/safetynet-fix.git)，谷歌 play 完整性校验 2 绕过
     14.   Thanox，[Tornaco/Thanox](https://github.com/Tornaco/Thanox)，十分好用的安卓权限、隐私配置软件，需要付费（`20RMB / 设备 / 永久` 或 `$5 / 不限设备 / 永久`）
     15.   LuckyTool，[Xposed-Modules-Repo/com.luckyzyx.luckytool](https://github.com/Xposed-Modules-Repo/com.luckyzyx.luckytool.git)，ColorOS 相关优化
6.   其他可选 magisk 模块，[参考](https://magisk.suchenqaq.club/query.php?file_type=magisk&is_classification_list=true)

     1.   自动神仙救砖-支持OTA稳定Lite白名单版v3
     2.   去广告
     3.   音量键救砖

```bash
$ ls *.zip *.apk
A-Automatic_brick_rescue.zip                                B-gkd-v1.11.6.apk
A-LSPosed-v1.9.2-7024-zygisk-release.zip                    B-HMA-V3.5.apk
A-safetynet-fix-v2.4.0.zip                                  B-LuckyTool_v1.3.2.20457.apk
A-Shamiko-v1.2.5-414-release.zip                            B-Re-Telegram-v18.0-Release.apk
A-zygisk-module-xfingerprint-pay-wechat-v6.0.2-release.zip  B-TwiFucker-V2.1.apk
B-ApplistDetector.V2.4.apk                                  B-Zhiliao_24.04.06.apk
B-BiliRoaming_1.7.0.apk                                     R-cx-file-explorer.apk
B-disableflagsecure.apk                                     R-Magisk-v30.6.apk
B-FuckCainiao_release_v0.1.1.apk                            R-MRepo-2.5.0.a27eaf7-921-release.apk
B-fuck-shake.apk                                            R-shizuku-v13.6.0.r1086.2650830c-release.apk
```

## reference

1.   [刷了 Magisk 之后装什么？我推荐这 20+ 个模块](https://sspai.com/post/68531)
2.   [2023 年 Magisk 推薦安裝的模組，提升手機效能、擋廣告、自定義主題](https://ivonblog.com/posts/magisk-recommended-modules/)
3.   [一加手机官方 ROM 下载](https://yun.daxiaamu.com/OnePlus_Roms/)
4.   [一加手机 magisk 模块下载](https://yun.daxiaamu.com/files/magisk%E6%A8%A1%E5%9D%97/)
5.   [小米 rom 下载](https://xiaomirom.com/series/)
