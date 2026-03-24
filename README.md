<h1 align="center"> OSS图床 | monorepo </h1>

<p align="center"><img width="160px" src="./packages/client/public/favicon.ico"/></p>

<p align="center">基于 对象存储服务（OSS）搭建的图床应用，<strong>前端纯静态，无需后端</strong></p>

<p align="center">支持 <a target="_blank" href="https://www.qiniu.com/products/kodo">七牛云</a> | <a target="_blank" href="https://www.upyun.com/products/file-storage">又拍云</a></p>

## Docker 镜像

```sh
docker run -d -p 8090:80 --restart unless-stopped --name image-bed-app sugarjl/image-bed:latest
```

应用将在 http://localhost:8090 可访问

## Vercel 部署

本项目支持一键部署到 Vercel。

### 部署步骤

1. 点击上方按钮或在 Vercel Dashboard 导入本仓库
2. 选择 `packages/client` 作为根目录
3. 配置构建命令：`cd packages/client && npm run build`
4. 输出目录：`packages/client/dist`
5. 点击部署

### 环境变量

可选配置：

- `VITE_APP_UPLOAD_TOKEN` - 默认的七牛云/又拍云上传 Token

### 注意事项

- 部署后需要在浏览器中配置上传 Token 才能使用
- 建议使用自定义域名以获得更好的访问体验
