
<p align="center">
  <a href="https://24ta.com/?g">
    <img src="src/assets/logo.png" width="130" />
  </a>
  <br />
  <b>发现导航</b>
  <p align="center">一个纯静态、支持SEO、在线编辑的强大导航网站，希望您会喜欢</p>
  <p align="center">内置收录多达 800+ 优质网站， 助您工作、学习和生活</p>
  <p align="center">
    <img src="https://img.shields.io/github/v/release/xiaoqy/nav" />
    <a href="https://github.com/xjh22222228/nav/stargazers"><img src="https://img.shields.io/github/stars/xiaoqy/nav" alt="Stars"/></a>
    <img alt="Angular" src="https://img.shields.io/static/v1.svg?label=&message=Angular11&style=flat-square&color=C82B38">
    <img src="https://img.shields.io/github/license/xiaoqy/nav" />
    <a href="https://hits.dwyl.com/xiaoqy/nav">
      <img src="https://hits.dwyl.com/xiaoqy/nav.svg" />
    </a>
  </p>
</p>

<br />
<br />


## 选择版本
目前有2个版本供选择, [v3](https://github.com/xiaoqy/nav/tree/v3) 和 `v5`, 这2个版本都会长期维护:

- v5 - 也就是当前分支, 需要依赖于Github配置, 提供自动维护数据功能(微后台)，但必须Fork到自己仓库里。
- v3 - 无需依赖Github, 您可以将代码部署在任意服务器, 但数据需要手工维护。

作者推荐您选择 `v5` 没有太多的心智负担。



## 预览
**主题**

- [Sim 在线预览](https://24ta.com/#/sim)
- [Light 在线预览](https://24ta.com/#/light)

![Preview](https://raw.githubusercontent.com/xiaoqy/public/gh-pages/nav/1.png)
![Preview](https://raw.githubusercontent.com/xiaoqy/public/gh-pages/nav/2.png)
![Preview](https://raw.githubusercontent.com/xiaoqy/public/gh-pages/nav/3.png)
![Preview](https://raw.githubusercontent.com/xiaoqy/public/gh-pages/nav/4.png)
![Preview](https://raw.githubusercontent.com/xiaoqy/public/gh-pages/nav/5.png)




## 拥有出色的特性
`发现导航` 的理念就是做一款无需依赖后端服务既简单又方便，没有繁杂的配置和数据库等配置概念, 做到开箱即用。

- 🍰 内置 `800+` 实用网站。
- 🍰 支持SEO, 没有可不行。
- 🍰 完全纯静态, 提供自动化部署功能。
- 🍰 三叉树分类、结构清晰、分类清晰。
- 🍰 颜值与简约并存，不再是杀马特时代。
- 🍰 支持多种浏览模式，创新。
- 🍰 支持足迹记忆。
- 🍰 支持移动端浏览。
- 🍰 支持搜索查询。
- 🍰 支持自定义引擎搜索。
- 🍰 完全开源，轻松定制化。
- 🍰 多款主题切换。
- 🍰 支持暗黑模式。
- 🍰 支持快捷键操作，一步到位。
- 🍰 支持在线新增数据, 没有传统的后台概念。



## 部署
推荐使用 `github pages` 服务, 这样就不需要提供服务器, 并且项目里自带了自动化部署服务，像数 `321` 一样简单。

1、Fork 当前项目。

2、[https://github.com/settings/tokens](https://github.com/settings/tokens) 申请 token, 勾选相应的权限, 如果不懂就全部选中，复制并保存Token。

3、到 https://github.com/用户名/nav/settings/secrets/new  添加刚刚申请的token， name填写 `TOKEN` 大写。

4、打开 https://github.com/用户名/nav/actions 点击 `绿色按钮`

5、务必修改项目配置文件 [nav.config.ts](nav.config.ts)

6、5分钟后打开 https://用户名.github.io/nav 就能看到一个非常强大的导航网站了。


注：如果想部署到自己的域名，那么以上教程同样适合，因为它提供了自动化部署， 之后可以通过 `CNAME` 或 `反向代理` 实现：

```conf
# nginx

server {
    listen       80;
    server_name  www.24ta.com 24ta.com;

    location / {
        proxy_pass https://xiaoqy.github.io/nav/;
    }
}
```


## 配置
所有可配置位于文件 `nav.config.ts`。




## 关于升级
在升级之前请保存根目录下的 `data` 文件夹,最好把 `nav.config.ts` 配置文件也保存一份以防万一, 升级完后替换即可。

点击右上角 `Watch` 按钮第一时间跟踪版本升级。



## 更新日志
[CHANGELOG](CHANGELOG.md)




## 快捷键
mac下是 `Command`，windows 下是 `Ctrl`

- `ctrl+e` 开启或关闭编辑模式
- `ctrl+v` 查看信息
- `ctrl+d` 开启或关闭暗黑模式

如对快捷键有特殊要求请发起 [issues](https://github.com/xiaoqy/nav/issues)





## 开发构建
``` bash
# 下载
git clone --depth=1 https://github.com/xiaoqy/nav.git

# 安装依赖
npm i

# 启动
npm start

# 打包
npm run build
```



## 建议
如果有任何功能上的建议可通过 [issue](https://github.com/xiaoqy/nav/issues) 发起, Thank you.



## 支持
项目成立于 2020 年到至今一直坚持维护和开源, 经过N次的迭代与优化, 如果项目能帮到您是我的荣幸。

您可以请作者喝杯咖啡，继续战斗下去（请备注Github名字）~

支付宝：1052406629@qq.com
微信：ixiaoqy

感谢您的认可：
| 姓名    | 支持金额              |
| --------------------------------------- |----------- |
| [Cyrus Xiao](https://github.com/xiaoqy)     | ￥20.00     |

