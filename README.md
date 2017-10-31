<h1 align="center">Loaders.css</h1>

<p align="center">
  <img src="https://img.shields.io/npm/v/loaders.css.svg?style=flat-square">
  <img src="https://img.shields.io/bower/v/loaders.css.svg?style=flat-square">
</p>

流畅的css加载动画~

### 是什么？

[See the demo](http://lywqs.com/loader)

A collection of loading animations written entirely in css.
Each animation is limited to a small subset of css properties in order
to avoid expensive painting and layout calculations.

I've posted links below to some fantastic articles that go into this
in a lot more detail.

### 安装(install)

```
bower install loaders.css
```

```
npm i --save-dev loaders.css
```

### 使用(Usage)

##### Standard
- 引入 `loaders.min.css`
- 创建一个元素并添加动动画 (例如： `<div class="loader-inner ball-pulse"></div>`)
- 将适当的 div 插入 元素内部

##### jQuery (optional)
- Include `loaders.min.css`, jQuery, and `loaders.css.js`
- Create an element and add the animation class (e.g. `<div class="loader-inner ball-pulse"></div>`)
- `loaders.js` is a simple helper to inject the correct number of div elements for each animation
- To initialise loaders that are added after page load select the div and call `loaders` on them (e.g. `$('.loader-inner').loaders()`)
- Enjoy

### diy个性定制

##### 改变背景颜色

对正确的子 div们元素添加样式，如下

``` css
.ball-grid-pulse > div {
  background-color: orange;
}
```

### 支持的浏览器如下

支持所有最新版本的主要浏览器，并支持IE9。

注意: T不能正常运行 请参考： [issue](https://github.com/ConnorAtherton/loaders.css/issues/18).

IE 11  | Firefox 36 | Chrome 41 | Safari 8
------ | ---------- | --------- | --------
✔ | ✔ | ✔ | ✔

### 贡献

欢迎拉请求！创建另一个文件 `src/animations`
并加载 `src/loader.scss`.

在单独的选项卡运行 `gulp --require coffee-script/register`. 打开 `demo/demo.html`
在浏览器中就可以看到您的动画运行。

### 讨论

- http://www.paulirish.com/2012/why-moving-elements-with-translate-is-better-than-posabs-topleft/
- http://aerotwist.com/blog/pixels-are-expensive/
- http://www.html5rocks.com/en/tutorials/speed/high-performance-animations/
- http://frontendbabel.info/articles/webpage-rendering-101/

### 灵感来自于 loaders.css

A few other folks have taken loaders and ported them elsewhere.

- **React** - [Jon Jaques](https://github.com/jonjaques) built a React demo you can check out [here](https://github.com/jonjaques/react-loaders)
- **Angular** - [the-corman](https://github.com/the-cormoran/angular-loaders) created some directives for angular, as did [Masadow](https://github.com/Masadow) in [this pr](https://github.com/ConnorAtherton/loaders.css/pull/50)
- **iOS** - [ninjaprox](https://github.com/ninjaprox/NVActivityIndicatorView) and [ontovnik](https://github.com/gontovnik/DGActivityIndicatorView)
- **Android** - [Jack Wang](https://github.com/81813780/AVLoadingIndicatorView) created a library and [technofreaky](https://github.com/technofreaky/Loaders.CSS-Android-App) created an app

### 声明

版权所有（c）2016 wqs.

更多技术内容，关注微信公众号：'前端h5'

邮箱：wqs565@163.com


