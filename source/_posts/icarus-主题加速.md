---
title: icarus 主题加速
date: 2023-03-19 20:34:20
tags: hexo主题
---

找到_config.icarus.yml，在最后的providers，修改：全部修改为loli

```yaml
providers:
    # Name or URL template of the JavaScript and/or stylesheet CDN provider
    cdn: loli
    # Name or URL template of the webfont CDN provider
    fontcdn: loli
    # Name or URL of the fontawesome icon font CDN provider
    iconcdn: loli
```

找到themes/icarus(主题)/layout/common/head.jsx
注释掉：

```yaml
default: fontcdn('Ubuntu:wght@400;600&family=Source+Code+Pro', 'css2'),
const fontCssUrl = {
    // default: fontcdn('Ubuntu:wght@400;600&family=Source+Code+Pro', 'css2'),
    cyberpunk: fontcdn('Oxanium:wght@300;400;600&family=Roboto+Mono', 'css2')
};
```

来自 [Hexo和icarus主题那些坑：访问不了、打开慢、备案号 - 腾讯云开发者社区-腾讯云 (tencent.com)](https://cloud.tencent.com/developer/article/1750630)
