# 无Tag插件包名单

无Tag插件包指在版本发行中不标识版本号的包。打了Tag的包名是wp-china-yes.2.1.0.zip这样的形式，而未打Tag的包名就直接是wp-china-yes.zip。

可以发现，对于不打Tag的包，每个版本的名字都是一样的，这就导致即便版本更新了CDN依旧会返回旧版本的问题。

目前为了应对该问题，我们维护了这个“无Tag包名单”并通过 [无Tag包更新监听服务][0] 对其定期扫描，通常情况下，包有更新了会在30秒内全网刷新。

[0]: https://github.com/wp-china-yes/update-no-tag-package

需要特别说明一下，打不打Tag并不能代表其开发者的个人水平，这只是一个习惯问题而已，WordPress官方允许不打Tag。