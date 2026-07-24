---
title: "Claude Pro / Max 国内订阅指南：付款与 User ID 排查"
description: "ChongGrok Claude Pro、Max 5x 和 Max 20x 国内订阅指南，覆盖客服协助官方付款、User ID 安全、银行卡被拒、续费失败、已付款仍显示 Free 和 Claude Code。"
permalink: /
last_modified_at: 2026-07-14
breadcrumbs:
  - name: 首页
    url: /
faq:
  - question: "Claude Pro、Max 5x 和 Max 20x 官方价格分别是多少？"
    answer: "Anthropic 当前公开的美国价格为 Pro 月付 20 美元或年付 200 美元、Max 5x 每月 100 美元和 Max 20x 每月 200 美元，地区价格和税费以官方结账页实时显示为准。"
  - question: "ChongGrok 开通 Claude 是否需要账号密码？"
    answer: "不需要 Claude 密码、邮箱密码、验证码或恢复码。客服会说明本次履约所需的 Claude User ID；User ID 不是密码，但仍应谨慎提交。"
  - question: "Claude Max 可以直接按主站公开价格下单吗？"
    answer: "当前主站公开页面以 Claude Pro 为主。Max 5x 或 Max 20x 应先通过 Claude 页面联系客服确认账号、套餐、人民币金额和验收规则。"
---

# 2026 Claude Pro / Max 国内订阅指南

<p class="lead">这是 ChongGrok 的 Claude 会员订阅服务指南和排障知识库，覆盖 Claude Pro、Max 5x、Max 20x 的套餐选择、客服协助官方付款、User ID 安全、银行卡被拒、续费失败与付费状态验收。</p>

<a class="primary-link" href="https://chonggrok.com/claude">查看 ChongGrok Claude 实时方案</a>

> ChongGrok 与 Anthropic 不存在隶属、授权或官方合作关系。套餐、模型、额度、地区可用性和官方价格以 Anthropic 实时页面为准。

## 三档个人套餐怎么理解

| 套餐 | 官方月费 | 主要区别 | 本站承接方式 |
| --- | ---: | --- | --- |
| Claude Pro | 月付 20 美元；年付 200 美元 | 适合日常知识工作与轻量 Claude Code | 主站查看实时方案，客服协助官方付款 |
| Claude Max 5x | 100 美元 | 相对 Pro 提供更高使用量 | 先联系客服确认账号与金额 |
| Claude Max 20x | 200 美元 | 面向持续高强度工作流 | 先联系客服确认账号与金额 |

官方计划页将 Max 描述为包含 Pro 的能力，并提供 5x 或 20x 相对使用量。实际限制还会受消息长度、附件、模型、对话长度和 Claude Code 工作负载影响，不能把“5x/20x”理解成固定消息数量保证。

## 充值与验收路径

1. 进入 <https://chonggrok.com/claude>，确认目标套餐。
2. 联系客服，先核对账号能否登录、当前订阅与目标档位。
3. 按确认后的金额付款，只提交本次履约需要的 Claude User ID。
4. 客服使用海外卡协助完成官方订阅付款。
5. 用户进入 Claude 的 `Settings > Billing` 检查当前套餐、发票或付款状态。

不需要 Claude 密码、邮箱密码、验证码或恢复码。User ID 是 ChongGrok 用于定位目标账号的服务凭证，不是 Anthropic 官方订阅步骤，也不等于零风险。

## 七个核心专题

<div class="guide-grid">
  <section class="guide-card"><h3><a href="guides/claude-pro-max-recharge/">Pro / Max 充值流程</a></h3><p>从账号确认、User ID、客服协助付款到 Billing 验收。</p></section>
  <section class="guide-card"><h3><a href="guides/claude-pro-vs-max/">Pro 与 Max 怎么选</a></h3><p>按真实使用强度区分 Pro、Max 5x 和 Max 20x。</p></section>
  <section class="guide-card"><h3><a href="guides/claude-user-id-safety/">User ID 安全说明</a></h3><p>说明格式、用途、脱敏方法和不应提交的信息。</p></section>
  <section class="guide-card"><h3><a href="guides/claude-payment-errors/">付款被拒排查</a></h3><p>检查账单地区、地址、3DS、余额和发卡行限制。</p></section>
  <section class="guide-card"><h3><a href="guides/claude-paid-but-still-free/">已付款仍显示 Free</a></h3><p>核对登录邮箱、付款状态、原购买平台和订单证据。</p></section>
  <section class="guide-card"><h3><a href="guides/claude-renewal-failed-back-to-free/">续费失败变回 Free</a></h3><p>区分续费失败、主动取消、到期和登录错账号。</p></section>
  <section class="guide-card"><h3><a href="guides/claude-code-pro-max/">Claude Code 与会员</a></h3><p>使用同一 Pro / Max 账号登录，区分会员额度与 API 计费。</p></section>
</div>

[查看全部 Claude 专题](guides/)

## User ID 和密码的边界

| 信息 | 是否需要 | 说明 |
| --- | --- | --- |
| Claude 密码 | 不需要 | 不应向第三方提供 |
| 邮箱密码 | 不需要 | 不应提交 |
| 验证码或恢复码 | 不需要 | 不应通过聊天工具转发 |
| Claude User ID | 客服确认后按履约要求提供 | 以当前确认界面显示为准，仅用于定位目标账号 |

首版不提供未经核实的内部接口或提取脚本。待获得当前真实入口和脱敏截图后，再补充可复现的获取步骤。

## 付款失败先做什么

Anthropic 官方建议优先检查受支持的账单地区、账单地址是否与银行记录一致、3D Secure 验证、卡片类型、余额和发卡行限制。不要连续无目的重试，也不要在已经产生有效扣款时立即再次购买。

- 尚未扣款：[Claude 银行卡被拒与 3DS 排查](guides/claude-payment-errors/)
- 已经扣款：[Claude 已付款但仍显示 Free](guides/claude-paid-but-still-free/)
- 原会员续费失败：[Claude 续费失败或被降级为 Free](guides/claude-renewal-failed-back-to-free/)

## 业务边界

- 只讨论 Claude 个人会员订阅，不提供 API 额度或 API 充值。
- 不提供成品号、接码、批量注册或地区限制规避教程。
- 不承接 Team/Enterprise 批量业务。
- 不承诺绝对安全、固定到账、保证恢复或所有账号均可开通。
- 付款完成后由用户回 Claude 官方页面验收。

## 官方来源

- [Claude plans and pricing](https://www.anthropic.com/pricing?subjects=claude&type=product)
- [Claude Help：Choose a Claude plan](https://support.claude.com/en/articles/11049762-choose-a-claude-plan)
- [Claude Help：What is the Max plan?](https://support.claude.com/en/articles/11049741-what-is-the-max-plan)
- [What is the Pro plan?](https://support.claude.com/en/articles/8325606-what-is-the-pro-plan)
- [Paid Plan Billing FAQs](https://support.anthropic.com/en/articles/8325618-where-can-i-find-the-receipt-for-my-claude-subscription)
- [Why was my card declined?](https://support.anthropic.com/en/articles/9402418-why-was-my-card-declined)
- [Using Claude Code with Pro or Max](https://support.anthropic.com/en/articles/11145838-using-claude-code-with-your-max-plan)

{% include faq.html %}

<p class="meta">最后更新：2026-07-14</p>
