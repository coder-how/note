# cli



定义了命令行的类

主要是针对启动时不同的参数，执行不同的函数

比如`build`、`preview`。（vite命令详见：https://cn.vitejs.dev/guide/cli.html）

一共注册了4个命令

```js
.command('[root]', 'start dev server')
.command('build [root]', 'build for production')
.command('optimize [root]', 'pre-bundle dependencies')
.command('preview [root]', 'locally preview production build')

```



