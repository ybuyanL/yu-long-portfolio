# 余龙个人网站

这是一个无框架、无构建依赖的静态个人网站，文件可以直接部署到任意静态托管服务。

## 本地预览

在当前目录启动任意静态文件服务器即可。例如：

```bash
python -m http.server 4173
```

然后打开 `http://localhost:4173`。

## 部署方式

### GitHub Pages

1. 在 GitHub 新建一个仓库，例如 `yu-long-portfolio`。
2. 将本目录下的全部文件上传到仓库根目录。
3. 进入仓库的 `Settings` -> `Pages`。
4. 在 `Build and deployment` 中选择 `Deploy from a branch`。
5. 分支选择 `main`，目录选择 `/ (root)`，点击保存。
6. 等待几分钟后，GitHub 会生成公开网址。

### Netlify

1. 登录 Netlify，选择 `Add new site` -> `Deploy manually`。
2. 将本目录整体拖入上传区域。
3. 上传完成后即可使用 Netlify 分配的网址。
4. 在站点设置中可以修改站点名称，或绑定自己的域名。

### Vercel

1. 将本目录上传到 GitHub。
2. 登录 Vercel，点击 `Add New` -> `Project`。
3. 导入刚才的 GitHub 仓库。
4. `Framework Preset` 选择 `Other`，构建命令留空，输出目录使用仓库根目录。
5. 点击部署。每次推送到 `main` 后，Vercel 会自动更新网站。

## 上线前检查

- 将联系方式换成你愿意公开展示的版本。
- 确认 `余龙-全栈方向简历.pdf` 与网页一起上传。
- 用手机打开一次，检查电话、邮箱和简历下载按钮。
- 如果绑定域名，将域名的 DNS 按托管平台提示配置即可。
