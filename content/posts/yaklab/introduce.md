---
title: "00-yakLab靶场Vulinbox-前言"   # 把文件名自动转成中文标题
date: 2025-10-20T14:20:47+08:00                              # 当前时间
draft: false                                    # 默认草稿，写完改 false
categories: ['yakLab']
tags: []
summary: ""                                    # 手动写摘要，避免系统自动截断
featuredImage: ""                              # 题图 URL，空着就无图
featuredImagePreview: ""                       # 列表页缩略图，可同图
toc: true                                      # 是否显示目录（true=开，false=关）
autoCollapseToc: true                          # 目录自动折叠
codeMaxLines: 10                               # 代码块默认折叠行数
codeLineNumbers: true                          # 代码行号
comment: true                                  # 是否开启评论
reward: false                                  # 是否开启打赏
pinned: false                                  # 是否置顶（FixIt 支持）
weight: 100                                    # 置顶权重，越大越靠前
---

【还在用 DVWA、Pikachu 练手？——是时候升级了】

DVWA、Pikachu 陪伴了无数人入门，但“OWASP Top 10 跑一遍就毕业”的痛点也客观存在：  
场景浅、更新慢、缺少逻辑漏洞与前端加密等高级主题。  
如果想把“能跑通”变成“能实战”，你需要一块更现代的靶场——Vulinbox（Yakit 官方出品）。

---

## 1. Vulinbox 是什么？

一句话：覆盖 OWASP Top 10、业务逻辑、组件漏洞、前端加解密与 JWT 伪造的「一站式综合靶场」。

- 20+ 漏洞模块，持续按月迭代
    
- 全中文界面 + 分级 Hint + 官方 WriteUp
    
- 单二进制、零依赖、一键启动，5 分钟完成部署
    
- 与 Yakit 抓包、Web Fuzzer、热加载脚本无缝联动，练习即实战
    

---

## 2. 安装 & 启动（3 步，5 分钟）

### 1. 装 Yakit
    
    - 官网 [yaklang.com](https://yaklang.com/) 一条命令或直链 exe，双击即可
	    ![|300](https://raw.githubusercontent.com/pa0paO2/blog_picb/main/official/20251017154532449.png)
### 2. 开靶场  
    右上角「设置」→ 实验性功能 → Vulinbox → 一键安装（镜像 ≈ 100 MB）
    ![|300](https://raw.githubusercontent.com/pa0paO2/blog_picb/main/official/20251017154532450.png)
    ![|300](https://raw.githubusercontent.com/pa0paO2/blog_picb/main/official/20251017154532451.png)
### 3. 跑起来  
    默认端口 8787 → Start，浏览器自动弹出 `http://127.0.0.1:8787`，开刷！
    ![|300](https://raw.githubusercontent.com/pa0paO2/blog_picb/main/official/20251017154532452.png)

> 端口冲突？在启动页随意改；用完点 Stop，进程干净退出。

---

## 3. 横向对比：Vulinbox vs 传统靶场


| 维度   | Vulinbox           | DVWA      | Pikachu   | WebGoat    |
| :--- | :----------------- | :-------- | :-------- | :--------- |
| 安装成本 | 单文件，零依赖            | PHP+MySQL | PHP+MySQL | Java+Maven |
| 漏洞深度 | 前端加密、JWT、SSRF、逻辑越权 | 10 类基础    | 15 类基础    | 30+ 企业级    |
| 中文支持 | 界面+文档全中文           | 英文        | 中文        | 英文         |
| 更新频率 | 每月迭代               | 年更        | 已停更       | 季更         |
| 上手体验 | Hint/WriteUp/一键抓包  | 纯手动       | 无提示       | 英文教程       |
|      |                    |           |           |            |

结论：

- 0-1 年新手：Vulinbox 足够友好，场景又新
    
- 1-3 年进阶：前端加密、业务逻辑关卡直接对标实战
    
- 红队应急：拿来验证 Payload 比自建环境快 10 倍
    

---

## 4. 高效通关路线

1. 按目录逐级刷：SQL 注入 → XSS → SSRF → 逻辑越权 → 前端加密 → JWT
	
2. 每关先看 Hint，再 F12 读源码，养成“先看验证逻辑再下手”的习惯
    
3. 每类漏洞写 3 行总结，沉淀成自己的「漏洞手册」
    
---

## 5. 下一站：实战连载预告

环境已就绪，下一篇带你打  
「高级前端加解密与验签实战 —— HMAC-SHA256 表单爆破」：

- 定位签名算法 → 手搓 JS 脚本 → 口令爆破 → 热加载自动化  
    可选择用 Yakit或burpsuite，搭配一个编译器
    

> 靶场就绪，练习开始。