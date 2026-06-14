# Study Garden

**Study Garden** 是一款使用 SwiftUI 开发的 macOS 学习效率 App，主要面向学生和轻办公用户，帮助用户管理任务、DDL、每日计划和专注时间。

它结合了任务管理、今日计划和小番茄钟功能，让用户可以更清晰地安排学习节奏，并通过番茄钟把计划真正执行起来。

## Features｜主要功能

* **任务与 DDL 管理**：添加短期任务或长期目标，并设置截止时间。
* **今日计划**：为当天安排具体时间段和学习/工作内容。
* **小番茄钟**：支持 30 分钟专注计时。
* **任务/计划绑定**：番茄钟可以绑定具体任务或今日计划。
* **本地数据保存**：任务、计划和番茄钟记录会保存在本地。
* **系统提醒**：支持 DDL 提醒和番茄钟完成提醒。
* **治愈风 UI**：采用柔和、简洁的界面风格，降低学习压力。

## Tech Stack｜技术栈

* Swift
* SwiftUI
* SwiftData
* UserNotifications
* Xcode
* macOS App Development
* AI-assisted development / Vibe Coding

## Requirements｜运行要求

由于本项目使用了 **SwiftData**，因此需要：

* macOS 14.0 Sonoma 或更高版本
* Xcode 15 或更高版本，如果你想从源码运行
* Apple Silicon 或 Intel Mac 均可尝试运行

如果你的 macOS 版本较低，可能会出现：

> This version of Study Garden is not compatible with this version of macOS.

这种情况下需要更新 macOS，或修改项目的数据存储方式。

## Download｜下载安装

### 方法一：从 GitHub Releases 下载 App

1. 打开本项目的 GitHub 页面。
2. 点击右侧或上方的 **Releases**。
3. 下载最新版本中的 `.zip` 文件。
4. 解压后得到 `Study Garden.app`。
5. 将 `Study Garden.app` 拖入 **Applications / 应用程序** 文件夹。
6. 双击打开 App。

如果 macOS 提示：

> “Study Garden” can’t be opened because Apple cannot check it for malicious software.

请使用下面的方法打开：

1. 右键点击 `Study Garden.app`。
2. 选择 **Open / 打开**。
3. 在弹窗中再次点击 **Open / 打开**。

或者：

1. 打开 **System Settings / 系统设置**。
2. 进入 **Privacy & Security / 隐私与安全性**。
3. 找到 Study Garden 的安全提示。
4. 点击 **Open Anyway / 仍要打开**。

这是因为 App 目前是个人项目，没有通过 Apple Developer notarization，不代表 App 一定有问题。

### 方法二：从源码运行

1. 打开 Terminal 终端。

2. 克隆项目：

```bash
git clone 你的GitHub仓库链接
```

例如：

```bash
git clone https://github.com/your-username/StudyGarden.git
```

3. 进入项目文件夹：

```bash
cd StudyGarden
```

4. 使用 Xcode 打开项目：

```bash
open StudyGarden.xcodeproj
```

如果你的项目是 workspace 文件，则使用：

```bash
open StudyGarden.xcworkspace
```

5. 在 Xcode 左上角选择运行目标为 **My Mac**。

6. 点击左上角的运行按钮，或按快捷键：

```text
Command + R
```

7. App 会在 Mac 上启动。

## How to Use｜使用教程

### 1. 首页总览

打开 App 后，你会看到 Study Garden 的首页。

首页主要展示：

* 今天的日期
* 今日番茄数量
* 今日计划数量
* 待完成任务数量
* 快速进入入口
* 快到 DDL 的任务

你可以通过首页快速进入：

* **任务 & DDL**
* **今日计划**
* **小番茄钟**

### 2. 添加任务与 DDL

进入 **任务 & DDL** 页面后，可以添加新的学习或工作任务。

操作步骤：

1. 输入任务名称，例如：`完成数学作业`。
2. 输入备注，例如：`先写第 1-3 题`。
3. 选择任务类型：

   * 短期任务
   * 长期目标
4. 选择截止日期和时间。
5. 点击 **种下这个任务**。
6. 任务会被保存到本地，并出现在任务列表中。

任务状态会根据 DDL 自动变化，例如：

* 今天截止
* 明天截止
* 还剩几天
* 已过期

### 3. 使用今日计划

进入 **今日计划** 页面后，可以为当天安排具体时间段。

操作步骤：

1. 选择开始时间。
2. 选择结束时间。
3. 输入计划内容，例如：`复习线性代数`。
4. 点击添加计划。
5. 计划会出现在今日计划列表中。

今日计划适合用来安排：

* 上课时间
* 写作业时间
* 复习时间
* 项目开发时间
* 休息和运动时间

### 4. 使用小番茄钟

进入 **小番茄钟** 页面后，可以开始专注计时。

操作步骤：

1. 选择绑定类型：

   * 绑定任务
   * 绑定计划
2. 选择一个具体任务或今日计划。
3. 点击 **开始**。
4. 番茄钟开始倒计时。
5. 完成后点击 **完成**，系统会记录本次专注。

如果绑定的是普通任务，默认专注时间为 30 分钟。

如果绑定的是今日计划，番茄钟可以根据计划的开始和结束时间自动生成专注时长。

### 5. 查看专注记录

完成番茄钟后，App 会记录当天的专注情况，包括：

* 今日番茄数量
* 今日专注分钟数
* 当前绑定任务
* 已完成的番茄记录

这些记录可以帮助用户复盘自己的学习状态。

## Project Highlights｜项目亮点

* 从 0 到 1 独立完成 macOS App 产品原型开发。
* 使用 SwiftUI 搭建完整桌面应用界面。
* 使用 SwiftData 实现本地数据持久化。
* 将任务管理、今日计划和番茄钟连接成完整学习闭环。
* 使用 AI-assisted development / Vibe Coding 方式进行需求拆解、代码生成、Bug 排查和 UI 迭代。
* 完成 App 图标设计、打包导出和本地分发测试。

## About This Project｜项目说明

Study Garden 是一个个人项目，也是一次 AI-assisted development / Vibe Coding 实践。

开发过程中，我通过 AI 辅助完成了需求拆解、功能规划、SwiftUI 代码实现、Bug 调试、UI 风格迭代和打包部署。项目重点不只是完成一个 Demo，而是将一个真实的学习自律需求转化为可以实际运行的 macOS 桌面应用。

## Author｜作者

**韩逸雪**

Project Role:

* Product Design
* UI Design
* SwiftUI Development
* AI-assisted Development
* Vibe Coding Practice

## License｜许可证

This project is for learning and portfolio purposes.

You may modify this section based on your preferred license.
