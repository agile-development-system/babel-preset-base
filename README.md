<p align="center">
    <img src="https://gitee.com/agile-development-system/agds-doc-preset/raw/master/lib/docs/logos/light/1.png" alt="logo">
</p>

# @agds/babel-preset-base

**版本** ：1.0.1

基础babel配置

## 快速开始

### 安装

```bash
npm i -D @agds/babel-preset-base
```

### 引入

```js
// babel.config.js
module.exports = {
    presets: ['@agds/babel-preset-base'],
};
```






<a name="source"></a>

## 配置源码

```js
module.exports = function (api) {
    api.cache(true);
    const presets = [
        [
            '@babel/preset-env',
            {
                targets: {
                    node: '12',
                },
            },
        ],
    ];

    const plugins = [
        ['@babel/plugin-proposal-decorators', { legacy: true }],
        ['@babel/plugin-proposal-class-properties', { loose: false }],
        ['@babel/plugin-transform-modules-commonjs'],
    ];

    return {
        presets,
        plugins,
    };
};
```




<a name="license"></a>

## 许可证

[MIT License](https://gitee.com/agile-development-system/gulppreset/blob/master/LICENSE)
Copyright (c) 2021 锦阳



<a name="donate"></a>

## 请维护者喝杯咖啡

<img src="https://gitee.com/agile-development-system/agds-doc-preset/raw/master/lib/docs/qrcode/alipay.jpeg" width="209px" >
<img src="https://gitee.com/agile-development-system/agds-doc-preset/raw/master/lib/docs/qrcode/wechatpay.jpeg" width="237px" >




<a name="dingtalk"></a>

## 加入钉钉群讨论或加入开发

<img src="https://gitee.com/agile-development-system/agds-doc-preset/raw/master/lib/docs/qrcode/dingtalk.jpeg" width="188px" >


