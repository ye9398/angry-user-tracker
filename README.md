# 愤怒用户追踪器 - Vercel 部署指南

## 📦 部署文件位置

```
tasks/angry-user-tracker/vercel-dist/
├── index.html          # 首页（查询表单）
├── sample-report.html  # 示例报告
└── vercel.json         # Vercel 配置
```

---

## 🚀 部署步骤

### 方式 1：Vercel CLI（推荐）

```bash
# 1. 安装 Vercel CLI
npm install -g vercel

# 2. 登录 Vercel
vercel login

# 3. 进入部署目录
cd tasks/angry-user-tracker/vercel-dist

# 4. 部署
vercel --prod
```

### 方式 2：Vercel 网站上传

1. 访问 https://vercel.com/new
2. 点击 **"Add New Project"**
3. 选择 **"Continue with GitHub"**（需要 Git 仓库）
4. 或者使用 **Vercel CLI** 直接上传

---

## 📝 部署后说明

### 页面功能

| 页面 | URL | 功能 |
|------|-----|------|
| **首页** | `https://your-project.vercel.app/` | 查询表单（演示模式） |
| **示例报告** | `https://your-project.vercel.app/sample-report` | 完整报告展示 |

### 演示模式说明

- ✅ 可以填写表单
- ✅ 点击"开始分析"会跳转到示例报告
- ❌ 不会执行真实分析（没有后端 API）

---

## 🔗 分享给朋友

部署成功后，发送链接给朋友：

```
首页：https://your-project.vercel.app/
示例报告：https://your-project.vercel.app/sample-report
```

---

## ⚠️ 注意事项

1. **API 不可用** - 这是纯静态演示，没有后端
2. **示例报告是硬编码数据** - 展示的是"破壁机/搅拌机"品类
3. **如需真实功能** - 需要部署完整后端（Railway/Render）

---

_部署时间：2026-03-20_
