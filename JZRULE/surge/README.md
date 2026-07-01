# Surge Rule Overlay

These files are designed for Surge `RULE-SET` references.

Each file contains only match rules, not policy names. The active Surge profile
decides the target policy:

```text
RULE-SET,https://raw.githubusercontent.com/Loveacup/looRule/main/JZRULE/surge/20-tools/productivity.list,"🧰 生产力工具","update-interval=86400"
```

Do not put local-only process paths, private LAN routes, or DoH egress IP locks
here. Those stay in the main Surge profile.

