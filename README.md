# nm-deploy-http-push

## 说明

本插件来源于FIS 默认的部署插件，提供本地部署以及远程upload部署能力

## 使用方法

也可以使用统一的 deploy 插件配置方法

```js
fis.match('*.js', {
    deploy: fis.plugin('http-push', {
        //如果配置了receiver，fis会把文件逐个post到接收端上
        receiver: 'http://www.example.com:8080/receiver.php',
        //这个参数会跟随post请求一起发送
        to: '/home/xxx/www'
    })
})
```
