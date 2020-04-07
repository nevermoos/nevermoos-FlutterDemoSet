##朋友app iOS flutter预研进度与规划

### 一、背景

#### 1.1、背景与目标

以多端复用为目的，在朋友app iOS端预研flutter

#### 1.2、行业内参考

阿里闲鱼在行业内是flutter运用比较成熟的，从2019年10月他们的一篇[实践博客](https://developer.aliyun.com/article/720799)来看，有一些值得我们关注和借鉴的数据：

- 研究成果：从2017年开始调研，到2019年10月，用了2年，闲鱼完成了预研、研发到成熟的过程，有相对成熟的框架及定制化底层支持，有20多个页面使用flutter构建
- 关键节点：开始调研实践-2017年；将flutter用于开发实践-约2018年7月；开源Fish Redux flutter应用框架-约2019年3月；开源AspectD AOP框架-约2019年6月
- 质量：Crash 水平在万分之一的数量级，详情页等帧率在 52 帧以上，可交互的页面加载时长是 300 毫秒
- 投入：闲鱼针对engine、flutter、dart、ui不同层次都有相应的定制化以及框架支撑。从入门到成熟，随着问题和功能的需要，很有可能我们也需要相应的投入。

### 二、整体规划

#### 2.1、基础入门阶段

1. 调研flutter技术大致原理、熟悉dart语法
2. 调研flutter与原生集成、通信交互方式，跑通demo工程

#### 2.2、实验阶段

1. flutter模块与企业微信工程融合，能够集成进去，跑起来，数据能够简单通信
2. 以一个功能模块为范例，用flutter复写，能够正常运行，并在Android端上线
3. 范例模块在Android、iOS共同上线，实现双端复用的开始

#### 2.3、成熟性建设阶段

1. flutter端基础框架建设，包括flutter栈、数据通信、ui框架、监控、网络等框架建设
2. 原生端与flutter端通信优化，数据通信从cpp直接与flutter通信，跳过jni、java层
3. 微信dart2cpp通信方案调研，能否借鉴，以提升通信效率
4. 其它定制化需求，如果有需要，或许要考虑flutter engine的定制化



com.pal.ARSections



https://github.com/flutterchina/flutter-in-action

https://www.jianshu.com/p/805f45d5793a

https://github.com/OpenFlutter/Flutter-Notebook

https://flutter-widget.live/zh_CN/widgets/Switch

https://api.flutter.dev/flutter/animation/animation-library.html

https://flutter.cn/docs/cookbook

https://github.com/flutter/samples/blob/master/INDEX.md

https://github.com/nisrulz/flutter-examples

https://dart.cn/guides/language/effective-dart/style

https://dart.cn/guides/libraries/library-tour

https://flutter.dev/docs/development/tools/devtools/inspector

https://api.flutter.dev/flutter/widgets/Flex-class.html

https://flutter.cn/docs/get-started/install/macos

https://flutter.cn/

https://juejin.im/post/5e228d21518825265c248e7b#heading-3

https://juejin.im/post/5e5f1d41518825495b29a05b

https://juejin.im/post/5e19306c6fb9a02ff67d3780

https://juejin.im/post/5e6f23eef265da574f355950

http://km.oa.com/group/38650/articles/show/412972?kmref=search&from_page=2&no=7

[http://km.oa.com/group/fluttergo/articles/show/402042#2.1%E3%80%81%E5%86%B7%E5%90%AF%E5%8A%A8%E4%B8%8E%E7%83%AD%E5%90%AF%E5%8A%A8](http://km.oa.com/group/fluttergo/articles/show/402042#2.1、冷启动与热启动)

https://mp.weixin.qq.com/s/0uVRSSRVUrXUTAJ3ftEN5w?from=timeline&isappinstalled=0&scene=2&clicktime=1585818393&enterid=1585818393

