### cnpm
* 如果项目中已经存在一个低版本的包，如果执行 cnpm install 不会更新包的最新版本
* 如果执行 cnpm install --save（或-S，也可以是 -dev）则将会对齐进行覆盖



### npm
* npm install 不加任何参数即会自动记录到 package.json 中（默认 -S 的效果）
* npm 在以上 cnpm 的两种情况中，不需要加参数即可对 package.json 中对应的依赖包进行更新并记录。


### 建议
* 不建议直接使用 cnpm 问题太多...
* 推荐是将使用 npm 但是将镜像源切换至 cnpm 的地址，依旧使用 npm 下包
* 查看 npm 默认仓库地址

```
npm config get registry 
- https://registry.npmjs.org/
```

* 改变默认地址，并检查

```
npm config set registry https://registry.npm.taobao.org
npm config get registry 
- https://registry.npm.taobao.org/
```