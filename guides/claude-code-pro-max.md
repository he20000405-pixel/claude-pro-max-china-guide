---
title: "Claude Code 使用 Pro / Max：登录账号、会员额度与 API 计费边界"
description: "Claude Code 使用 Claude Pro 或 Max 会员的登录指南：用同一 Claude 账号认证，检查套餐、更新客户端、切换错误账号，并区分会员额度与 API 计费。"
permalink: /guides/claude-code-pro-max/
date_published: 2026-07-14
last_modified_at: 2026-08-05
breadcrumbs:
  - name: Claude 指南
    url: /
  - name: 专题
    url: /guides/
  - name: Claude Code 与 Pro / Max
    url: /guides/claude-code-pro-max/
faq:
  - question: "Claude Pro 和 Max 是否都能使用 Claude Code？"
    answer: "Anthropic 官方说明 Pro 与 Max 订阅者都可以使用 Claude Code，但可用模型、额度和功能以当前官方计划说明及账号实际显示为准。"
  - question: "Claude Code 和网页 Claude 是否共享会员使用量？"
    answer: "官方说明 Pro 或 Max 计划的使用量会在 Claude 应用与 Claude Code 之间共享，任务长度、项目规模和模型都会影响消耗。"
  - question: "Claude 会员是否等于 API 额度？"
    answer: "不是。Pro / Max 会员与 Anthropic Console/API 是不同计费体系。本指南只讨论会员订阅，不提供 API 额度或 API 充值。"
---

# Claude Code 使用 Pro / Max

<p class="lead">先在 Claude 网页确认 Pro 或 Max 仍有效，再让 Claude Code 登录同一个账号。若终端正在使用 API Key，继续操作可能进入独立计费，而不是消耗会员用量。</p>

## 开始前先确认三件事

1. 在 Claude 网页打开 `Settings > Billing`，确认计划显示 Pro、Max 5x 或 Max 20x。
2. 记录网页当前登录邮箱，不要只看头像或昵称。
3. 如果系统配置了 `ANTHROPIC_API_KEY`，先停止登录排查。Anthropic 官方说明，该变量可能让 Claude Code优先使用 API Key 并产生独立费用。

如果网页本身显示 Free，请先处理[已付款仍显示 Free](../claude-paid-but-still-free/)或[续费失败](../claude-renewal-failed-back-to-free/)，不要在终端反复登录。

## 官方支持边界

Anthropic 官方说明 Pro 与 Max 订阅都可用于 Claude Code。Pro 适合较轻量的代码任务，Max 提供更高使用量；具体模型访问和限制会随官方计划调整。

| 套餐 | Claude Code 适用判断 |
| --- | --- |
| Pro | 轻量代码任务、小型项目、先验证工作流 |
| Max 5x | 日常持续使用、较大项目、Pro 经常触达限制 |
| Max 20x | Max 5x 仍不足的重度工程工作流 |

不要用固定 prompt 数量作为保证。项目规模、上下文、文件、模型和自动执行设置都会影响使用量。

## 登录正确的会员账号

首次运行时，按 Claude Code 提示通过浏览器登录，选择与 Claude Pro / Max 相同的账号。浏览器授权完成后回到终端，确认没有再次出现登录提示，然后检查：

- 浏览器登录邮箱与 Claude Billing 中的订阅邮箱一致；
- Claude Code 没有连接到另一个免费账号；
- 当前账号的 `Settings > Billing` 显示有效 Pro 或 Max；
- 网页 Claude 与终端使用的是同一身份。

## 登录错账号时的处理顺序

Anthropic 官方给出的重新登录顺序是：

```text
/logout
claude update
```

执行 `/logout` 后运行 `claude update`，完全关闭并重新打开终端，再运行 `claude`。出现账号选择时，使用与网页 Billing 相同的 Claude 账号。

预期结果是终端进入 Claude Code 会话，并使用订阅账号。如果仍显示另一个账号、API 计费或登录循环，请停止重复授权，保存终端提示和当前版本，再联系 Anthropic 支持。

## 会员额度与 API 计费不是一回事

Claude Pro / Max 是个人会员订阅；Anthropic Console/API 是另一套计费体系。本文不提供 API 充值或 API 使用教程。

使用 Claude Code 时应确认当前选择的是会员账号。如果终端提示切换到额外付费或其他计费方式，先阅读提示并确认自己的目标，不要默认同意产生另一套费用。

如果只希望使用会员包含的额度，应拒绝额外计费选项。本文不提供 API Key、API 额度或自动充值设置教程。

## Claude Code 显示无会员时怎么排查

1. 回 Claude 网页查看 `Settings > Billing`；
2. 确认订阅没有到期、续费失败或被降级；
3. 确认终端登录的是同一个邮箱；
4. 更新 Claude Code；
5. 完全退出后重新登录；
6. 如果官方已成功扣款但账号仍为 Free，进入[已付款仍显示 Free](../claude-paid-but-still-free/)；
7. 如果续费失败，进入[续费失败专题](../claude-renewal-failed-back-to-free/)。

## 完成验收

下面四项同时满足，才算排查完成：

- 网页 `Settings > Billing` 显示有效 Pro 或 Max；
- 网页与 Claude Code 使用同一个登录账号；
- 终端可以正常进入 Claude Code 会话；
- 没有在不知情的情况下切换到 API Key 或额外计费。

## 订阅选择与国内付款

先根据真实限制记录选择套餐，不因 Claude Code 的单次大型任务直接购买最高档。需要给自己的 Claude 账号开通 Pro，或咨询 Max 5x/20x 时，可访问 <https://chonggrok.com/claude>。

ChongGrok 不需要密码，由客服确认 User ID 和目标套餐后协助官方付款；完成后仍需回 Claude Billing 和 Claude Code 验收。

## 官方来源

- [Anthropic Help：Using Claude Code with Pro or Max](https://support.anthropic.com/en/articles/11145838-using-claude-code-with-your-max-plan)
- [Anthropic plans and pricing](https://www.anthropic.com/pricing?subjects=claude&type=product)
- [Anthropic Help：Paid Plan Billing FAQs](https://support.anthropic.com/en/articles/8325618-where-can-i-find-the-receipt-for-my-claude-subscription)

{% include faq.html %}
