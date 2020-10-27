# Ban Bad Websites

[GitHub](https://github.com/Phuker/BanBadWebsites) | [Greasy Fork](https://greasyfork.org/zh-CN/scripts/389721)

又一个屏蔽中文世界爬虫、机器翻译等 SEO 垃圾网站的浏览器用户脚本。

本项目特色：

- 不是特定网站的针对性脚本，而是处理所有网页的所有超链接。
- 支持高亮超链接，让用户在点击之前就意识到，哪些链接指向垃圾网站。

垃圾网站黑名单类型：

- SEO 爬虫采集站，例如爬 Stack Overflow 并进行机器翻译的网站
- 博彩网站，被搜索引擎搜到时看起来是正常网站，点击后进入博彩网站
- 低质量博客、下载站

此脚本会遍历所有的 `<a>` 标签，查询域名和 `URL` 前缀黑名单，识别指向垃圾网站的超链接。根据用户配置，可以高亮标记/屏蔽/删除识别出的超链接。

## 效果

默认设置：

![default](./screenshots/screenshot1.png)

## 安装

## 设置

编辑源代码 `Start User Config` 和 `End User config` 之间的代码，可以启动/关闭以下功能。

- `option_highlight_link`：突出显示目标超链接，改变链接的外观、指针样式等
- `option_disable_link`：使目标超链接无法点击。不推荐，因为垃圾网站有时候还有一定参考价值，必要时可能仍然需要点击访问
- `option_remove_link`：隐藏目标超链接。不推荐，因为此脚本不是特定网站的针对性脚本，无法完美删除目标超链接，可能会导致网页显示错乱

## 初始黑名单来源参考

- [https://www.v2ex.com/t/597368](https://www.v2ex.com/t/597368)
- [https://www.v2ex.com/t/593519](https://www.v2ex.com/t/593519)
- [https://greasyfork.org/zh-CN/scripts/389270-翻译垃圾再利用](https://greasyfork.org/zh-CN/scripts/389270-翻译垃圾再利用)
- [https://github.com/liubiantao/uBlacklist-Websites](https://github.com/liubiantao/uBlacklist-Websites)

## 类似项目推荐

- [https://greasyfork.org/zh-CN/scripts/389270-翻译垃圾再利用](https://greasyfork.org/zh-CN/scripts/389270-翻译垃圾再利用)
- [uBlacklist 扩展程序](https://chrome.google.com/webstore/detail/ublacklist/pncfbmialoiaghdehhbnbhkkgmjanfhe) + [liubiantao/uBlacklist-Websites 垃圾网站列表](https://github.com/liubiantao/uBlacklist-Websites)

## License

This repo is licensed under the **GNU General Public License v3.0**
