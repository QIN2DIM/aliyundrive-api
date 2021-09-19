---
title: "Quick Start"
date: 2021-09-19T14:49:13+08:00
draft: false
weight: 3

---





快速上手面向开发者的阿里云盘API，并使用Python获取账号信息。

## Intro

- 截止至2021/09/15，`Aliyundrive`仍采用`access-token` + `auto refresh`机制实现用户鉴权以及身份信息的超时更新。
- 需要通过手动（或额外的自动化操作脚本）的方式“首次”获取`access_token`、`refresh_token`以及`default_drive_id` ，之后可携带“更新码”请求相应的接口实现身份信息的自动化更新。

## Get Token

