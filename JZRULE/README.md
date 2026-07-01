# JZRULE

Personal overlay rules for the YinXingHui Surge gateway.

This directory is the clean replacement layer for scattered legacy custom rules
in the repository root. Root-level files remain legacy compatibility sources.

Principles:

- Keep public upstream rules in blackmatrix7 / ACL4SSR.
- Put only personal decisions, local long-term overrides, and uncovered gaps here.
- Do not mix policies inside one rule file. Surge binds policy in the main config.
- Local network, DoH egress locks, and process-path rules stay in the Surge profile.

