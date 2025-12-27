# Claude Buddy

> Claude Code 开发的得力助手
>
> Claude Buddy 是一个强大的 CLI 工具，通过以下功能简化你的 Claude Code 工作流程：
>
> - **API 密钥管理**：轻松存储、切换和管理多个 Claude API 密钥
> - **模型映射**：便捷地自定义和管理模型配置
> - **快速配置**：通过直观的命令，几秒钟即可完成设置
> - **开发者友好**：专为专注于编码的开发者打造



<center>
  <img src="https://i.postimg.cc/1tcCx7bb/Screen-Shot-2025-12-24-164021-347.png" alt="MIT License">
</center>

## 通过 npm 安装

### npm主页
[npm主页](https://www.npmjs.com/package/@yesdgq/claude-buddy)

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


### Web 配置界面

使用以下命令启动配置管理界面：

```bash
ccby config
```



## 使用方法

### 基本使用

```bash
# 打开配置页面，配置您的 API 地址和访问令牌(TOKEN)
ccby config

# 启动claude code
ccby 或 claude

# 在指定目录中工作
ccby /path/to/project

# 查看历史会话
ccby -r

# 继续上次会话
ccby -c 

# 查看Claude-Buddy版本
ccby --version
ccby -v

# 查看Claude版本
claude --version
claude -v
```

其它更多方法，可参考 ：[claude code 使用文档](https://code.claude.com/docs/zh-CN/slash-commands)



## 许可证
MIT
