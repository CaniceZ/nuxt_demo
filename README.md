# nuxt测试项目

## Build Setup

```bash
# install dependencies
$ yarn install

# serve with hot reload at localhost:8084
$ yarn dev

# 服务端渲染
$ yarn build
$ yarn start

# 静态文件渲染
$ yarn generate
```
```bash
# ssr部署
1.yarn build
2.打包.nuxt、package.json、nuxt.config.js为压缩文件
3.将压缩包上传到云服务器
4.在服务器解压
5.执行以下代码
$ yarn
$ nohup yarn start &
$ 回车
```
