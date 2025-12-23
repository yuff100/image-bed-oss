<h1 align="center"> OSS图床 | monorepo </h1>

<p align="center"><img width="160px" src="./packages/client/public/favicon.ico"/></p>

<p align="center">基于 对象存储服务（OSS）搭建的图床应用，<strong>前端纯静态，无需后端</strong></p>

<p align="center">支持 <a target="_blank" href="https://www.qiniu.com/products/kodo">七牛云</a> | <a target="_blank" href="https://www.upyun.com/products/file-storage">又拍云</a></p>

## Docker 镜像
```sh
docker run -d -p 8090:80 --restart unless-stopped --name image-bed-app sugarjl/image-bed:latest
```
应用将在 http://localhost:8090 可访问
