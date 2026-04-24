# 刘崇豪 - 个人简历网站

## 🚀 部署到 Vercel（推荐，免费，无需备案）

### 方式一：直接上传（最快）
1. 打开 https://vercel.com 登录
2. 点击 **Add New → Upload**
3. 将本文件夹内的所有文件拖入上传区域
4. 点击 **Deploy**，等待 1-2 分钟即可获得公网地址

### 方式二：通过 GitHub（方便后续更新）
1. 在 GitHub 创建新仓库 `resume`
2. 将本文件夹内文件推送到仓库：
   ```bash
   git init
   git add .
   git commit -m "初始化个人简历网站"
   git remote add origin https://github.com/你的用户名/resume.git
   git push -u origin main
   ```
3. 打开 https://vercel.com → Import Git Repository → 导入你的仓库
4. Framework Preset 选 **Other**
5. 点 **Deploy**

### 绑定自定义域名
1. 购买域名（阿里云/腾讯云/Cloudflare 等）
2. 在域名 DNS 管理中添加 CNAME 记录：
   - 主机记录：`@` 和 `www`
   - 记录值：`cname.vercel-dns.com`
3. Vercel 项目 → Settings → Domains → 输入你的域名
4. 等待 DNS 生效（通常几分钟），Vercel 自动配置 HTTPS

## 📁 文件说明

| 文件 | 说明 |
|------|------|
| index.html | 简历主页（完整单页应用） |
| vercel.json | Vercel 部署配置 |
| package.json | 项目信息 |

## 🛠️ 本地预览

```bash
npx serve .
```
然后打开 http://localhost:3000 查看
