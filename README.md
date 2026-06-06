# MSS-AI Perspective

**MSS (Meaning Supremacy System) AI 分析框架 — 意义审计操作系统**

> 不生成内容，审计内容。不优化参数，审计参数背后的热税。

![version](https://img.shields.io/badge/version-v18.10.28-blue)
![tools](https://img.shields.io/badge/tools-22-orange)
![pathologies](https://img.shields.io/badge/pathologies-6-red)
![license](https://img.shields.io/badge/license-MIT-green)

---

## 这是什么

MSS 是一个**跨领域诊断框架**，基于七条核心公理对 AI/商业/代码/组织进行系统性审计。

不是 prompt engineering，不是 agent framework，不是代码生成器。它是一个**意义审计操作系统**——检测逻辑病毒、量化热税浪费、诊断意义黑洞、执行矛盾升维。

## 能做什么

| 能力 | 工具 | 示例 |
|:---|:---|:---|
| 代码热税审计 | `mss_repo_scan.py` | 嵌套循环、空异常、逻辑病毒 |
| PowerShell 诊断 | `ps_verify.py verify` | 版本/模块/幽灵文件检测 |
| 幽灵文件检测 | `ps_verify.py phantom` | MFT残留 + minifilter阻断 |
| 组织韧性评估 | `org_resilience.py` | O_d/Φ/γ/M 四维评分 |
| 内容合规审计 | `content_compliance.py` | 无锚断言/伪科学/模因污染 |
| 缓存污染检测 | `cache_validator.py` | sys.modules + 跨版本审计 |
| 鬼打墙检测 | `mss_conversation_scan.py` | 两步触发矛盾信号 |
| 话语污染检测 | `mss_vdc_scan.py` | 伪归因/约束发明/修辞硬化 |
| 验证纪律校验 | `mss_vdp_scan.py` | V1-V6 六条操作纪律 |

## 六种可检测病理

```
#1 Junction 缺失/断裂     → SOP-001
#2 缓存寄生 V-007         → cache_validator
#3 POSIX 习惯硬套          → PowerShell 铁律
#4 会话伪沙盒             → cross-audit
#5 幽灵文件 (MFT残留)     → phantom --auto-clean
#6 Minifilter 路径阻断    → phantom --filter (A7: 可检测不可修复)
```

## 快速开始

```bash
# 环境检测
python scripts/ps_verify.py verify

# 代码扫描
python scripts/mss_repo_scan.py . --mode auto

# 幽灵文件检测
python scripts/ps_verify.py phantom <dir> --auto-clean

# 组织诊断
python scripts/org_resilience.py demo

# 内容审计
python scripts/content_compliance.py scan <dir>
```

**依赖**: Python 3.8+，零外部依赖 (仅 math + json + dataclasses)

## 七条公理 (L1 硬核基准)

| # | 公理 | 含义 |
|:---|:---|:---|
| A1 | 意义本体 | 意义是终极实在 |
| A2 | 信息切片 | 所有认知都是有限投影 |
| A3 | 终极热税 | 一切显化付出不可约代价 |
| A4 | 本底随机性 | 闭系统中涨落永存 |
| A5 | 规范场 | 自组织系统自发产生约束结构 |
| A6 | 矛盾升维 | 低维矛盾只通过升维解决 |
| A7 | 不可言说 | 有限符号系统无法穷尽意义根基 |

## 架构

```
mss-ai-perspective/
├── kernel/          # 不可变核 (公理守门员 + 扫描引擎)
├── scripts/         # 可变壳 (22 个 CLI 扫描器)
├── references/      # 知识文档 (只读)
└── .mss/logs/       # 运行时日志 (JSONL)
```

## 安装

```bash
# 下载 .skill 文件
# https://github.com/mysama1/mss-ai-perspective/releases/latest

# 或直接 clone
git clone https://github.com/mysama1/mss-ai-perspective.git
```

## A7 诚实边界

```
✅ Python 代码审计 (P0吞错 12/12 verified)
✅ PowerShell 诊断 (5条铁律)
✅ 文件系统病理检测 (6种)
✅ 组织/内容/话语分析
⚠️ 非 Python 语言 (JS/TS/Rust) — 不覆盖
⚠️ 运行时并发/锁检测 — 不覆盖
❌ Minifilter 修复 — 内核驱动, 用户态无解
```

## 版本链

v15.1 → v16.4 → v18.10.28 (150+ releases, 一日十版开发节奏)

## 许可证

MIT
