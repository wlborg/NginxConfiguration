
# 说明
这个是服务器上nginx及其相关组件的配置说明文档，此文档的目录树结构使用`mddir`生成：

```
# 安装mddir
npm install mddir -g
# 进入项目根目录然后直接mddir生成目录树
cd dircotry 
mddir
```

## 目录和文件说明

|-- 根目录
    |-- `README.html`
    |-- `README.md` `说明文件`
    |-- `conf` `配置目录`
        |-- `503.conf` `维护配置文件`
        |-- `anti_spam_bots.conf` `屏蔽垃圾蜘蛛或者爬虫`
        |-- `baidusearch.conf` `百度站内搜索本地化`
        |-- `gongshang.conf` `应对工商查询`
        |-- `guard_dedecms.conf` `dedecms 织梦系统防护配置`
        |-- `m.yourdomain.com.pagespeed.conf` `移动端pagespeed配置文件`
        |-- `mobile2pc.conf` `移动端跳到PC端` 
        |-- `nginx.conf` `nginx主配置文件`
        |-- `nocached.conf` `禁止服务器和浏览器缓存文件配置`
        |-- `pc2mobile.conf` `PC跳转移动端配置`
        |-- `secure_cors.conf` `HTTPS安全和跨域配置`
        |-- `www.yourdomain.com.pagespeed.conf` `PC端pagespeed配置`
        |-- `vhost` `虚拟主机配置目录`
            |-- `m.yourdomain.com.conf` `移动端主机`
            |-- `www.yourdomain.com.conf` `PC端主机`

## 文件说明

除了`vhost`内是主要的配置文件，以及`nginx.conf`主配置外，其他的配置文件都属于“增强模块”，可以依据情况引入。

如果要使用`pagespeed`配置文件，则必须安装`pagespeed`组件

推荐的最基本配置文件是：
`anti_spam_bots.conf`
`guard_dedecms.conf`
`nocached.conf`
`pc2mobile.conf`
`secure_cors.conf`





