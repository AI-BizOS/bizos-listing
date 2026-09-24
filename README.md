# BizOS Listing

An open Amazon Listing skill that works with or without BizOS Work. It drafts and audits titles, bullets, descriptions, Search Terms, A+ direction, and image briefs from evidence.

The skill follows two evidence paths:

1. **BizOS path:** when the user has connected and authorized relevant BizOS MCP tools, use their actual competitor, keyword, traffic, and review results. Record the source, scope, and observation date.
2. **Portable path:** otherwise use competitor ASINs, exports, and product facts provided by the user, plus public pages that the current host is allowed to read. Record what was actually checked. Public pages do not imply access to private sales, search volume, or conversion data.

Both paths produce the same evidence summary and requested Listing draft. Missing evidence reduces the strength of the conclusion; it never becomes invented data.

## Install

Copy [`skills/bizos-listing`](skills/bizos-listing) into an Agent Skills directory, or import that directory in BizOS Work through **Skills → Add Skill**. The skill ID is `bizos-listing`, distinct from BizOS Work's protected `bizos-amazon-listing` package, so the two can coexist.

An example request and illustrative response using fictional products are in [`examples/demo-brief.md`](examples/demo-brief.md) and [`examples/demo-output.md`](examples/demo-output.md). The skill does not install an MCP server, provide market data, or publish anything to Amazon. It uses only tools already available and authorized in the host.

## Scope

The public project contains the portable Listing workflow and evidence rules. BizOS MCP services, customer data, private market methods, official Skill signing, Agent orchestration, Computer Use, and Charts are outside this repository. Amazon policy changes by marketplace and category; before calling copy compliant, verify the current applicable official rules.

See [`CONTRIBUTING.md`](CONTRIBUTING.md) for contributions. Licensed under MIT.

---

## 中文说明

这是可独立使用的亚马逊 Listing Skill。已授权的 BizOS MCP 数据可用时优先用它找竞品、关键词和评论；没有接入 BizOS 时，使用用户提供的资料和当前宿主获准读取的公开页面。两条路径都要写清来源、日期与缺失字段，不能把公开页面推断成销量等私有指标。将 [`skills/bizos-listing`](skills/bizos-listing) 文件夹导入 BizOS Work，或放进其他支持 Agent Skills 的工具即可使用。
