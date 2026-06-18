# 网络安全实战练习

> 从“写代码”到“审代码”的第一天。  
> 主题：XSS 注入与防御、JavaScript 调试、浏览器 F12 武器库。

## 📌 今日核心成就
- ✅ 成功复现 **反射型 XSS**（注入 `<img src=x onerror=alert(1)>`）
- ✅ 使用 `textContent` 防御 XSS，完成攻防闭环
- ✅ 掌握浏览器 F12 三件套：Console（查变量）、Sources（断点）、Network（抓包）
- ✅ 熟悉 `for...of`、`for`、`break`、`continue` 循环控制
- ✅ Linux Vim 精准定位行号（`:set number`、`:87`）

## 🛠️ 技术栈
- HTML / CSS / JavaScript (Vanilla)
- 浏览器开发者工具 (DevTools)
- Vim / Linux 命令行

## 🔐 核心收获
> **“永远不要相信用户输入”**  
> **“内容用 textContent，属性用白名单”**

## 📁 目录结构
- `xss-lab/` —— XSS 注入与防御靶场（漏洞版 + 修复版）
- `debugging/` —— 基于 MDN 教学示例的调试练习（经手动漏洞修复）
- `loop-exercises/` —— JavaScript 循环控制基础练习
- `notes/` —— 每日实战手记
