---
layout: page
title: 视频文字版目录
description: 智财小站全部公开视频的文字版目录，按主题归类。每页含校对逐字稿、发布日期、适用前提、数据来源与风险声明。
permalink: /episodes/
---

全部公开视频的文字版，按主题归类，按日期倒序。每页都保留发布日期、适用前提、来源和风险声明；正文与最终视频、中文字幕一致。

{% assign groups = site.episodes | group_by: "topic" %}
{% for g in groups %}
## {{ g.name }}

{% assign eps = g.items | sort: "upload_date" | reverse %}
{% for ep in eps %}- {{ ep.upload_date }} · [{{ ep.title }}]({{ ep.url | relative_url }})
{% endfor %}
{% endfor %}

<p class="note risk">候选池不是买入清单。本站不提供个性化投资建议，也不承诺任何收益。</p>
