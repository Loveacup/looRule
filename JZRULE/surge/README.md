# Surge Rule Overlay

These files are designed for Surge `RULE-SET` references.

Each file contains only match rules, not policy names. The active Surge profile
decides the target policy:

```text
RULE-SET,https://raw.githubusercontent.com/Loveacup/looRule/main/JZRULE/surge/20-tools/productivity.list,"🧰 生产力工具","update-interval=86400"
```

Do not put local-only process paths, private LAN routes, or DoH egress IP locks
here. Those stay in the main Surge profile.

## Legacy Custom Migration

Root-level `Custom*.list` files are retained untouched for history and compatibility. Active Surge references should use these JZRULE files instead:

- `00-core/custom-direct.list` -> `🎯 全球直连`
- `00-core/intercept.list` -> `🛑 广告拦截`
- `30-region/hk.list` -> `🇭🇰 香港优选`
- `30-region/sg.list` -> `🇸🇬 新加坡优选`
- `30-region/jp.list` -> `🇯🇵 日本优选`
- `30-region/us.list` -> `🌎 北美核心`
- `00-core/proxy.list` -> `🚀 手动选择2`

`90-temp/custom-gfw.list` is no longer active; remaining proxy-only exceptions live in `00-core/proxy.list`.

Keep local-only process paths, DEVICE routes, and temporary household diagnostics in the main Surge profile, not in this repo.
