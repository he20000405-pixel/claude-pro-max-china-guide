# 2026 Claude Pro / Max 国内订阅指南：支付宝微信付款、User ID、付款失败与订阅排查

> **English summary:** An independent Claude Pro and Max knowledge base by [ChongGrok](https://chonggrok.com/claude), covering plan choice, account safety and payment troubleshooting. The current merchant service is a personal monthly Pro subscription on the customer's own account, opened through assisted iOS in-app purchase; Max is not offered. [Read the English guide](README_EN.md).

这是 **ChongGrok Claude 会员订阅知识库**。内容围绕 Claude Pro、Max 5x、Max 20x 的官方套餐知识、付款与账号状态排查展开。商家当前服务仅为自有账号个人 Pro 月度开通，人工通过 iOS 内购办理，不提供 Max、团队席位或 API。

**服务入口：<https://chonggrok.com/claude>**

> ChongGrok 是独立第三方会员订阅协助服务，与 Anthropic 不存在隶属、授权或官方合作关系。Claude 的价格、模型、额度、地区可用性和订阅规则以 Anthropic 实时页面为准。

## 快速结论

| 问题 | 直接回答 |
| --- | --- |
| 官方个人套餐有哪些？ | Claude Pro 网页月付为 20 美元，也提供年付选项；Max 5x 为 100 美元/月；Max 20x 为 200 美元/月。年付、移动端、税费和地区价格以账号结账页为准。 |
| ChongGrok 怎么处理？ | 核对账号、支持地区与资料要求后，人工通过 iOS 内购为用户自有账号开通个人 Pro 月度订阅。 |
| 是否需要密码？ | 不需要 Claude 密码、邮箱密码、验证码或恢复码。 |
| User ID 是什么？ | Claude 账号标识，不是密码。是否需要提交以当前订单要求为准；先确认用途与所属账号，不根据旧教程猜测或发送完整会话数据。 |
| ChongGrok 提供 Max 吗？ | 不提供。Max 5x/20x 保留为官方套餐知识；购买、续费和管理请使用 Claude 官方渠道。 |
| 是否提供 API？ | 不提供。这里只讨论 Claude 个人会员订阅，不提供 API 额度或 API 充值。 |

## 先判断套餐

| 套餐 | 官方月费 | 适合情况 | ChongGrok 入口 |
| --- | ---: | --- | --- |
| Claude Pro | 网页月付 20 美元；年付以结账页为准 | 日常写作、资料整理、文件分析和轻量 Claude Code | 主站查看实时方案 |
| Claude Max 5x | 100 美元 | Pro 用量长期不足、较高频知识工作和更大的代码任务 | 本站不提供，请查看 Claude 官方渠道 |
| Claude Max 20x | 200 美元 | Max 5x 仍不足的重度、持续工作流 | 本站不提供，请查看 Claude 官方渠道 |

详细决策见：[Claude Pro、Max 5x、Max 20x 怎么选](guides/claude-pro-vs-max.md)。

## 按你现在的问题进入

| 你看到的情况 | 先做什么 | 什么时候停止 |
| --- | --- | --- |
| 还没有会员，不知道选哪一档 | 先记录一周内实际遇到的使用限制，再看[套餐选择](guides/claude-pro-vs-max.md) | 当前 Free 或 Pro 已能完成任务时，不必升级 |
| 银行卡付款没有通过 | 保存报错和购买入口，按[付款失败排查](guides/claude-payment-errors.md)逐项检查 | 已扣款、交易待处理或收到收据时，不要再次付款 |
| 已扣款但 Claude 仍显示 Free | 核对收据邮箱、当前登录邮箱和 `Settings > Billing` | 原订单没有查清前，不要新建第二份订阅 |
| Claude Code 没有识别会员 | 先确认网页 Billing 有效，再核对终端登录账号 | 终端正在使用 API Key 计费时，先停止并确认计费方式 |

## Pro 月度开通流程

1. 打开 <https://chonggrok.com/claude>，核对个人 Pro 月度服务、实时金额与售后条件。
2. 联系客服，确认 Claude 账号能正常登录、本人符合支持地区要求，且没有未查清的订阅或待处理交易。
3. 按确认后的流程付款，只提供当前订单所需的账号资料；若需 User ID，先核对用途和所属账号。
4. 人工通过 iOS 内购为目标账号开通 Pro 月度订阅。
5. 用户回到 Claude 的 `Settings > Billing`，验收 Pro 状态、有效期与订单交付结果。
6. 如状态不一致，保留订单、付款记录和 Claude Billing 页面信息，由对应责任方继续排查。

完整流程见：[Claude Pro 月度开通与验收](guides/claude-pro-max-recharge.md)。

## 七个核心专题

1. [Claude Pro 月度开通与验收](guides/claude-pro-max-recharge.md)
2. [Claude Pro、Max 5x、Max 20x 怎么选](guides/claude-pro-vs-max.md)
3. [Claude User ID 格式、用途与安全提交](guides/claude-user-id-safety.md)
4. [Claude 银行卡被拒、账单地址与 3DS 排查](guides/claude-payment-errors.md)
5. [Claude 已付款但仍显示 Free](guides/claude-paid-but-still-free.md)
6. [Claude 续费失败或被降级为 Free](guides/claude-renewal-failed-back-to-free.md)
7. [Claude Code 使用 Pro / Max 登录与额度边界](guides/claude-code-pro-max.md)

## 安全与服务边界

- 不索要 Claude 密码、邮箱密码、验证码或恢复码，不要发送完整会话令牌。
- User ID 不是密码，但仍应只在确认的客服履约流程中提交。
- 不承诺绝对安全、固定到账、保证恢复或所有账号都能开通。
- 付款和 iOS 内购不会改变地区或身份验证要求；开通失败按约定处理退款，成功开通后的官方风控封号不提供质保。
- 服务仅为个人 Pro 月度，不包含 Max；官方 Max 套餐比较不代表商家可售范围。
- 不提供 API 额度、成品号、接码、批量注册、Team/Enterprise 批量业务或地区限制规避教程。
- 官方套餐与会员订阅不等于 Anthropic API 额度。

## 官方资料

- [Anthropic：Claude plans and pricing](https://www.anthropic.com/pricing?subjects=claude&type=product)
- [Claude Help：Choose a Claude plan](https://support.claude.com/en/articles/11049762-choose-a-claude-plan)
- [Claude Help：What is the Max plan?](https://support.claude.com/en/articles/11049741-what-is-the-max-plan)
- [Claude Help：What is the Pro plan?](https://support.claude.com/en/articles/8325606-what-is-the-pro-plan)
- [Anthropic Help：Paid Plan Billing FAQs](https://support.anthropic.com/en/articles/8325618-where-can-i-find-the-receipt-for-my-claude-subscription)
- [Anthropic Help：Why was my card declined?](https://support.anthropic.com/en/articles/9402418-why-was-my-card-declined)
- [Anthropic Help：Using Claude Code with Pro or Max](https://support.anthropic.com/en/articles/11145838-using-claude-code-with-your-max-plan)

GitHub Pages：<https://he20000405-pixel.github.io/claude-pro-max-china-guide/>

指南门户：<https://guides.chonggrok.com/>

服务说明更新：2026-10-28；官方套餐与价格以实时页面为准。
