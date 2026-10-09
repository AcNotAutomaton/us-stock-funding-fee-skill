# 五方案路径目录

入金编号与路径以用户于 2026-09-26 提供的五方案截图为依据。截图费率是参考模型，不是已核实的当前报价。模型计算见 `calculation-rules.md`；实际比较须同时判断路径可用性和全程费用。

## 入金：汇丰香港 → 嘉信

| 方案 | 资金路径 | 模型费用 | 适用前提与提示 |
|---|---|---:|---|
| 一 | 汇丰香港 HKD → 嘉信指定的港币收款路径 → 嘉信兑换为 USD 入账 | 汇损约 0.16% | 截图估计的嘉信端兑换折损，不是电汇费。须取得适用于本人账户的 HKD 收款指示；不得自行猜测本地收款账户或 FPS 支持情况。实际兑换率不保证，银行转账费用另计。 |
| 二 | 汇丰香港 USD → 国际美元电汇 → 嘉信指定收款银行及归户账户 → 嘉信 USD 入账 | 21.88 USD | 截图固定成本假设，未核实组成及适用收费选项；汇丰发汇费、代理行扣费应核对。按本人嘉信账户最新指示填写收款人及归户附言。 |
| 三 | 汇丰香港 HKD → Wise 换为 USD → 嘉信关联本人 Wise USD 账户，并由嘉信发起 ACH 拉取 | 兑换费约 0.4%；USD 拉取段按用户说明为 0 | 有条件可用；港币换美元仍有兑换成本。须有支持扣款的 Wise USD 账户资料，完成嘉信外部账户关联及验证，并备足 USD 余额。汇丰到 Wise 的港币转账费按实际计，不自动套用方案四的美元路径收费。 |
| 四 | 汇丰香港 USD → 本人 Wise USD 余额 → 嘉信关联该账户并发起 ACH 拉取 → 嘉信 USD 入账 | 香港本地 CHATS 入 Wise：Wise 收款费 10 HKD 或等值；Wise USD 到嘉信：0（用户提供） | 有条件可用；使用 Wise 香港多币种收款资料，经汇丰本地 RTGS／CHATS 汇 USD 时，汇丰本行发汇费 0，10 HKD 是 Wise 收款费。需有可用香港收款资料、完成嘉信外部账户验证与扣款授权，并备足 USD。不得推广到国际 SWIFT 或其他付款方式；全程保持 USD 时无换汇损失。 |
| 五 | 汇丰香港 USD → Global Transfers 至本人 HSBC US USD 账户 → 适用的 ACH 转账 → 本人嘉信账户 | 0 转账手续费（有条件） | 须拥有可用 HSBC US 账户、符合汇丰 Global Transfers 免手续费资格，并完成嘉信 ACH 关联及资格确认；“有美卡”不等于满足条件。HKD 先换 USD 的汇差、账户维护成本不在零转账费中。 |

### 官方核查（2026-09-26）

- [Wise 美元转账指南](https://wise.com/help/articles/2932150/guide-to-usd-transfers)：不支持向券商账户、中转银行发送 USD，也不支持 FFC；这是 Wise 主动汇款规则，不能用于否定由嘉信发起的 ACH 拉取。
- [Wise Direct Debit 说明](https://wise.com/help/articles/2977956/getting-started-with-direct-debits)：支持 USD 账户资料的直接扣款；若缺少相应币种可能自动换汇，因此无汇损模型要求备足 USD。
- [Wise 美元直接扣款介绍](https://wise.com/us/blog/usd-direct-debits-launch)：介绍关联银行、券商及交易平台进行扣款的机制；此历史产品说明不保证每个账户当前均可关联。
- [嘉信 MoneyLink 条款](https://www.schwab.com/legal/schwab-moneylink-terms-and-conditions)：允许嘉信向已授权外部账户发起 ACH 借记，账户需符合验证和服务资格。用户补充确认这里使用的是该方向的拉取；以上官方资料支持机制，但不构成对用户具体 Wise 账户的逐户验证。
- [嘉信香港入金说明](https://www.schwab.com.hk/fund-your-account)：列出美元电汇及归户要求；其他外币须联系嘉信获取指示，并提示代理行收费。该页面要求汇款账户所有持有人与嘉信香港账户一致；其他嘉信实体须用各自适用规则。
- [嘉信国际电汇指引](https://international.schwab.com/content/how-to-fund-your-account)：收款人通常为嘉信公司，通过附言指定个人账户；须以登录后指示为准。
- [汇丰香港 Global Transfers](https://www.hsbc.com.hk/transfer-payments/products/international/global-transfers/)：支持美国；页面列明 Global Private Banking、Premier Elite、Premier、HSBC One 客户享免手续费，币种和账户类型仍有限制。

上述来源不证明截图中的 0.16%、21.88 USD、0.4% 是当前全程成本。方案四的 10 HKD 于 2026-10-10 另查 [Wise 香港收款资料](https://wise.com/help/articles/12CQfcpIVOHULnFNNzBgmE/how-do-i-receive-money-with-my-hkd-account-details) 与 [汇丰本地 RTGS 说明](https://www.hsbc.com.hk/transfer-payments/products/local/)：该费用为 Wise 本地 CHATS 收款费，而非汇丰发汇费；详见 [香港美元汇入华美](hong-kong-to-east-west-bank.md) 的本地入 Wise 环节，不套用其 Wise 主动出款费到嘉信拉取段。截图中的每条路径不代表对所有地区及账户类型均可用。

## 出金：嘉信 → 汇丰香港

以下出金路径来自先前推测，尚无用户原始出金图或逐项官方核验支持。不得因入金截图已确认就把这些出金编号映射当成已确认事实；仅作待核实模型，实际推荐前须另行核实。

| 方案 | 资金路径 | 模型费用 | 适用前提与提示 |
|---|---|---:|---|
| 一 | 嘉信 USD 账户 → 国际 USD SWIFT 电汇 → 汇丰香港 USD 账户 | 15–50 USD | 直接国际电汇；区间用于涵盖发汇、代理行或收款行扣费，到账金额可能低于汇出金额。 |
| 二 | 嘉信 USD 账户 → Wise 的 USD 收款资料 → Wise 以 USD 汇至汇丰香港 USD 账户 | 9.57 USD | 固定费模型；Wise 对香港 USD 出款的收费会随付款方式变化，操作前看订单最终报价。 |
| 三 | 嘉信 USD 账户 → Wise → 换成 HKD → 汇丰香港 HKD 账户 | 金额的 0.3% | 将模型视为 USD/HKD 换汇与转出成本；比较时应以实际到帐 HKD 与银行牌价一并判断。 |
| 四 | 嘉信 USD 账户 → ACH 至 HSBC US 同名账户 → 汇丰 Global Transfer 至汇丰香港同名账户 | 0 USD | 必须持有 HSBC US，并满足 Global Transfer 的同名账户、地区与币种资格；模型不计汇差。 |
| 五 | 嘉信 USD 账户 → ACH 至 IBKR → IBKR USD/HKD 换汇 → 提现至汇丰香港 | 2 USD | 2 USD 仅为模型中的 IBKR 换汇费；IBKR 提现额度、后续提现费、入金/出金审核与嘉信对外部券商转账规则均可能带来额外限制或费用。 |

## 使用约束

- 输出时应同时显示上述“资金路径”和“模型费用”，不能只写方案编号。
- 按方向逐行判断状态：已知不支持、不满足条件、待核实、可用。未知资格不能写成已满足，也不能直接断言永久不可用。入金三、四使用嘉信发起的 ACH 拉取，符合账户关联及扣款条件时可参与推荐；不得与 Wise 主动汇款混淆。
- 不把模型费率描述为官方实时价。若用户要求实际操作建议、实时费用或确认某路径可否入金，应先核验嘉信、汇丰、Wise 或 IBKR 的当前规则。
