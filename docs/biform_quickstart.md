﻿# 快速开始

通过本文，您可以了解到基于 biForm 的一些主要信息，并了解到如何使用 biForm 进行开发。

随着 biForm 的发展，本文档还会不断更新。如果找不到您需要的信息，请告诉我们，我们会尽力添加相关内容，并在此过程中帮助您！


## 简单介绍一下 biForm

biForm 是一个以 Python3 为脚本语言的集成化开发工具。底层使用了 Qt5。

目前最新版本 V3.1 基于 Python 3.6 及 Qt 5.11.1。

biForm适合于开发需要图形化用户界面（GUI）的桌面应用。以“表单”为所有应用的基本构成单元。

## biForm 的基础概念

### 在 biForm 的世界里，**一切皆表单**。

这种**表单**在biForm中有特定的格式和功能。biForm 是一个针对这类表单的**界面设计器、脚本编器、调试、试运行、打包发布**功能于一体的集成式开发环境。

设计好的一个“表单”最终会以一个**PFF文件**的形式发布并提供给最终用户。PFF是便捷式表单文件（**Portable Form File**）的缩写。

一个PFF文件通常针对一个具体的、相对独立的功能，比如“销售订单.PFF”就是一个用来对销售订单进行增、删、改、查、导出、导入、打印等操作的表单，“销售日报.PFF”就是一个用来对每日销售数据进行汇总统计的表单。

一个或多个“表单”可组合出各种复杂的功能。多个PFF文件也可以打包成应用程序包。比如“销售订单.PFF”、“销售日报.PFF”、“采购订单.PFF”及其他相关表单就可以一起打包成为一个进销存系统。

最终用户通过使用**百利孚软件应用平台**（简称**biReader**）使用这些表单。

### biReader 是什么？

biReader 是供最终用户使用的运行时环境。它的功能是为PFF表单提供环境，响应用户的操作，与操作系统和数据库管理系统底层进行交互，与其它表单协作和共享数据，组合起来完成各类复杂的功能。

有的PFF表单需要使用数据库，在设计时只设计表结构，并不直接与DBMS相关。一般情况下，同一个PFF表单，可以在不同的数据库管理使用。根据用户启动时连接的数据源，自动创建数据表，且会与其它共享数据表的PFF自动进行集成。

使用不同的数据库管理系统，PFF表单的功能一般不会受到影响。但也有些PFF表单是专门针对某类数据库管理系统设计的，那这种表单就只能使用特定的数据库管理系统。

### biReader 和 PFF 的关系

- PFF表单并不是可执行程序，但通过biReader打开一个PFF文件，就可以执行其中的程序
- 每个PFF表单都可以单独被biReader打开使用
- 多个PFF表单可以组合起来完成更复杂的功能
- PFF表单的组合可以由最终用户自己组合，也可以由开发人员将相关表单组合打包为PFP文件后一起发布
- 多个不相关的PFF表单都可以在同一个biReader中使用，互不干扰
- biReader本身没有具体的面向最终用户的功能，它只是提供运行时底层环境，通过使用PFF文件来实现各种应用

## 版本

目前发布的版本是 **biForm V3.1** 和 **biReaderV3.1**。

Windows 版本

[下载biForm V3.1 其中已包含biReader V3.1](https://www.bilive.com/site_media/media/setup/Setup_biform_V3.1.msi)

Linux 版本

[下载 Deepin Linux V15.10 amd 64bit 适用版](https://www.bilive.com/site_media/media/setup/biform_v3.1.001_amd64_20190819.zip)

[下载 Deepin Linux V15.5 龙芯 64bit 适用版](https://www.bilive.com/site_media/media/setup/biform_v3.1.001_loongson_20190819.zip)

[下载 Linux Mint V19.1 mate 64bit 适用版](https://www.bilive.com/site_media/media/setup/biform_v3.1.001_mint19_20190526.zip)

[更多文档](https://www.bilive.com/site_media/media/setup/bilive_doc.zip)

[本文档所用示例下载](https://www.bilive.com/site_media/media/setup/bilive_demo.zip)

biReader V3.1 支持 SQLite、MS SQL Server2000/2005/2008、PostgreSQL 等数据库管理系统。

操作系统目前发布的版支持Windows系列各版本及Linux部分发行版。未来会陆续发布支持其他DBMS、其它操作系统的版本。


## 从一个简单的表单开始使用 biForm

通过这个[书籍清单管理的例子](guides/first_form)了解如何使用 biForm。 


## 获取开发者账号

联系biForm开发团队 <bilive@foxmail.com> ，获取开发者账号。

注册过开发者账号之后，biForm发布的PFF可不受限制使用。

未经注册的biForm，开发生成的PFF在最终用户处使用时会受到一定限制。

## 获取更多文档和帮助

访问 [官方网站](https://www.bilive.com) 获得更多文档和帮助。
