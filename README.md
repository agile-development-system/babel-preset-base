# @ads/babel-preset-base
**版本** ：1.0.0
基础babel配置

## 快速开始

### 安装
```bash
npm i -D @ads/babel-preset-base
```

### 引入
```js
// babel.config.js
module.exports = {
    presets: ['@ads/babel-preset-base'],
};
```


 <!-- 渲染后缀内容  -->



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



