# weixin-cli

> A Vue.js project

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```
# weixin项目
## 项目需求

  * 模块划分
    1. 头部（导航区）
       标题（title）

    2. 内容区

      * 流媒体的左右区域，相对称

      * 文字

        左右两列
        文字左右两侧的间距，左侧6px + 46px(头像+左箭头距离)，右侧46px，自适应（4h），如果全是英文，需要自动折行

        气泡会跟着文字变化而变化，气泡与文字的间距10px(3H)
        文字行间距1.5em

      * 语音
        最长65%，最短34%(4H)

      * 图片
          最多9张,每发送一张，图片的显示最宽51%，高度自适应。等比例缩放

      * 头像区域
          40*40，针对不规则图片处理方法：图片设置最大宽高40px，然后让其长条水平居中，竖条的垂直居中

      * 各功能区域的间隔15px

    3. 底部区域
      fixed 布局底部输入框，只需要开发文字输入



    4. 交互的需求细节

       * 语音播放结束后，动画结束播放
       * 当前语音继续点击时，真难听当前语音播放
       * 点击其他语音，先暂停所有语音动画（ 并且所有语音回归到三线状态）
       * 每次重复点击  语音都会重头播放



## 预先计划会

  * 讨论需求的可行性

  * 功能区域复杂度

  * 模块拆分

## 计划会（需求估时）

  * 头部模块 3h
  * 内容区 2d
  * 底部区 1d



## 开发
  * 架构
  * base，global
  * 业务模块
  * 切分支
  * 开发

## 交付
  * 自己测试（各种Android· iphone 机型测试）
  * 与UI比对，误差不超过3px
  * 发邮件，抄送给开发


## 联调
  * 与开发校验数据
  * 与QA调bug

## 上线
  * 运维

For detailed explanation on how things work, checkout the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).
