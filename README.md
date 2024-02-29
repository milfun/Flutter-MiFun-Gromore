# Flutter-MiFun-Gromore
Flutter Gromore MiFun
logo

一款优质的 Flutter 广告插件（GroMore、穿山甲）
    
## MiFun-Gromore 有什么特点？
flutter项目中，使用kotlin语言，实现对接穿山甲gromore功能插件，不懂可以（🧑🏻‍💻咨询我【CMiFon】）。

### 插件特点
🔨 接入简单快速（封装原生端配置，仅需引入即可开始）
📡 事件统一返回（将原生端各种重要回调事件统一返回，方便业务处理和埋点统计等需求）
🎁 注重优化体验（无闪烁 Logo 开屏、iOS 开屏防止事件穿透、权限申请、隐私跟踪申请等）
🏆 极客代码封装（原生端代码不凑合，两端统一基础框架、广告事件封装抽象、易扩展）

### 支持功能
✅ 开屏广告
✅ 插屏广告  可自己写
✅ 横幅广告
✅  激励视频 
🏆 信息流（🚀 Pro 版）
🏆 激励视频-二次激励（可大幅提升收益，🚀 Pro 版）
🏆 实时获取 eCPM（上报归因，买量更有效，🚀 Pro 版）
🏆 可视化测试工具（高效测试，直击问题，🚀 Pro 版）
🏆 预缓存能力（提高展示率，增加收益，🚀 Pro 版）

## 开屏广告

``` dart
  FlutterPangleAds.showSplashAd(
     AdsConfig.splashId,
     logo: AdsConfig.logo,
     timeout: 3.5,
  );
```

## SDK初始化
``` dart


   bool result = await MiFunGromore.initAd(
      AppConfig.kAppId,
      config: AppConfig.appPlatform,
      limitPersonalAds: 1,
    );
```

## 激励广告
```
await MiFunGromore.showRewardVideoAd(
  AppConfig.gRewardVideoSlot,
  customData: "customData",
);
```
