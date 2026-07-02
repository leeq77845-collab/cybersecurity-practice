# PortSwigger Web Security Academy - SQL Injection Labs

SQL Injection 学习笔记与实验记录（PortSwigger Web Security Academy）

## 📖 目录
- [简介](#简介)
- [学习收获](#学习收获)
- [Labs 列表](#labs-列表)
- [环境与工具](#环境与工具)
- [常用 Payload](#常用-payload)
- [后续计划](#后续计划)

## 简介
本仓库记录了我在 **PortSwigger Web Security Academy** SQL Injection 模块中完成的所有实验，包括：
- 基础 UNION 注入
- 盲注（Boolean-based、Time-based）
- Out-of-Band（待补充）
- 数据库枚举等

**目标**：系统性掌握 SQL 注入的检测、利用与绕过技巧。

## 学习收获
- 熟练掌握了不同类型 SQLi 的利用方法
- 理解了数据库差异（MySQL / PostgreSQL / Oracle / MSSQL）
- 提升了 Burp Suite 使用能力
- ...

## Labs 列表

| 序号 | Lab 名称 | 难度 | 关键技术 | 状态 |
|------|----------|------|----------|------|
| 01   | SQL injection in WHERE clause | Apprentice | OR 1=1 | ✅ |
| 02   | Login bypass | Apprentice | Comment | ✅ |
| 03   | UNION attack - determining columns | Practitioner | ORDER BY / UNION | ✅ |
| ...  | ... | ... | ... | ✅ |

**详细 Writeup** 请查看 [labs 文件夹](./labs)

## 环境与工具
- **平台**：PortSwigger Web Security Academy
- **工具**：Burp Suite Community / Professional
- **数据库**：MySQL、PostgreSQL、Oracle 等

## 常用 Payload
```sql
-- 基础
' OR 1=1--
' UNION SELECT NULL,NULL--
