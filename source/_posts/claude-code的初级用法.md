---
title: claude code的初级用法
tags:
  - Claude code
categories:
  - Agent
thumbnail: "https://cdn.jsdelivr.net/gh/dengxuduo408-commits/image-bed@main/img/20261124213206120.png"
date: 2026-11-24 21:28:53
---
### 一、基础指令
1、shift+tab 切换权限模式：auto mode、manual mode等。
2、回滚：若是不满意这一版的输出，反而要上一版的输出，可以使用回滚功能。
- 点两次Esc
- 输入 /rewind

### 二、基础用法
建立CLAUDE.md，这是agent每次运行前都会遵循的原则。
1、建议在项目初具雏形的时候，让ai为你生成该项目的CLAUDE.md。
2、后续可以输入/memory命令，选择project或者user（全局）instructions，来手动添加原则。
*这里小编建议不要塞太多东西，都是动态变化、不断修订的*

### 三、Skill
Skill分为四类：知识型、流程型、工具型、混合型。
那如何寻找好用的Skill呢，我们可以使用Skill来找Skill——"find-skills"
https://github.com/vercel-labs/skills

### 四、Hook
Prompt：帮我做个hook，我想要你XX的时候，你能XX。（即触发某个条件时能做某件事）

### 五、subagent
手动让agent创建几个subagent，再让他自己来分配任务

### 六、plugin
使用/plugins，可以discover plugin