# 小红书-飞书云文档外观隐私政策

更新日期：2026 年 10 月 28 日

适用产品：小红书-飞书云文档外观，Microsoft Edge 扩展 0.1.0，内置飞书外观脚本 0.12.5。

本扩展是独立、非官方的网页外观工具，与小红书、飞书及其权利人无关联。

## 1. 用途与页面内的数据处理

本扩展在小红书桌面网页版提供文档式导航、列表和阅读界面。
为实现这些功能，扩展会在当前页面中读取和处理网站已经加载的内容，
例如笔记标题、作者昵称、封面地址、笔记链接及标识、互动数量，以及详情和评论中的作者关系。
扩展借用原生列表组件的数据和加载、刷新、详情打开回调；原生评论及其交互由小红书网站提供。

这些页面内容仅用于本地界面呈现和原生交互，可能暂时保留在当前页面的内存或 DOM 中。
扩展不会将笔记、评论、作者资料或浏览记录写入扩展的持久设置存储，
也不会将这些数据上传至开发者服务器。

本扩展不提供收集密码、登录 Cookie 或私信的功能。
需要登录时，用户通过小红书原生登录界面完成登录；扩展不接收登录凭据。

## 2. 本地保存的设置

扩展使用 `chrome.storage.local`，只持久保存以下三个外观设置：

| 设置 | 用途 |
| --- | --- |
| `xhs-lark-enabled` | 是否启用皮肤 |
| `xhs-lark-list-mode` | 首页使用纯文字或图文列表 |
| `xhs-lark-search-list-mode` | 搜索结果使用纯文字或图文列表 |

设置在同一浏览器配置中的小红书标签页之间保持一致。
本扩展不使用 `chrome.storage.sync`，也不将这些设置上传至开发者服务器。
本扩展不读取或迁移 Tampermonkey 的脚本设置。

## 3. 网络通信与第三方

本扩展没有开发者数据接收服务器、广告、统计或遥测功能。
扩展自身不会为收集页面内容而调用数据上传接口，也不会出售用户数据、
将数据用于与网页外观功能无关的目的，或用于信用评估及贷款用途。

小红书网站及其媒体服务仍会按网站原有方式发起网络请求。
用户主动使用搜索、加载笔记、登录或发表评论时，相关交互仍由小红书处理。
这些原生站点行为受相应服务的隐私政策约束。

扩展执行所需的 JavaScript 和样式随安装包提供，不从远程服务器加载额外的扩展可执行代码。

## 4. 权限与控制

扩展仅申请 `storage` 权限，内容脚本仅匹配以下主站地址：

- `https://www.xiaohongshu.com/*`
- `https://xiaohongshu.com/*`

扩展不申请浏览历史或 Cookie 权限。
用户可以在扩展弹窗中关闭皮肤或调整列表模式，也可以在 Edge 扩展管理页停用或移除扩展。
直接从浏览器管理页停用扩展后，刷新已打开的小红书页面即可停止该页面中已注入的皮肤。

## 5. 联系与政策更新

开发者支持：<https://github.com/yangyq081/xiaohongshu-lark-docs/issues>

如果未来版本的数据处理方式发生变化，本政策将相应更新，并注明新的更新日期。

---

# Privacy Policy for Xiaohongshu - Lark Docs Appearance

Last updated: October 28, 2026

Applies to: 小红书-飞书云文档外观, Microsoft Edge extension 0.1.0, containing appearance script 0.12.5.

This is an independent, unofficial appearance extension. It is not affiliated with Xiaohongshu, Lark, or their respective owners.

## 1. Purpose and local page processing

The extension provides document-style navigation, note lists and a reading layout on the desktop Xiaohongshu website.
To provide these features, it reads and processes content already loaded by the website in the current page,
such as note titles, author nicknames, cover image addresses, note links and identifiers, interaction counts,
and author relationships in note details and comments.
It uses the native feed component's data and existing loading, refresh and detail-opening callbacks.
Native comments and their interactions are provided by Xiaohongshu.

Page content is used locally for presentation and native interactions and may be temporarily retained in page memory or the DOM.
The extension does not persist notes, comments, author profiles or browsing records in extension settings storage,
and does not upload this information to developer-operated servers.

The extension does not provide password, login-cookie or private-message collection features.
Users sign in through Xiaohongshu's native login interface; the extension does not receive login credentials.

## 2. Locally stored preferences

The extension uses `chrome.storage.local` to persist only three appearance preferences:

| Setting | Purpose |
| --- | --- |
| `xhs-lark-enabled` | Whether the skin is enabled |
| `xhs-lark-list-mode` | Text-only or visual homepage lists |
| `xhs-lark-search-list-mode` | Text-only or visual search-results lists |

Preferences remain consistent across Xiaohongshu tabs in the same browser profile.
The extension does not use `chrome.storage.sync` or upload these preferences to developer-operated servers.
It does not read or migrate Tampermonkey script settings.

## 3. Network communication and third parties

The extension has no developer-operated data collection server, advertising, analytics or telemetry.
It does not invoke data-upload endpoints to collect page content, sell user data,
use data for purposes unrelated to its appearance features, or use data for creditworthiness or lending purposes.

Xiaohongshu and its media services continue making their normal website requests.
Interactions initiated by users, such as searching, loading notes, signing in or posting comments, remain handled by Xiaohongshu.
These native website activities are governed by the relevant service's privacy policy.

The extension's JavaScript and styles are included in the installation package.
It does not load additional executable extension code from remote servers.

## 4. Permissions and user controls

The extension requests only the `storage` permission.
Content scripts match only these website addresses:

- `https://www.xiaohongshu.com/*`
- `https://xiaohongshu.com/*`

The extension does not request browser-history or cookie permissions.
Users can switch the skin off or change list modes in the popup, or disable or remove the extension in Edge's extension manager.
After disabling the extension through the browser's extension manager, reload open Xiaohongshu pages to stop the skin already injected into those pages.

## 5. Contact and policy updates

Developer support: <https://github.com/yangyq081/xiaohongshu-lark-docs/issues>

If a future version changes how data is processed, this policy will be updated with a new revision date.
