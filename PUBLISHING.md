# Claude 知识库发布与收录记录

## 仓库与 Pages

- GitHub：`https://github.com/he20000405-pixel/claude-pro-max-china-guide`
- Pages：`https://he20000405-pixel.github.io/claude-pro-max-china-guide/`
- 部署：`Settings → Pages → Build and deployment → Source` 选择 `GitHub Actions`，由仓库内发布前检查工作流发布 `main` 的合格产物，不使用分支直接发布。

按 [发布前检查说明](.github/PUBLISHING-CHECKS.md) 确认 `github-pages` 部署环境仅允许 `main`。工作流依次执行 `verify` → `release-ready` → `deploy`；`release-ready` 是无权限哨兵任务，依赖 `verify` 成功。PR 和 `ci-check` 测试分支只验收，不发布。只有 `main` 的正常检查通过后才部署同一次运行已检查的产物；检查失败时不执行发布，线上保留上一次成功版本。

## 发布后检查

先在 `Actions` 确认本次 `main` 的三个任务均成功，再检查公开页面；不要把推送成功或单独的检查成功视为已上线。

1. 首页、`/guides/`、`/en/`、7 个专题、`/robots.txt`、`/llms.txt` 和 `/sitemap.xml` 返回 200。
2. `sitemap.xml` 包含首页、英文入口和全部专题。
3. 手机端导航、标题和表格无横向页面溢出。
4. 社交预览图为 1200×630，不使用 Anthropic 官方 Logo。
5. 商家服务链接使用 `https://chonggrok.com/claude`，仅说明自有账号个人 Pro 月度与人工 iOS 内购；Max 官方套餐知识与商家服务分开，不引导联系 ChongGrok 办理 Max。
6. 桌面及移动端页头、页尾保留原导航，并能进入 `https://guides.chonggrok.com/` 指南门户。

## 搜索引擎

- Google Search Console：在根站属性提交 Claude sitemap，并仅请求首页、专题目录和英文入口一次。
- Bing Webmaster Tools：在根站属性提交 Claude sitemap，并仅提交同三个重点 URL 一次。
- 不重复提交 ChatGPT 或 Grok 的既有页面。

## 截图规则

当前只保留源码隐藏占位。获得清晰真实素材后，先遮蔽邮箱、User ID、订单号、付款信息和其他账号数据，再公开插图。

