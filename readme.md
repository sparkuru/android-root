# android-root

android device root record

1. [root record](./root-record.md)
2. [mi-rom-flash](./mi-rom-flash.sh)
3. [flash-LineageOS-record](./flash-LineageOS-record.md)

## tool

1.   adb 调试工具，[SDK Platform-Tools](https://developer.android.com/tools/releases/platform-tools?hl=zh-cn)，解压备用（文件路径不能含有中文名）
2.   miui 解锁工具，[链接](https://www.miui.com/unlock/index.html)
3.   miui rom 下载，[xiaomirom](https://xiaomirom.com/series/)
4.   magisk 下载，[topjohnwu/Magisk](https://github.com/topjohnwu/Magisk)
5.   ~~magisk-delta 下载，[HuskyDG/magisk-files](https://github.com/HuskyDG/magisk-files/releases)~~

## 模块与工具

### Magisk 内启用

| 模块名称 | 地址 | 备注 |
| --- | --- | --- |
| Shamiko | [Shamiko releases](https://github.com/LSPosed/LSPosed.github.io/releases) | 提供更好的 root 授权服务 |
| Zygisk - LSPosed | [LSPosed/LSPosed](https://github.com/LSPosed/LSPosed.git) | ART hooking framework；下面大多数模块都要基于这个框架（或者类似物）实现，适配 libxposed 100 之前版本；意味着更新的模块无法使用，推荐用 Vector |
| Vector | [JingMatrix/Vector](https://github.com/JingMatrix/Vector.git) | 推荐使用，适配 libxposed 100 以前及之后的版本，LSPosed 是其 upstream |
| PlayIntegrityFix | [KOWX712/PlayIntegrityFix](https://github.com/KOWX712/PlayIntegrityFix.git) | （旧版 android，已失效）谷歌 Play 完整性校验绕过（方案 1）；另推荐检查工具 simple play integrity checker（spic） |
| safetynet-fix | [kdrag0n/safetynet-fix](https://github.com/kdrag0n/safetynet-fix.git) | （旧版 android，已失效）谷歌 Play 完整性校验绕过（方案 2） |
| Play Integrity Fix [INJECT] | [KOWX712/PlayIntegrityFix](https://github.com/KOWX712/PlayIntegrityFix.git) | 谷歌 Play 完整性校验绕过（方案 3） |
| KTweak | [tytydraco/KTweak-Android-App](https://github.com/tytydraco/KTweak-Android-App.git) | 优化手机省电 |
| FingerprintPay | [eritpchy/FingerprintPay](https://github.com/eritpchy/FingerprintPay.git) | 模拟实现指纹支付功能：微信、QQ、支付宝、淘宝、云闪付 |
| 爱玩机工具箱 | [release](https://aiwanji.xiake.pro/) | 提供更好地系统信息查看、配置修改、应用安装管理器；免费版足够用 |
| 救急模块 | [参考](https://magisk.suchenqaq.club/query.php?file_type=magisk&is_classification_list=true) | 自动神仙救砖-支持 OTA 稳定 Lite 白名单版 v3、去广告、音量键救砖 |

### 管理与检测

| 工具名称        | 地址                                                         | 备注                      |
| --------------- | ------------------------------------------------------------ | ------------------------- |
| MRepo           | [MRepoApp/MRepo](https://github.com/MRepoApp/MRepo)          | 下载及管理各类模块        |
| momo            | [地址](https://t.me/s/magiskalpha/517)                       | 测试当前 root 环境        |
| ApplistDetector | [Dr-TSNG/ApplistDetector](https://github.com/Dr-TSNG/ApplistDetector.git) | 测试设备环境下的 apk 列表 |

### 支持 Shizuku

| 工具名称 | 地址 | 备注 |
| --- | --- | --- |
| Shizuku | [RikkaApps/Shizuku](https://github.com/RikkaApps/Shizuku) | 为普通应用提供 ADB 或 root 权限调用能力 |
| gkd | [gkd-kit/gkd](https://github.com/gkd-kit/gkd.git) | 李跳跳 |

### LSPosed / Vector 模块

- **LSPosed**：适配 libxposed 100 之前；[LSPosed/LSPosed](https://github.com/LSPosed/LSPosed.git)
- **Vector**：推荐使用，适配 libxposed 100 以前及之后的版本；[JingMatrix/Vector](https://github.com/JingMatrix/Vector.git)

| 模块名称/作用目标 | 地址 | LSPosed | Vector | 备注 |
| --- | --- | --- | --- | --- |
| Thanox | [Tornaco/Thanox](https://github.com/Tornaco/Thanox) | ✓ | ✓ | 冰箱类似物，需要付费（`20RMB / 设备 / 永久` 或 `$5 / 不限设备 / 永久`） |
| 哔哩哔哩 | [yujincheng08/BiliRoaming](https://github.com/yujincheng08/BiliRoaming.git) | ✓ | ✓ | 软件优化；已经 PA，推荐用 BBZQ |
| BBZQ | [HSSkyBoy/BBZQ](https://github.com/HSSkyBoy/BBZQ.git) | ✗ | ✓ | 软件优化 |
| Telegram | [unexpecteds/TAuxiliary](https://modules.lsposed.org/module/org.telegram.auxiliary/) | ✗ | ✓ | 软件优化；另推荐 [shatyuka/Killergram](https://github.com/shatyuka/Killergram.git) 去广告 |
| qq | [cinit/QAuxiliary](https://github.com/cinit/QAuxiliary.git) | ✓ | ✓ | 软件优化；有风控风险，谨慎使用 |
| 菜鸟 | [duzhaokun123/FuckCainiao](https://github.com/duzhaokun123/FuckCainiao.git) | ✓ | ✓ | 软件优化 |
| 知乎 | [shatyuka/Zhiliao](https://github.com/shatyuka/Zhiliao.git) | ✓ | ✓ | 软件优化 |
| 抖音 | [twyora/DouyinEnhancer](https://github.com/twyora/DouyinEnhancer.git) | ✓ | ✓ | 软件优化 |
| ChiMi | [yonghen/chimi-](https://github.com/yonghen/chimi-) | ✓ | ✓ | MIUI 13 界面定制信息等优化 |
| DisableFlagSecure | [LSPosed/DisableFlagSecure](https://github.com/LSPosed/DisableFlagSecure.git) | ✗ | ✓ | 解除安卓安全限制（可以强制截屏） |
| Fuck Shake | [pwh-pwh/fuck_shake](https://github.com/pwh-pwh/fuck_shake.git) | ✓ | ✓ | 屏蔽摇一摇广告 |
| TwiFucker | [Dr-TSNG/TwiFucker](https://github.com/Dr-TSNG/TwiFucker.git) | ✓ | ✓ | 软件优化 |
| Hide My Applist | [Dr-TSNG/Hide-My-Applist](https://github.com/Dr-TSNG/Hide-My-Applist.git) | ✗ | ✓ | 喜欢侵犯隐私；旧版支持 api 100 之前，新版仅支持 101+ |
| LuckyTool | [Xposed-Modules-Repo/com.luckyzyx.luckytool](https://github.com/Xposed-Modules-Repo/com.luckyzyx.luckytool.git) | ✓ | ✓ | ColorOS 相关优化 |

## reference

1.   [刷了 Magisk 之后装什么？我推荐这 20+ 个模块](https://sspai.com/post/68531)
2.   [2023 年 Magisk 推薦安裝的模組，提升手機效能、擋廣告、自定義主題](https://ivonblog.com/posts/magisk-recommended-modules/)
3.   [一加手机官方 ROM 下载](https://yun.daxiaamu.com/OnePlus_Roms/)
4.   [一加手机 magisk 模块下载](https://yun.daxiaamu.com/files/magisk%E6%A8%A1%E5%9D%97/)
5.   [小米 rom 下载](https://xiaomirom.com/series/)
