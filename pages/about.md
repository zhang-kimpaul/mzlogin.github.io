---
layout: page
title: About
description: coding and noting
keywords: zhang jinbao
comments: true
menu: 关于
permalink: /about/
---

I'm a second year undergraduate student from [School of EECS](https://esist.ustc.edu.cn/), [Peking University](https://www.ustc.edu.cn/). My research interest includes computer vision ,aiming at 3d object detection.



[Email](mailto:zjb19990529@mail.ustc.edu.cn) 


## 联系

<ul>
{% for website in site.data.social %}
<li>{{website.sitename }}：<a href="{{ website.url }}" target="_blank">@{{ website.name }}</a></li>
{% endfor %}
{% if site.url contains 'mazhuang.org' %}
<li>
微信公众号：<br />
<img style="height:192px;width:192px;border:1px solid lightgrey;" src="{{ site.url }}/assets/images/qrcode.jpg" alt="闷骚的程序员" />
</li>
{% endif %}
</ul>


## Skill Keywords

{% for skill in site.data.skills %}
### {{ skill.name }}
<div class="btn-inline">
{% for keyword in skill.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
