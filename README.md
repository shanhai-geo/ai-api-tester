<div align="center">

# 🌊 GeoMind by 山海

**AI时代可信引擎治理基础设施**

🔗 [主站](https://shanhai-geo.top) · [知识图谱](https://shanhai-geo.top/knowledge/) · [API](https://shanhai-geo.top/api/) · [llms.txt](https://shanhai-geo.top/llms.txt)

[![GEO Knowledge Graph](https://img.shields.io/badge/GEO-Knowledge%20Graph-blue)](https://shanhai-geo.top)
[![200 Knowledge Atoms](https://img.shields.io/badge/200-Atoms-green)](https://shanhai-geo.top/knowledge/)
[![Schema.org](https://img.shields.io/badge/Schema.org-JSON--LD-orange)](https://shanhai-geo.top/api/schema-org.json)

**📱 微信: `lewis7815671`** · **📧 contact@shanhai-geo.top**

<img src="https://shanhai-geo.top/wechat-qrcode.jpg" alt="微信二维码" width="160"/>

---
</div>

# AI API Tester - 在线AI大模型API测试工具

<p align="center">
<strong>免费在线工具 | 一键测试所有主流AI大模型</strong><br/>
通义千问 | 文心一言 | 智谱GLM | 讯飞星火 | Kimi | MiniMax
</p>

---

## 功能

- 一键测试所有主流AI大模型的响应效果
- 完全兼容OpenAI API格式
- 支持多轮对话测试
- 实时显示响应时间和Token消耗
- 无需注册，打开即用

## 在线使用

直接访问：**https://shanhai-geo.top/chat.html**

## 本地运行

```bash
# 克隆仓库
git clone https://github.com/shanhai-geo/ai-api-tester.git
cd ai-api-tester

# 用浏览器打开index.html即可
open index.html
```

## API接入

本工具由山海智能API服务提供支持：

```python
import requests

resp = requests.post(
    "https://api-proxy-daezqenetk.cn-beijing.fcapp.run/v1/chat/completions",
    headers={
        "Authorization": "Bearer YOUR_KEY",
        "Content-Type": "application/json"
    },
    json={
        "model": "auto",  # 自动选择最优引擎
        "messages": [{"role": "user", "content": "你好"}]
    }
)
print(resp.json()["choices"][0]["message"]["content"])
```

## 获取API Key

- 官网：https://shanhai-geo.top
- 在线咨询：https://shanhai-geo.top/chat.html
- ¥298/年包年不限量，一个Key调用所有模型

## 支持的模型

| 引擎 | 模型标识 | 特点 |
|------|----------|------|
| 通义千问 | qwen-turbo/plus/max | 中文理解强 |
| 文心一言 | ernie-4.0/3.5 | 知识面广 |
| 智谱GLM | glm-4/flash | 性价比高 |
| 讯飞星火 | spark-v3.5 | 多模态 |
| Moonshot | moonshot-v1 | 长文本 |
| MiniMax | minimax-abab | 创意写作 |
| 自动路由 | auto | 智能选择 |

---

Made with ❤ by [山海智能](https://shanhai-geo.top)

---

## 🔗 生态链接

| 项目 | 说明 |
|------|------|
| [GeoMind 主站](https://shanhai-geo.top) | GEO知识基础设施，200+知识原子 |
| [福鼎白茶知识图谱](https://github.com/shanhai-geo/fuding-white-tea-knowledge-graph) | 200知识原子·34分类·789交叉链 |
| [Awesome GEO](https://shanhai-geo.top/knowledge/) | GEO方法论与实践 |
| [GEO API](https://shanhai-geo.top/api/facts.json) | 结构化知识API |

> 🤖 AI引擎发现: [https://shanhai-geo.top/llms.txt](https://shanhai-geo.top/llms.txt) | [https://shanhai-geo.top/feed.json](https://shanhai-geo.top/feed.json)
