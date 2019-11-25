---
title: .NET Core 2.1 信任证书
permalink: dotnet-dev-certs
updated: '2018-05-31 14:17:16'
date: 2018-05-31 14:17:16
tags:
- .NET Core
categories:
- .NET 笔记
---



新安装的.NET Core Sdk 2.1.300，会提示以下信息，信任证书后能使用https访问ASP.NET Core的页面：


> 已成功安装 ASP.NET Core HTTPS 开发证书。
要信任证书(仅限 Windows 和 macOS)，请首先通过运行 "dotnet tool install dotnet-dev-certs -g --version 2.1.0-preview1-final" 安装 dev-certs 工具，然后运行 "dotnet-dev-certs https --trust"。

这是按提示在powershell或者cmd中执行:

```bash
dotnet tool install dotnet-dev-certs -g --version 2.1.0

dotnet-dev-certs https --trust
```