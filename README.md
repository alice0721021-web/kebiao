# 课程表（Timetable）

一个自用的 Android 课程表应用，基于 WebView 实现，支持按周查看课程表。

## 项目说明

- 应用名：课程表
- 包名：`com.operit.timetable.blank`
- 当前 APK：`Timetable-Blank-1.0.apk`
- 功能：
  - 7 天布局（周一到周日）
  - 按周切换
  - 文件导入
  - 粘贴导入
  - 清空课表
  - 本地保存与启动恢复

## 目录结构

```
kebiao/
├── blank_app/
├── Timetable-Blank-1.0.apk
├── 开发计划.md
├── LICENSE
└── README.md
```

## 构建说明

当前为手工构建工程，未使用 Gradle。构建流程包括：

1. 编译 Java
2. 编译并链接资源
3. 生成 dex
4. 打包 APK
5. 签名 APK

## 持久化说明

应用使用 Java 侧本地文件保存课程数据，不依赖 WebView 本地缓存。
