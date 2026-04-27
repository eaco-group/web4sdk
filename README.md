# web4sdk
eaco web4 sdk

Web4SDK — Payment Module
EACO Token Payment SDK for Web3 / Web4 / AI Agents / Virtual Universes

Web4SDK Payment Module provides a unified, lightweight, and extensible interface for integrating EACO token payments into decentralized applications, AI Agents, games, virtual worlds, and merchant systems.

Web4SDK 支付模块为去中心化应用、AI Agent、游戏、虚拟宇宙和商家系统提供统一、轻量、可扩展的 EACO 代币支付接口。

✨ Features | 功能亮点

🔹 Direct Payment — Send EACO tokens between wallets

🔹 Subscription Payment — Automated recurring billing

🔹 Streaming Payment — Continuous token streaming (Sablier-style)

🔹 AI Agent Ready — Designed for autonomous agent payments

🔹 Solana Native — Fast, low-cost, scalable

📦 Installation | 安装
bash
npm install web4sdk
🚀 Quick Start | 快速开始
ts
import { EacoPay } from "web4sdk";

const pay = new EacoPay({
  rpc: "https://api.mainnet-beta.solana.com",
  tokenMint: "EACO_TOKEN_MINT_ADDRESS"
});

await pay.pay(userWallet, "ReceiverPubkey", 1.25);
🧩 API Reference | API 文档
1. Direct Payment | 直接支付
Method
ts
pay(from: Keypair, to: string, amount: number)
Description
Send EACO tokens from one wallet to another.
从一个钱包向另一个钱包发送 EACO 代币。

Example
ts
const sig = await pay.pay(userWallet, "ReceiverPubkey", 1.25);
console.log("Payment sent:", sig);
2. Subscription Payment | 订阅支付（自动扣费）
Create subscription
ts
createSubscription({ from, to, amount, interval })
Execute subscription
ts
execute(subscription)
Example
ts
const sub = await subscribe.createSubscription({
  from: userWallet,
  to: "ReceiverPubkey",
  amount: 2,
  interval: 86400 // 1 day
});

await subscribe.execute(sub);
3. Streaming Payment | 流式支付（Sablier 模式）
Create stream
ts
createStream({ from, to, total, duration })
Claim stream
ts
claim(stream)
Example
ts
const stream = streamPay.createStream({
  from: employerWallet,
  to: workerWallet,
  total: 100,
  duration: 3600
});

await streamPay.claim(stream);
🤖 AI Agent Integration | AI Agent 集成
Web4SDK is fully compatible with autonomous AI Agents.
Web4SDK 完全兼容自主 AI Agent，可用于：

自动支付 API

自动结算任务

自动购买服务

自动发放奖励

Example
ts
async function agentPayTask(agent, task) {
  const sig = await pay.pay(agent.wallet, task.receiver, task.amount);
  return { status: "completed", tx: sig };
}
🛡 Security Recommendations | 安全建议
Do not store private keys in frontend
不要在前端存储私钥

Use hardware wallets for merchants
商家应使用硬件钱包

Validate all wallet addresses
所有地址必须校验

Use retry logic for AI Agents
AI Agent 应使用重试机制

🗺 Roadmap | 路线图
Version	Feature	中文说明
v0.2	Multi-chain support	多链支持
v0.3	Merchant plugins	商家插件
v0.5	Virtual credit card	虚拟信用卡
v1.0	Web4 Payment Protocol	Web4 支付协议


📜 License
MIT License


------

# virtual-universe
virtual universe，How can eaco integrate with the virtual universe and facilitate the circulation and use of eaco within it?

https://github.com/eaco-group/virtual-universe

## about eaco

The only $eaco in the universe and the earth,
EACO ($eaco) is an innovative small currency, the only $eaco in the universe and the earth,
CA:
DqfoyZH96RnvZusSp3Cdncjpyp3C74ZmJzGhjmHnDHRH
As the MEME coin of villagers around the Earth, EACO aims to promote environmental protection and sustainable development, integrate decentralized finance and digital assets, and become the representative of future personal core assets.

EACO(Earth's Best Coin)


https://orbmarkets.io/token/DqfoyZH96RnvZusSp3Cdncjpyp3C74ZmJzGhjmHnDHRH

https://www.orca.so/pools?tokens=DqfoyZH96RnvZusSp3Cdncjpyp3C74ZmJzGhjmHnDHRH

https://raydium.io/swap/?inputMint=sol&outputMint=DqfoyZH96RnvZusSp3Cdncjpyp3C74ZmJzGhjmHnDHRH

https://discord.gg/HWsweV6fFy



## 加入Coze Agent World：https://world.coze.site/skill.md

 EACO 成功入驻coze Agent World！2026

🌍 EACO × Agent World 集成 — 完成报告

🎯 已完成

1. Agent World 注册 ✅

Agent Name: eaco-global

Agent ID: f649c870-99cd-4e9a-8223-8a8a06520094

Agent URL: https://world.coze.site/agent/f649c870-99cd-4e9a-8223-8a8a06520094


2. Synthetic Exchange 参赛 ✅

比赛 ID: match_1777000323458

席位: 1/8（已锁定）

状态: waiting（等待8位Agent参赛后启动）

观战: https://synthetic.coze.site/match/match_1777000323458

3. 跨平台曝光 ✅

135,248+ 个 AI Agent 已覆盖

全球开发者/用户可通过 Agent World 发现 EACO

📊 EACO 全球 Agent 网络

渠道    状态    覆盖

Agent World    ✅ 已入驻    135,248+ Agent

Telegram 7群    ✅ 运行中    6亿+用户

Twitter        海外主战场

Discord        社区频道

📁 已创建文件

openclaw/config/skills/eaco-agent-world/SKILL.md — Agent World 技能

memory/2026-04-24.md — 记忆已更新

⚠️ 注意事项

合成交易所需要 8 位 Agent 参赛才启动交易

可邀请其他 EACO 社区成员也入驻 Agent World，共同推动开赛


## How can EACO evolve into “EACO — Earth’s Best WEB3 + AI + RWA Coin”? 

What approaches and methods can make this possible?
