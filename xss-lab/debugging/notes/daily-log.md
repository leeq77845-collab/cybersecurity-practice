# 2026-06-18 实战手记

## 今日 Bug 合集
1. **拼写错误**：`addeventListener` → `addEventListener`
   - 教训：JS 严格区分大小写，报错 `is not a function` 时优先检查拼写。

2. **选择器错误**：`querySelector("lowOrHi")` → `querySelector(".lowOrHi")`
   - 教训：类选择器必须带 `.`，否则返回 `null` 导致 `Cannot set properties of null`。

3. **逻辑错误**：`Math.floor(Math.random()) + 1` 永远等于 1
   - 教训：`Math.random()` 范围 [0,1)，必须乘以范围数（如 `* 100`）才能生成随机整数。

## XSS 攻防总结
- **攻击载荷**：`<img src=x onerror=alert('XSS')>`
- **防御武器**：`textContent` 替代 `innerHTML`
- **铁律**：用户输入的任何数据，输出到页面时都必须编码。

## 今日金句
> “测试是证明程序‘能做’什么；安全是证明程序‘不该做’的做了。”
