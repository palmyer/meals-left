# 人生饭量余额

吃饭是无意识的日常，但一生的饭量有总额度

> 点子来源：Obsidian《人生可视化 / 人生饭量余额》 · 同系列仓库参考 [life-grid](https://github.com/palmyer/life-grid)

## 功能

- 已吃掉 / 剩余 / 一生总顿数
- 人生饭量额度已消耗百分比进度条
- 生日与寿命全站共享设置（iOS 滚轮）

## 运行

纯静态零依赖，任选其一：

```bash
cd meals-left
python -m http.server 8740
```

- 网页版：<http://127.0.0.1:8740/>
- 手机壳预览：<http://127.0.0.1:8740/preview.html>（life-grid 同款）

或直接双击 `index.html`。

## 设计

- iOS 暗色风格：纯黑背景、#1C1C1E 分组卡片、SF 系统色板
- 选择一律使用 iOS 风格底部滚轮（`shared/wheel.js`）
- 数据存于浏览器 localStorage（`lv-` 前缀），不上传任何服务器
- 生日 / 预期寿命与同系列工具共享同一份配置
