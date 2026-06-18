# GitHub Pages 部署说明

这个项目已经处理成可以直接部署到 GitHub Pages 的版本。

## 你需要做的事

1. 在 GitHub 新建一个仓库
2. 把这个文件夹里的全部内容上传到仓库
3. 仓库默认分支使用 `main`
4. 进入 GitHub 仓库页面：
   `Settings -> Pages`
5. 在 `Build and deployment` 里选择：
   `Source: GitHub Actions`
6. 提交代码后，GitHub 会自动执行 `.github/workflows/deploy.yml`

## 已经帮你处理好的内容

- `vite.config.js`
  已设置 `base: './'`，避免静态资源路径导致页面打不开

- `.github/workflows/deploy.yml`
  已配置 GitHub Pages 自动部署

## 本地构建命令

```bash
npm install
npm run build
```

## 说明

如果你后面把仓库名改掉，这个版本也不用再额外改路径配置，直接还能用。
