# 添加头像框微信小程序

## 功能
- 选择当前头像或本地图片进行合成
- 自动支持任意数量的头像框模版
- 支持对头像原图进行缩放操作

## 使用

- 将 `project.config.json` 中 `appid` 修改为自己的
- 将 `app.json`中 `navigationBarTitleText` 改为小程序标题
- `pages\index` 文件夹下
  - 将 `index.wxss` 中 `.container` 的 `background-color`改为背景色
    - 可添加 `background-image: url('url')`属性来设置背景图片
  - `index.wxml` 中
    - 将 `topImg` 的 `src` 改为头图的 url
    - 将 `bottomImg` 的 `src` 改为底图的 url
  - 将 `index.js` 中 `urls` 数组改为头像框图片的 url

- 在微信公共平台的 `开发管理-开发设置-服务器域名` 处添加两个 `downloadFile` 域名：

    1. 微信官方头像域名：`https://thirdwx.qlogo.cn`
    2. 图片资源的域名，如：`https://cloud.tsinghua.edu.cn`

## 参考
[Yonghui-Lee/profile_photo_editor_weChatApplet](https://github.com/Yonghui-Lee/profile_photo_editor_weChatApplet)
