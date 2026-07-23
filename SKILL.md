---
name: us-stock-funding-fee
description: 比较汇丰香港与嘉信理财的双向资金路径手续费与折损，支持 inflow/outflow 方向、USD/HKD 币种，输出 5 个方案成本、最低成本方案、交叉点和风险提示。当用户询问美股出入金费用、汇丰转嘉信、嘉信转汇丰、资金路径对比时使用。
---

# US Stock Funding Fee

## Purpose
用于比较汇丰香港 <-> 嘉信的双向资金路径手续费与折损：
- 入金：汇丰香港 -> 嘉信（inflow）
- 出金：嘉信 -> 汇丰香港（outflow）

## Required Inputs
- `direction`（必填）：`inflow` 或 `outflow`
- `amount`（必填）
- `currency`（必填）：`USD` 或 `HKD`
- `rate`（可选）：默认 `7.8`

## Core Rules
严格按 `references/calculation-rules.md` 执行；不可混用入金/出金费率。

## Output Requirements
- 必须输出对应方向下 5 个方案（不省略）
- 输出：方案名称（含操作路径，如"港币直入花旗香港""美元电汇花旗美国"等）、手续费、折算、备注
- 给出最低手续费方案 + 前提
- 给出关键交叉点
- 给出稳定性/风控提示
- 附免责声明
