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
