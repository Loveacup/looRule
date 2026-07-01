# JZRULE Manifest

| File | Default Surge Policy | Purpose |
| --- | --- | --- |
| `surge/00-core/direct.list` | `DIRECT` / `🎯 全球直连` | Stable direct overrides |
| `surge/00-core/intercept.list` | `🛑 广告拦截` | Migrated legacy `CustomIntercept.list` without touching the root file |
| `surge/00-core/custom-direct.list` | `🎯 全球直连` | Migrated legacy `CustomDirect.list` without touching the root file |
| `surge/10-ai/core.list` | `✴️ Ai` | Strict Claude Code / Codex / Gemini local gaps |
| `surge/20-dev/devtools.list` | `🚀 手动选择1` or future DevTools | Development helper domains |
| `surge/20-tools/productivity.list` | `🧰 生产力工具` | Generic AI, creative, and productivity tools |
| `surge/30-region/jp.list` | `🇯🇵 日本优选` | Japan-only regional exceptions |
| `surge/30-region/tw.list` | `🇼🇸 台湾优选` | Taiwan regional exceptions |
| `surge/30-region/sg.list` | `🇸🇬 新加坡优选` | Migrated legacy `CustomSingapore.list` without touching the root file |
| `surge/30-region/hk.list` | `🇭🇰 香港优选` | Migrated legacy `CustomHongKong.list` without touching the root file |
| `surge/30-region/us.list` | `🌎 北美核心` | North-America-specific exceptions |
| `surge/40-app/makerworld-direct.list` | `DIRECT` | MakerWorld China/domestic endpoints |
| `surge/40-app/makerworld-global.list` | `🌐 全球常规可用` | MakerWorld international endpoints |
| `surge/90-temp/custom-gfw.list` | `🚀 手动选择2` | Migrated legacy `CustomGFWList.list`; keep here until semantic split |

Last updated: 2026-07-01.

Migration note: root `Custom*.list` files are retained untouched for compatibility/history; active Surge references should use `JZRULE/surge/...`.

