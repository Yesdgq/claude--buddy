
# Claude Buddy

[English](README.md) | [中文](README_zh.md)

## 概述

Claude Buddy 是一款简单易用的 CLI 工具，通过可视化方式快速配置 Claude Code、Codex 和 Gemini 等CLI的API密钥、模型映射等信息，可极大的方便和简化您对Claude Code等CLI的使用。



## 功能特性

 - **API 密钥管理**：轻松存储、切换和管理多组API 密钥
 - **模型映射**：便捷地自定义和管理模型配置
 - **一次安装永久使用**：本地部署，安装后可长久使用
 - **快速配置**：可视化界面，几秒钟即可完成设置
 - **开发者友好**：专为专注于编码的开发者打造



## npm主页

[项目npm主页](https://www.npmjs.com/package/@yesdgq/claude-buddy)



## 截图

<center>
  <img src="https://i.postimg.cc/Xv6qRCHc/Screen-Shot-2026-01-22-094205-987.png" alt="MIT License">
</center>


## 前提条件

- Node.js >= 18.0.0

  
## 安装

### 安装包
```bash
npm install -g @yesdgq/claude-buddy -f
```

### 更新包

```bash
npm update -g @yesdgq/claude-buddy
npm install -g @yesdgq/claude-buddy@latest
```

### 删除包

```bash
npm uninstall -g @yesdgq/claude-buddy
```



## 配置


### 可视化配置界面

使用以下命令启动可视化配置管理界面：

```bash
ccby config
```



## 可用命令


```bash
# 打开配置页面，配置您的 API 地址和访问令牌(TOKEN)
ccby config

# 启动claude code
ccby 或 claude

# 查看历史会话
ccby -r

# 继续上次会话
ccby -c

# 查看Claude-Buddy版本
ccby --version

# 查看Claude版本
claude --version

```
其它更多方法，可参考 ：[claude code 使用文档](https://code.claude.com/docs/zh-CN/slash-commands)

> [!IMPORTANT]
> **配置生效提示**：切换或更新配置后，需重启 Claude Code（CLI工具）方可生效。



## 使用问题

### Claude Code首次使用问题
首次配置后使用claude code若仍提示登录，或有如下异常提示等：
```ruby
Unable to connect to Anthropic services
Failed to connect to api.anthropic.com: ERR_BAD_REQUEST
Please check your internet connection and network settings.
```

可临时在终端设置环境变量运行一次：
```bash
# Mac OS使用如下命令：
export ANTHROPIC_BASE_URL=https://your-custom-api-endpoint.com
export ANTHROPIC_AUTH_TOKEN=your_api_token
claude

#Windows使用如下命令：
set ANTHROPIC_BASE_URL=https://your-custom-api-endpoint.com
set ANTHROPIC_AUTH_TOKEN=your_api_token
claude

之后即可使用ccby config管理你的配置了。

```



## 许可证

MIT



