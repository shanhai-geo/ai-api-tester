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

直接访问：**https://shanhai-geo.github.io/chat.html**

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

- 官网：https://shanhai-geo.github.io
- 在线咨询：https://shanhai-geo.github.io/chat.html
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

Made with ❤ by [山海智能](https://shanhai-geo.github.io)
