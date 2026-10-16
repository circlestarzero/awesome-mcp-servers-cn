<p align="center">
  <img src="https://img.shields.io/badge/MCP-Servers-blue?style=for-the-badge&logo=modelcontextprotocol" alt="MCP">
  <img src="https://img.shields.io/badge/语言-中文-red?style=for-the-badge" alt="中文">
  <img src="https://img.shields.io/badge/🇨🇳-国内可用-brightgreen?style=for-the-badge" alt="国内可用">
  <img src="https://img.shields.io/github/stars/Vincent-crypto-coder/awesome-mcp-servers-cn?style=for-the-badge&logo=github" alt="Stars">
</p>

<h1 align="center">🔌 Awesome MCP Servers 中文合集</h1>

<p align="center">
  <b>精选 MCP 服务器合集 —— 国内开发者友好，标注国内可用性</b><br>
  <sub>Model Context Protocol · Claude · Cursor · Windsurf · Cline</sub>
</p>

---

## 什么是 MCP？

**MCP（Model Context Protocol）** 是 Anthropic 推出的开放协议，让 AI 助手（Claude、Cursor 等）能够连接外部工具和数据源。通过 MCP Server，AI 可以：

- 读写数据库
- 操作文件系统
- 调用 API
- 访问浏览器
- 控制智能家居
- ……

> 类比：MCP 之于 AI，就像 USB 之于电脑 —— 一个统一的接口标准。

## 📖 目录

- [官方服务器](#官方服务器)
- [数据库](#数据库)
- [文件系统](#文件系统)
- [Web 与浏览器](#web-与浏览器)
- [开发工具](#开发工具)
- [云服务与 DevOps](#云服务与-devops)
- [通讯与协作](#通讯与协作)
- [AI 与 LLM](#ai-与-llm)
- [搜索与知识](#搜索与知识)
- [媒体与创意](#媒体与创意)
- [智能家居](#智能家居)
- [中国生态](#中国生态)
- [如何使用](#如何使用)
- [如何贡献](#如何贡献)

---

## 官方服务器

由 MCP 官方团队维护的核心服务器。

| 名称 | 描述 | 国内可用 | 安装 |
|------|------|----------|------|
| [filesystem](https://github.com/modelcontextprotocol/servers/tree/main/src/filesystem) | 文件系统读写操作 | ✅ | `npx @modelcontextprotocol/server-filesystem` |
| [fetch](https://github.com/modelcontextprotocol/servers/tree/main/src/fetch) | HTTP 请求抓取网页 | ⚠️ 部分网站被墙 | `npx @modelcontextprotocol/server-fetch` |
| [memory](https://github.com/modelcontextprotocol/servers/tree/main/src/memory) | 知识图谱持久记忆 | ✅ | `npx @modelcontextprotocol/server-memory` |
| [everything](https://github.com/modelcontextprotocol/servers/tree/main/src/everything) | 测试/参考服务器 | ✅ | `npx @modelcontextprotocol/server-everything` |
| [sequentialthinking](https://github.com/modelcontextprotocol/servers/tree/main/src/sequentialthinking) | 链式思考推理 | ✅ | `npx @modelcontextprotocol/server-sequentialthinking` |

## 数据库

| 名称 | 描述 | 国内可用 | 安装 |
|------|------|----------|------|
| [postgres](https://github.com/modelcontextprotocol/servers/tree/main/src/postgres) | PostgreSQL 读写查询 | ✅ | `npx @modelcontextprotocol/server-postgres` |
| [sqlite](https://github.com/modelcontextprotocol/servers/tree/main/src/sqlite) | SQLite 数据库操作 | ✅ | `npx @modelcontextprotocol/server-sqlite` |
| [mysql](https://github.com/nicholasoxford/mysql-mcp-server) | MySQL 数据库查询 | ✅ | `pip install mysql-mcp-server` |
| [redis](https://github.com/modelcontextprotocol/servers/tree/main/src/redis) | Redis 缓存操作 | ✅ | `npx @modelcontextprotocol/server-redis` |
| [milvus](https://github.com/zc276596/mcp-server-milvus) | Milvus 向量数据库 | ✅ | `pip install mcp-server-milvus` |
| [qdrant](https://github.com/modelcontextprotocol/servers/tree/main/src/qdrant) | Qdrant 向量数据库 | ✅ | `npx @modelcontextprotocol/server-qdrant` |
| [elasticsearch](https://github.com/elastic/mcp-server-elasticsearch) | Elasticsearch 搜索 | ✅ | `npx @elastic/mcp-server-elasticsearch` |
| [bigquery](https://github.com/LucasHild/mcp-server-bigquery) | Google BigQuery | ⚠️ 需要 GCP | `pip install mcp-server-bigquery` |

## 文件系统

| 名称 | 描述 | 国内可用 | 安装 |
|------|------|----------|------|
| [filesystem](https://github.com/modelcontextprotocol/servers/tree/main/src/filesystem) | 本地文件系统读写 | ✅ | `npx @modelcontextprotocol/server-filesystem` |
| [google-drive](https://github.com/modelcontextprotocol/servers/tree/main/src/google-drive) | Google Drive 文件访问 | ⚠️ 需要 Google | `npx @modelcontextprotocol/server-gdrive` |
| [obsidian](https://github.com/MarkusPfiztger/obsidian-mcp) | Obsidian 笔记库 | ✅ | `npx obsidian-mcp` |

## Web 与浏览器

| 名称 | 描述 | 国内可用 | 安装 |
|------|------|----------|------|
| [puppeteer](https://github.com/modelcontextprotocol/servers/tree/main/src/puppeteer) | 浏览器自动化（截图、点击） | ✅ | `npx @modelcontextprotocol/server-puppeteer` |
| [playwright](https://github.com/executeautomation/mcp-playwright) | Playwright 浏览器控制 | ✅ | `pip install mcp-playwright` |
| [firecrawl](https://github.com/mendableai/firecrawl-mcp-server) | 网页爬取 + Markdown 转换 | ⚠️ 需要 API Key | `npm install firecrawl-mcp` |
| [brave-search](https://github.com/modelcontextprotocol/servers/tree/main/src/brave-search) | Brave 搜索引擎 | ⚠️ 需要 API Key | `npx @modelcontextprotocol/server-brave-search` |
| [tavily](https://github.com/tavily-ai/tavily-mcp) | Tavily AI 搜索 | ⚠️ 需要 API Key | `npx tavily-mcp` |

## 开发工具

| 名称 | 描述 | 国内可用 | 安装 |
|------|------|----------|------|
| [github](https://github.com/modelcontextprotocol/servers/tree/main/src/github) | GitHub API（Issues/PR/Repo） | ✅ | `npx @modelcontextprotocol/server-github` |
| [gitlab](https://github.com/modelcontextprotocol/servers/tree/main/src/gitlab) | GitLab API | ✅ | `npx @modelcontextprotocol/server-gitlab` |
| [git](https://github.com/modelcontextprotocol/servers/tree/main/src/git) | 本地 Git 操作 | ✅ | `npx @modelcontextprotocol/server-git` |
| [docker](https://github.com/QuantGeekDev/docker-mcp) | Docker 容器管理 | ✅ | `npx docker-mcp` |
| [sentry](https://github.com/modelcontextprotocol/servers/tree/main/src/sentry) | Sentry 错误追踪 | ✅ | `npx @modelcontextprotocol/server-sentry` |
| [linear](https://github.com/tacticlaunch/mcp-linear) | Linear 项目管理 | ✅ | `npx mcp-linear` |

## 云服务与 DevOps

| 名称 | 描述 | 国内可用 | 安装 |
|------|------|----------|------|
| [aws](https://github.com/modelcontextprotocol/servers/tree/main/src/aws) | AWS 服务操作 | ✅ | `npx @modelcontextprotocol/server-aws` |
| [kubernetes](https://github.com/manusa/kubernetes-mcp-server) | K8s 集群管理 | ✅ | `npx kubernetes-mcp-server` |
| [terraform](https://github.com/hashicorp/terraform-mcp-server) | Terraform 基础设施 | ✅ | `npx terraform-mcp-server` |
| [cloudflare](https://github.com/cloudflare/mcp-server-cloudflare) | Cloudflare 管理 | ⚠️ 部分功能被墙 | `npx @cloudflare/mcp-server-cloudflare` |

## 通讯与协作

| 名称 | 描述 | 国内可用 | 安装 |
|------|------|----------|------|
| [slack](https://github.com/modelcontextprotocol/servers/tree/main/src/slack) | Slack 消息操作 | ⚠️ 国内用得少 | `npx @modelcontextprotocol/server-slack` |
| [discord](https://github.com/modelcontextprotocol/servers/tree/main/src/discord) | Discord 机器人 | ⚠️ 需要代理 | `npx @modelcontextprotocol/server-discord` |
| [notion](https://github.com/makenotion/notion-mcp-server) | Notion 页面/数据库 | ✅ | `npx @notionhq/notion-mcp-server` |
| [google-calendar](https://github.com/nsprovidence/google-calendar-mcp) | Google 日历 | ⚠️ 需要 Google | `npx google-calendar-mcp` |
| [feishu](https://github.com/nicholasoxford/feishu-mcp) | 飞书消息/文档 | ✅ | `pip install feishu-mcp` |

## AI 与 LLM

| 名称 | 描述 | 国内可用 | 安装 |
|------|------|----------|------|
| [ollama](https://github.com/arynnearidi/mcp-ollama) | Ollama 本地模型调用 | ✅ | `pip install mcp-ollama` |
| [openai](https://github.com/purpars/mcp-openai) | OpenAI API 调用 | ⚠️ 需要代理 | `pip install mcp-openai` |
| [huggingface](https://github.com/purpars/mcp-huggingface) | HuggingFace 模型 | ✅ (HF镜像) | `pip install mcp-huggingface` |
| [replicate](https://github.com/deepfates/mcp-replicate) | Replicate 模型运行 | ⚠️ 需要代理 | `npx mcp-replicate` |
| [langchain](https://github.com/rectalogic/langchain-mcp) | LangChain 集成 | ✅ | `pip install langchain-mcp` |

## 搜索与知识

| 名称 | 描述 | 国内可用 | 安装 |
|------|------|----------|------|
| [arxiv](https://github.com/blazickjp/arxiv-mcp-server) | arXiv 论文搜索 | ✅ | `pip install arxiv-mcp-server` |
| [wikipedia](https://github.com/nicholasoxford/mcp-wikipedia) | Wikipedia 查询 | ⚠️ 中文 Wikipedia 可用 | `npx mcp-wikipedia` |
| [wolframalpha](https://github.com/SecretiveShell/MCP-wolfram-alpha) | Wolfram Alpha 计算 | ✅ | `pip install mcp-wolfram-alpha` |
| [perplexity](https://github.com/purpars/perplexity-mcp) | Perplexity AI 搜索 | ⚠️ 需要代理 | `npx perplexity-mcp` |

## 媒体与创意

| 名称 | 描述 | 国内可用 | 安装 |
|------|------|----------|------|
| [image-gen](https://github.com/purpars/mcp-image-gen) | 图片生成（DALL-E） | ⚠️ 需要 OpenAI | `pip install mcp-image-gen` |
| [elevenlabs](https://github.com/purpars/elevenlabs-mcp) | 文字转语音 | ⚠️ 需要 API Key | `npx elevenlabs-mcp` |
| [youtube](https://github.com/anaisbetts/mcp-youtube) | YouTube 视频/字幕 | ⚠️ 需要代理 | `npx mcp-youtube` |
| [spotify](https://github.com/varunneal/spotify-mcp) | Spotify 音乐控制 | ⚠️ 需要代理 | `npx spotify-mcp` |

## 智能家居

| 名称 | 描述 | 国内可用 | 安装 |
|------|------|----------|------|
| [homeassistant](https://github.com/allenporter/mcp-server-home-assistant) | Home Assistant 控制 | ✅ | `pip install mcp-server-home-assistant` |
| [hue](https://github.com/bartvanandel/mcp-hue) | Philips Hue 灯光 | ✅ | `npx mcp-hue` |

## 中国生态

专为中国开发者打造或适配国内环境的 MCP 服务器。

| 名称 | 描述 | 国内可用 | 安装 |
|------|------|----------|------|
| [feishu](https://github.com/nicholasoxford/feishu-mcp) | 飞书消息、文档、日历 | ✅ | `pip install feishu-mcp` |
| [wechat-mp](https://github.com/nicholasoxford/wechat-mp-mcp) | 微信公众号 | ✅ | `pip install wechat-mp-mcp` |
| [dashscope](https://github.com/nicholasoxford/dashscope-mcp) | 通义千问 API | ✅ | `pip install dashscope-mcp` |
| [baidu-map](https://github.com/nicholasoxford/baidu-map-mcp) | 百度地图 | ✅ | `pip install baidu-map-mcp` |
| [alipay](https://github.com/nicholasoxford/alipay-mcp) | 支付宝支付 | ✅ | `pip install alipay-mcp` |
| [zhipu](https://github.com/nicholasoxford/zhipu-mcp) | 智谱 AI（GLM） | ✅ | `pip install zhipu-mcp` |

| [Doc2X MCP](https://github.com/NoEdgeAI/doc2x-mcp) | PDF/图片解析、文档导出与版面 JSON；MIT 开源 stdio 服务，API 按量计费 | ⚠️ 需自备 Doc2X API Key（未实测调用） | `npx -y @noedgeai-org/doc2x-mcp` |

> 🚧 中国生态 MCP 服务器还在快速发展中。如果你知道更多，请提交 PR！

---

## 如何使用

### 1. Claude Desktop

编辑 `~/Library/Application Support/Claude/claude_desktop_config.json`：

```json
{
  "mcpServers": {
    "filesystem": {
      "command": "npx",
      "args": ["@modelcontextprotocol/server-filesystem", "/path/to/allowed/dir"]
    },
    "sqlite": {
      "command": "npx",
      "args": ["@modelcontextprotocol/server-sqlite", "--db-path", "/path/to/db.sqlite"]
    }
  }
}
```

### 2. Cursor

在 `.cursor/mcp.json` 中配置：

```json
{
  "mcpServers": {
    "filesystem": {
      "command": "npx",
      "args": ["@modelcontextprotocol/server-filesystem", "/path/to/allowed/dir"]
    }
  }
}
```

### 3. Windsurf

在 `.windsurfrules` 或设置中添加 MCP 配置，格式同上。

### 4. Cline（VS Code 扩展）

在 Cline 设置中 → MCP Servers → 添加服务器配置。

---

## 🇨🇳 国内网络注意事项

| 问题 | 解决方案 |
|------|----------|
| `npx` 下载超时 | 用淘宝镜像：`npm config set registry https://registry.npmmirror.com` |
| `pip install` 慢 | 用阿里云镜像：`pip install -i https://mirrors.aliyun.com/pypi/simple/` |
| GitHub 克隆失败 | 用镜像：`git clone https://ghproxy.com/https://github.com/xxx/xxx.git` |
| 需要 OpenAI API | 用通义千问兼容模式替代，或用 [OpenRouter](https://openrouter.ai) |
| 需要 Google 服务 | 考虑用国内替代（百度地图替代 Google Maps 等） |

---

## 如何贡献

1. Fork 本仓库
2. 在对应分类下添加你的 MCP 服务器
3. 格式：`| [名称](GitHub链接) | 描述 | ✅/⚠️ | 安装命令 |`
4. 提交 PR

### 贡献要求

- 项目必须有 GitHub 仓库
- 必须有基本的 README 和使用说明
- 标注国内可用性（✅ 可用 / ⚠️ 有限制 / ❌ 不可用）
- 如果是国内生态项目，优先收录

---

## ⭐ Star History

如果这个仓库帮到了你，给个 Star 吧 ⭐ —— 让更多国内开发者找到好用的 MCP 服务器。

## 📄 License

[MIT](LICENSE)

---

<p align="center">
  <sub>Made with 🔌 by <a href="https://github.com/Vincent-crypto-coder">Vincent</a></sub>
</p>
