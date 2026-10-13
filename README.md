# FDE 学习中心

[打开学习网站](https://964351819-ui.github.io/fde-learning-center/)

38 课沿同一个模拟企业项目学习，包含课程目录、案例资料、逐步示范、判断题、引导练习和完整白话词卡。

## 学习记录与评审

- 回答只保存在当前浏览器，不上传 GitHub。清理浏览器前请导出备份。
- 原网站的“记录 → 导出”文件，可以通过这里的“记录 → 导入记录”迁移。已有导师反馈保留。
- 完成练习后点击“复制评审资料”，粘贴到原来的学习对话，由导师逐题评审。
- GitHub Pages 版没有原站的后台评审服务。原学习对话中的定时提醒保持原设置。
- 资讯从 `daily-news.json` 读取；显示实际资料日期，不自动把旧资料标成今天。此仓库尚未配置自动资讯更新。

## 内容与源码

- `index.html`：直接可部署的独立页面，JS/CSS/课程内容内嵌，不依赖原站。
- `practice.zip`：工程练习包。
- `source.zip`：可编辑的前端源码和构建脚本，不含个人回答、数据库或密钥。

解压 `source.zip` 后（Node.js 22 及以上）：

```sh
npm install
npm run check
npm run build
```

生成的 `publish/` 文件可重新上传到仓库。源码的 `lib/casebook.ts` 管理案例与课堂练习；`lib/word-details.ts` 管理词卡；`pages/learning-center.tsx` 管理学习界面。

## 发布设置

仓库 Settings → Pages → Deploy from a branch → `main` → `/ (root)`。

本课程为原创模拟项目学习材料；并非培训机构的付费课程原文，也不提供职业认证。
