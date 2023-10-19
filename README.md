此项目为 Base64 项目打包后生成的 Dist 包

配合 WebHooks 钩子 实现提交后自动同步至服务器的功能

如果直接打包至根目录，每次打包时，会清空包括 .git 文件夹的内容

所以把 dist 包放在此项目的 dist 文件夹内

VueConfigJS 配置为：

```js
module.exports = {
  // 打包至与此项目同级的Base64_build项目下的dist文件夹
  outputDir: '../Base64_build/dist',
}
```

服务器配置为：

网站运行文件夹为 `/Base64_build/dist`


