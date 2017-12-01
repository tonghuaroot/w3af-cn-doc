# w3af 中文文档

## 前言
本文档为对 w3af 官方文档的翻译，除了将英文内容完全通过中文呈现出来外，还会加一些我对部分内容的理解。若后续时间充裕还会写一些源码分析。

## 相关素材
- [w3af 官网](http://w3af.org/)
- [w3af 官方文档](http://docs.w3af.org/en/latest/)
- [w3af 项目仓库](https://github.com/andresriancho/w3af/)

## 欢迎来到w3af中文文档
本文档是 Web 应用程序攻击和审计框架（w3af）的用户指南，撰写本文档的目的是提供w3af的基本概述、工作原理以及使用说明。


w3af 是审计和利用Web应用程序的完整环境。这个环境为 Web 漏洞评估和渗透测试提供了一个可靠的平台。

## 目录
- [安装](http://docs.w3af.org/en/latest/install.html)
- - [安装前的准备](http://docs.w3af.org/en/latest/install.html#prerequisites)
- - [安装](http://docs.w3af.org/en/latest/install.html#id1)
- - [支持平台](http://docs.w3af.org/en/latest/install.html#supported-platforms)
- - [在Kali中安装](http://docs.w3af.org/en/latest/install.html#installation-in-kali)
- - [使用Docker安装](http://docs.w3af.org/en/latest/install.html#installing-using-docker)
- - [使用Mac OSX安装](http://docs.w3af.org/en/latest/install.html#installation-in-mac-osx)
- - [故障排除](http://docs.w3af.org/en/latest/install.html#troubleshooting)
- [高级安装](http://docs.w3af.org/en/latest/advanced-install.html)
- - [开发版 vs 稳定版](http://docs.w3af.org/en/latest/advanced-install.html#bleeding-edge-vs-stable)
- - [使用 virtualenv 安装](http://docs.w3af.org/en/latest/advanced-install.html#installing-using-virtualenv)
- [更新至最新版](http://docs.w3af.org/en/latest/update.html)
- - [手动更新](http://docs.w3af.org/en/latest/update.html#manually-updating)
- - [自动更新功能](http://docs.w3af.org/en/latest/update.html#auto-update-feature)
- - [git 分支](http://docs.w3af.org/en/latest/update.html#branches)
- [介绍](http://docs.w3af.org/en/latest/phases.html)
- - [主要插件类型](http://docs.w3af.org/en/latest/phases.html#main-plugin-types)
- - [其他插件](http://docs.w3af.org/en/latest/phases.html#other-plugins)
- - [扫描配置](http://docs.w3af.org/en/latest/phases.html#scan-configuration)
- - [配置建议](http://docs.w3af.org/en/latest/phases.html#scan-configuration)
- [运行 w3af](http://docs.w3af.org/en/latest/basic-ui.html)
- - [运行 w3af 图形界面](http://docs.w3af.org/en/latest/basic-ui.html#running-w3af-with-gtk-user-interface)
- - [插件配置](http://docs.w3af.org/en/latest/basic-ui.html#plugin-configuration)
- - [保存配置](http://docs.w3af.org/en/latest/basic-ui.html#saving-the-configuration)
- - [开始扫描](http://docs.w3af.org/en/latest/basic-ui.html#starting-the-scan)
- [自动化使用脚本](http://docs.w3af.org/en/latest/scripts.html)
- - [VIM 语法文件](http://docs.w3af.org/en/latest/scripts.html#vim-syntax-file)
- [认证](http://docs.w3af.org/en/latest/authentication.html)
- - [基础NTLM身份认证](http://docs.w3af.org/en/latest/authentication.html#basic-and-ntlm-authentication)
- - [表单认证](http://docs.w3af.org/en/latest/authentication.html#form-authentication)
- - [设置 HTTP Cookie](http://docs.w3af.org/en/latest/authentication.html#setting-http-cookie)
- - [设置 HTTP 头](http://docs.w3af.org/en/latest/authentication.html#setting-http-headers)
- [常见用例](http://docs.w3af.org/en/latest/common-use-cases.html)
- - [只扫描一个目录](http://docs.w3af.org/en/latest/common-use-cases.html#scanning-only-one-directory)
- - [保存URL并将其作为其他扫描的输入](http://docs.w3af.org/en/latest/common-use-cases.html#saving-urls-and-using-them-as-input-for-other-scans)
- [高级用例](http://docs.w3af.org/en/latest/advanced-use-cases.html)
- - [复杂 Web 应用](http://docs.w3af.org/en/latest/advanced-use-cases.html#complex-web-applications)
- - [REST API](http://docs.w3af.org/en/latest/advanced-use-cases.html#rest-apis)
- - [选择要忽略的表单](http://docs.w3af.org/en/latest/advanced-use-cases.html#choosing-which-forms-to-ignore)
- [docker 中的 w3af](http://docs.w3af.org/en/latest/docker.html)
- - [端口和服务](http://docs.w3af.org/en/latest/docker.html#ports-and-services)
- - [与容器共享数据](http://docs.w3af.org/en/latest/docker.html#sharing-data-with-the-container)
- - [调试容器](http://docs.w3af.org/en/latest/docker.html#debugging-the-container)
- [利用 Web 应用漏洞](http://docs.w3af.org/en/latest/exploitation.html)
- [Web 应用 payload](http://docs.w3af.org/en/latest/advanced-exploitation.html#running-web-application-payloads)
- - [介绍](http://docs.w3af.org/en/latest/advanced-exploitation.html#introduction)
- - [运行 Web 应用 payload](http://docs.w3af.org/en/latest/advanced-exploitation.html#running-web-application-payloads)
- - [通过肉鸡进行流量代理](http://docs.w3af.org/en/latest/advanced-exploitation.html#proxying-traffic-through-the-compromised-host)
- [Bug 报告](http://docs.w3af.org/en/latest/report-a-bug.html)
- - [优质 bug 报告案例](http://docs.w3af.org/en/latest/report-a-bug.html#good-bug-reporting-practices)
- - [基础调试信息](http://docs.w3af.org/en/latest/report-a-bug.html#basic-debugging)
- - [漏报](http://docs.w3af.org/en/latest/report-a-bug.html#false-negatives)
- - [误报](http://docs.w3af.org/en/latest/report-a-bug.html#false-positives)
- - [常见问题](http://docs.w3af.org/en/latest/report-a-bug.html#common-problems)
- - [过时的配置文件](http://docs.w3af.org/en/latest/report-a-bug.html#outdated-profiles)
- [贡献力量](http://docs.w3af.org/en/latest/contribute.html)

