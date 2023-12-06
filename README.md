# GitDataV

GitDataV is a github "big data visualization platform" through which you can more intuitively see some of your data in github:
- Personal information (✔), warehouse stars status (✔), warehouse language classification (✔)
- Warehouse public number (✔), number of fans (✔), number of followers (✔), warehouse data (✔), recent operations (✔)
- Recent fans (✔), recent followers (✔), latest information (✔)
Small easter egg with arrow in the upper left corner: full screen (✔), international language switching (✔), return to home page (✔), skin switching (under development...)


[GitDataV online demonstration use](https://hongqingcao.github.io/GitDataV/)

(ps: The online demonstration is dev.1.0 version, with more functions, you can switch to dev.2.0 or master branch clone to run locally)

###### ![Instance effect](https://user-gold-cdn.xitu.io/2018/8/24/1656c59629551995?w=1954&h=934&f=gif&s=3919397)
###### ![Instance effect](https://user-gold-cdn.xitu.io/2019/7/9/16bd4cd0238a41ba?w=1897&h=940&f=png&s=494477)
 
### Development log

- [2018-09 DEV1.0](https://github.com/HongqingCao/GitDataV/tree/dev1.0)
- [2019-05 DEV2.0 Refactor](https://github.com/HongqingCao/GitDataV/tree/dev2.0)
- [2019-08 DEV2.0 Add number scrolling effect](https://github.com/HongqingCao/GitDataV/tree/dev2.0)

## Build and setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report

# run unit tests
npm run unit

# run all tests
npm test
```

## error 

```
opensslErrorStack: [ 'error:03000086:digital envelope routines::initialization error' ]
```

```
export NODE_OPTIONS=--openssl-legacy-provider
```


## Project directory structure  

``` bash
├── README.md                 Project Introduction
├── vue.config.js             Project configuration
├── deploy.sh                 Deployment files
├── package.json              npm package configuration file, which defines the project's npm script, dependent packages and other information
├── src                       Source code directory  
│  ├── main.js                Entry js file
│  ├── router.js              routing
│  ├── store.js               vuex status
│  ├── app.vue                root component
│  ├── components             Public component directory
│  │  └── index.js            Traverse all components
│  ├── lang                   Language switching dictionary
│  │  └── index.js            Language switching dictionary
│  ├── assets                 Resource directory, the resources here will be built by wabpack
│  │  └── css                 css basic reset
│  │  └── data                Pictures required for visual interface
│  │  └── iconfont            Font icon
│  │    └── bg.png
│  └── views                  Page directory
│    ├── app                  Entry file
│    └── data                 visualization file
├── static                    Pure static resources will not be built by wabpack.
```

## 相关链接  
- ["Using Vue to build a github "visual big data platform"-GitDataV, design and development sharing" (Nuggets)](https://juejin.im/post/5b7f6cd46fb9a019f709b17b)

## Technical points
- vue (vue project construction, flexible use of instructions, component encapsulation, communication between components)
- vue-router (preliminary knowledge of routing: difference between hash and history, dynamic routing, routing switching parameters)
- vuex, vue-i18n (language switching)
- Network request axios (encapsulate axios yourself, cross-domain proxy configuration)
- Visual tools echarts and v-charts handle graphics (control size, layout, color, accept data format)
- es6 (basic syntax, such as map traversal of arrays, object and array conversion, etc. used in the process of sorting out data)
- scss (configuration, syntax)
- bootstrap, iconfont (used when there is no designer and the front-end design ability is limited, so these two are quoted)

## License

MIT