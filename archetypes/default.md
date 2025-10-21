---
title: "{{ replace .Name "-" " " | title }}"   # 把文件名自动转成中文标题
date: {{ .Date }}                              # 当前时间
draft: true                                    # 默认草稿，写完改 false
categories: []
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