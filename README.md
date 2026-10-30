# HyperHand

小米 14 / HyperOS 3（Android 16）原生单手模式触发增强。

在系统自带的一手模式手势通道上做"底部快速下滑"判定，命中后调用原生
`OneHandedController.startOneHanded()` —— 缩小动画、缩小布局、触摸映射、
退出方式全部沿用系统实现；只扩大底部触发区（25dp → 56dp）、加入向下
峰值速度门限，并与桌面的下拉通知/控制中心手势互斥。

## 安装

从 [Releases](../../releases) 下载 `HyperHand.apk`，在 Vector / LSPosed 中启用即可。

- 作用域已静态声明：`com.android.systemui`、`com.miui.home`
- 需要支持 **libxposed API 102** 的框架（Vector 2.x / 新版 LSPosed）

## 源码

https://github.com/zPan2327/HyperHand

## License

MIT
