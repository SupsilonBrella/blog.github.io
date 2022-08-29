# 如何使用SUpsilon网站访客统计系统

## 这是一篇有关SUpsilon访问统计系统（v1.4.4）的使用指南（应用于Wikidot）

源文件位于这里：http://www.brella.top/supsilon/supsilon-access-system.js

这玩意是我本年度写过第二长的代码，Bug一堆~

**版本仍为测试版，数据显示不稳定**

SUpsilon访问统计系统能够让你直观地看见你网站或页面的总访客人数、总访问次数以及单页面的访问次数，现在我们开始使用吧！

1.你需要将SUpsilon系统安装到你的网站上（至少在主页有一个系统的安装），在你的网站的任何想要显示相关数据的地方输入以下字段：
```toml
[[html]]
<script async src="http://www.brella.top/supsilon/supsilon-access-system.js">
</script>
[[/html]]
```

2.当系统安装完毕时，它便已经开始工作了，你只需要在你想要显示网站相关数据的地方安装SUpsilon标签（这些标签必须和SUpsilon系统本源在一个页面中）。
**在你想要显示网站总访问量的地方输入以下字段：**

```toml
[[html]]
站点总访问量<span id="supsilon_value_site_pv"></span>次
[[/html]]
```

**在你想要显示网站总访客人数的地方输入以下字段：**

```toml
[[html]]
站点总访客人数<span id="supsilon_value_site_uv"></span>人次
[[/html]]
```

**在你想要显示网站总访客人数的地方输入以下字段：**

```toml
[[html]]
本页面总访问量<span id="supsilon_value_page_pv"></span>次
[[/html]]
```

{{< admonition tip >}}
请注意！标签必须和SUpsilon系统本源在同一个页面中
{{< /admonition >}}

**如果你嫌以上操作过于麻烦，可以直接使用下面的代码**

```toml

[[html]]
<script async src="http://www.brella.top/supsilon/supsilon-access-system.js">
</script>

本站总访问量<span id="supsilon_value_site_pv"></span>次
本站访客数<span id="supsilon_value_site_uv"></span>人次
本文总阅读量<span id="supsilon_value_page_pv"></span>次
[[/html]]

```



