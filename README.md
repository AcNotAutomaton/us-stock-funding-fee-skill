# us-stock-funding-fee

用于比较“汇丰香港 <-> 嘉信”双向路径的手续费与折损，支持一键给出 5 方案成本、最低成本方案、关键交叉点和风险提示。

## 1) 支持场景

- `inflow`：汇丰香港入金嘉信
- `outflow`：嘉信出金汇丰香港

## 2) 你需要提供什么

最少 3 个参数：
- `direction`：`inflow` 或 `outflow`
- `amount`：金额（数字）
- `currency`：初始持有资金的币种，`USD` 或 `HKD`

可选参数：
- `rate`：USDHKD 汇率（不传默认 `7.8`）

建议输入习惯：
- 金额尽量写纯数字，比如 `10000`，不要写 `1w`、`十万`
- 若是港币金额，明确标注 `currency=HKD`
- `rate` 是 USD/HKD 比较基准，不代表实际成交汇率

入金按初始币种分组比较：港币对应方案一、三；美元对应方案二、四、五。具体路径和适用条件见 [路径目录](references/route-catalog.md)，计算方法见 [计算规则](references/calculation-rules.md)。费用为参考模型；出金路径目前仍待核实。

## 3) 怎么提问（可直接复制）

### A. 最标准话术

```text
请按 us-stock-funding-fee-skill 计算：
direction=inflow
amount=10000
currency=USD
rate=7.82
请输出5个方案成本、最低成本方案、交叉点和风险提示。
```
