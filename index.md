---
layout: default
title: 智财小站公开文字资料库
description: 美股趋势交易、AI 辅助筛选、风险控制和周末市场快报的可检索文字版，包含校对后的公开视频逐字稿与来源。
---

# 美股趋势交易，留下能检索、能核对的文字

智财小站用中文讨论美股趋势交易、AI 辅助筛选、仓位与止损，也会整理市场环境、宏观事件和长期 ETF 的思考。这个网站把公开视频转成校对后的文字，保留发布日期、适用前提和来源，方便读者查找，也方便搜索引擎和聊天机器人理解原意。

[前往智财小站 YouTube 频道]({{ site.youtube_channel }}){:.primary-link}

## 这里提供什么

- **公开逐字稿**：与最终视频和中文字幕保持一致。
- **简要回答**：先给结论，再写适用条件和原因。
- **方法页**：解释趋势、入场、止损、仓位和 AI 各自负责什么。
- **来源与日期**：行情和新闻都标注时间；无法核实的内容不会写成事实。

## 方法与节目

- [趋势交易、AI 与风险控制]({{ '/trend-trading/' | relative_url }})
- [美股周末快报如何使用新闻]({{ '/weekend-briefing/' | relative_url }})
- [关于作者、资料和风险声明]({{ '/about/' | relative_url }})

## 公开视频文字版

{% assign sorted_episodes = site.episodes | sort: "upload_date" | reverse %}
<div class="episode-list">
{% for ep in sorted_episodes %}
  <article class="episode-card">
    <p class="eyebrow">{{ ep.format }} · {{ ep.upload_date }}</p>
    <h2><a href="{{ ep.url | relative_url }}">{{ ep.title }}</a></h2>
    <p>{{ ep.description }}</p>
  </article>
{% endfor %}
</div>

<p class="note risk">候选池不是买入清单。本站不提供个性化投资建议，也不承诺任何收益。</p>
