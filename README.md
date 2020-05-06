> 官网: [https://haomo-tech.com](https://haomo-tech.com)

> 作者: 毫末科技

> 邮箱: hxg@haomo-studio.com

## 预览

![预览图片](http://downloads.haomo-tech.com/uniapp/hm-task-list-card.png)

[在线效果预览](http://template.uniapp.haomo-tech.com/pages/haomo/test-component/hm-task-list-card)

更多毫末科技的uni-app跨端模板，请见[毫末科技uni-app跨端模板](https://haomo-tech.com/sale.html)

## 技术支持
我们公司提供超低价的切图服务哈。移动端平均50元每个页面，PC Web端平均80元每个页面。目前支持出vue、react、uniapp、taro、flutter、小程序代码代码，代码支持自适应。其中uniapp、taro一份代码支持多端。app原生会在五月份开始支持。示例demo: [http://edu.uniapp.haomo-tech.com](http://edu.uniapp.haomo-tech.com)。部分样例代码：[http://downloads.haomo-tech.com/uniapp-demo.zip](http://downloads.haomo-tech.com/uniapp-demo.zip)

* [uni-app插件市场](https://ext.dcloud.net.cn/plugin?id=1527)

* [npm包](https://www.npmjs.com/package/hm-uniapp-task-list-card)

* [github地址](https://github.com/haomo-studio/hm-uniapp-task-list-card)

* [gitee地址](https://gitee.com/haomo/hm-uniapp-task-list-card)

毫末科技将长期迭代本组件。需要技术支持，请进钉钉群（群号30423559）：

<img width="250" src="http://downloads.haomo-tech.com/%E6%AF%AB%E6%9C%ABuniapp%E7%BB%84%E4%BB%B6%E6%8A%80%E6%9C%AF%E6%94%AF%E6%8C%81.jpg">

## 概述

毫末uni-app毫末任务列表卡片组件。支持H5/小程序(微信、支付宝、头条、百度、QQ)/App；组件可自适应各种屏幕大小的手机。

## 使用

请使用HBuilderX导入组件。

在script中引用：

```javascript
import HmTaskListCard from '@/components/hm-task-list-card/index.vue'
export default {
    components: { HmTaskListCard }
}
```

在template中使用：

```html
<template>
  <div class="test-component">
    <hm-task-list-card :options="options"></hm-task-list-card>
  </div>
</template>
<script>
import HmTaskListCard from '@/components/hm-components/hm-task-list-card/index.vue'

export default {
  components: { HmTaskListCard },
  data() {
    return {
      options: {
          text: 'P',
          projectMeeting: '项目会议',
          word: '…',
          num: '2019年2月26日下午2:29',
          loremIpsumPrev: '在出版和设计中，',
          loremIpsum: 'lorem ipsum',
          isPlaceholder: '是一个占位',
          characterText: '符文本。',
          side:
            '/static/hm-task-list-card/images/img_25847_0_0.png'
        }
    };
  },
  methods: {
    onClick: function(e) {
      console.log('onClick');
    }
  }
};
</script>
<style>
</style>

```

## 属性说明

| 属性名        | 类型     | 默认值 | 说明                                                                       |
|-----------   |---------|--------|----------------------------------------------------------------------------|
| options        | Object  | -      | 卡片属性                                                                   |

options对象各个属性说明如下：

| 属性名        | 类型     | 默认值 | 说明                                                                       |
|-----------   |---------|--------|----------------------------------------------------------------------------|
| projectMeeting        | String  | -      | 标题文字                                                                   |
| num        | String  | -      | 时间                                                                   |
| loremIpsumPrev        | String  | -      | 文本                                                                   |
| side        | String  | -      | 状态图片                                                                   |

## 事件说明

| 事件称名   | 事件说明           | 返回参数 |
|----------|--------------------|----------|
| @click   | 点击 Card 触发事件 | -        |

## 更新日志

### 0.0.1(2020-03-28)

* 完成第一个版本