---
title: "Claude 已付款仍显示 Free：Billing 与账号归属排查"
description: "Claude Pro 或 Max 已扣款但仍显示 Free 时，检查官方收据、Settings > Billing、原登录邮箱、网页或应用商店购买入口，以及 ChongGrok 订单和 User ID。"
permalink: /guides/claude-paid-but-still-free/
date_published: 2026-07-14
last_modified_at: 2026-07-14
breadcrumbs:
  - name: Claude 指南
    url: /
  - name: 专题
    url: /guides/
  - name: 已付款仍显示 Free
    url: /guides/claude-paid-but-still-free/
faq:
  - question: "Claude 已扣款但显示 Free，是否应该重新购买？"
    answer: "不应该立即重新购买。先确认扣款是否最终入账、是否收到 Anthropic 或应用商店收据、当前登录邮箱以及 Settings > Billing 的状态。"
  - question: "Anthropic 官方建议先检查什么？"
    answer: "官方 Billing FAQ 建议检查是否登录了其他邮箱，以及付款方式是否失败导致账号被降级；可在 Settings > Billing 查看最近付款状态。"
  - question: "ChongGrok 订单未生效应该提供什么？"
    answer: "向客服提供订单号、目标套餐、提交时间、脱敏后的目标账号信息和 Billing 状态，不要再次提交密码、验证码或恢复码。"
---

# Claude 已付款但仍显示 Free

<p class="lead">不要因为页面没有立即显示 Pro 或 Max 就再次付款。先确认“银行扣款”“官方订单成功”和“当前账号获得权益”三个环节是否属于同一笔交易和同一个账号。</p>

## 第一步：确认是否为最终成功扣款

| 证据 | 能说明什么 | 不能说明什么 |
| --- | --- | --- |
| 银行待处理或预授权 | 银行暂时占用资金 | 不能证明 Anthropic 已完成订阅 |
| 银行最终入账 | 付款可能完成 | 仍需核对订单与账号 |
| Anthropic 官方收据 | 官方订单已生成的重要证据 | 仍需确认收据对应哪个登录邮箱 |
| `Settings > Billing` 显示有效套餐 | 当前账号存在订阅 | 仍需确认网页和 App 是否登录同一账号 |

没有官方收据且交易仍待处理时，先联系银行确认状态，不要重复购买。

## 第二步：检查当前登录邮箱

Anthropic 官方 Billing FAQ 将“登录了不同邮箱”列为付费账号显示 Free 的首要检查项。

依次尝试：

1. 查看官方收据发送到哪个邮箱；
2. 确认网页、桌面端和手机端的登录邮箱；
3. 检查是否使用了不同登录方式创建多个 Claude 账号；
4. 退出当前账号，再用原购买邮箱登录。

不要只凭头像或昵称判断账号归属。

## 第三步：查看 Settings > Billing

在原购买账号进入 `Settings > Billing`，核对：

- 当前套餐；
- 最近发票；
- 付款是否成功或失败；
- 是否需要更新付款方式；
- 订阅是否已取消或到期。

如果付款方式失败，账号可能被降级为 Free。此时应先处理原付款方式或联系 Anthropic，而不是创建第二份订阅。

## 第四步：按原购买平台处理

### 网页或 Claude Desktop

通过 Anthropic 网页购买的订阅，在 Claude 的 Billing 页面管理。

### iOS App Store

应用商店订单、取消与退款由 Apple 管理。检查原 Apple ID 的订阅和收据，同时确认 Claude App 登录的是原购买时的 Claude 账号。

### Android Google Play

检查原 Google Play 账号中的订阅状态和订单，并确认 Claude App 登录的是原购买账号。不要套用 iOS 专用的恢复购买入口。

## 第五步：ChongGrok 订单路径

如果这笔付款是 ChongGrok Claude 订阅协助订单：

1. 核对订单号、目标套餐和提交时间；
2. 确认提交的 User ID 属于当前目标账号；
3. 将 Claude Billing 状态和脱敏后的账号邮箱提供给客服核对；
4. 等原订单状态查清后再决定下一步，不重复下单。

User ID 不是密码，但仍属于账号相关信息。不要在公开评论中粘贴完整 User ID。

## 什么时候联系谁

| 问题 | 联系对象 |
| --- | --- |
| Anthropic 官方收据存在，但 Billing 不显示 | Anthropic 支持 |
| App Store 订单、退款或扣款 | Apple 支持 |
| Google Play 订单、退款或扣款 | Google Play 支持 |
| 银行待处理或重复扣款 | 发卡银行 |
| ChongGrok 订单、User ID 或处理记录 | ChongGrok 客服 |

## 证据清单

- 付款日期、金额和币种；
- 官方或应用商店收据；
- 原购买入口；
- 当前登录邮箱；
- `Settings > Billing` 状态；
- 如为 ChongGrok 订单，附订单号和已提交套餐。

所有截图应遮蔽完整卡号、账单地址、User ID、邮箱和订单敏感字段。

## 官方来源

- [Anthropic Help：Paid Plan Billing FAQs](https://support.anthropic.com/en/articles/8325618-where-can-i-find-the-receipt-for-my-claude-subscription)
- [Anthropic Help：Cancel a paid subscription](https://support.anthropic.com/en/articles/8325617-how-do-i-cancel-my-paid-claude-subscription)

{% include faq.html %}
