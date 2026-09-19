# 清漫 QINGMAN ANIME

一个「超现实主义拼贴 × 科技蓝图」风格的番剧导航站。纯白底、深蓝 #0033CC 主色，相框嵌套卡片，错位排版。

## 在线访问

- 线上站：https://kcndk3ao3jqd.aiforce.cloud/app/app_17ec9jccm7a
- 本仓库：https://gitee.com/xixikeshkkk/qingman

## 本地运行

单文件自包含，直接用浏览器打开 `index.html` 即可，无需构建。

```
index.html        # 整个站点（React + Tailwind + Framer Motion，全部 CDN）
assets/           # 封面图、数据、播放器配置
```

## 功能

- 首页轮播 + 分类推荐 + 排行榜
- 动漫库：类型/年代/标签筛选，全局实时搜索，分页
- 详情页：剧情简介、集数列表，点击集数本站原生播放
- 个人手记 / 观看者评价（数据存 Supabase，跨设备共享）

## 如何参与修改

1. 点右上角 **Fork** 到你自己的账号
2. 改本地文件（主要是 `index.html`）
3. 提交并推送，然后到本仓库发 **Pull Request**

## 部署说明

本仓库只是源码，线上站是独立发布的。PR 合并后需要管理员重新部署，线上才会更新——Gitee 改动不会自动同步到线上。

## 技术栈

- 原生 HTML + 内联 React (CDN) + Tailwind CDN + Framer Motion CDN
- Hash 路由：`#/`、`#/library`、`#/notes`、`#/rankings`、`#/reviews`、`#/anime/:id`、`#/anime/:id/play/:ep`
- 后端：Supabase（reviews / notes 两张表，匿名读写）

## License

仅作学习交流，番剧版权归原作者及发行方所有。
