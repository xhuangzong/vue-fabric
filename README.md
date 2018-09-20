# vue-fabric
purestart vue-fabric.

## Installation
```
npm install vue-fabric --save
```

## Import
```
在main.js中
import 'vue-fabric/dist/vue-fabric.min.css';
import { Fabric } from 'vue-fabric';
```
```
Vue.use(Fabric);
```

使用

```
 <vue-fabric ref="canvas" :width="width" :height="height"></vue-fabric>
```

## Usage
#### Props
| Name              | Type               | Default             | Description                                         |
| ----------------| ---------------- | ---------------| ------------------------------------------|
| width             | Number            |  ''                | canvas width    |
| height				| Number		| ''               | canvas height |


## Function
#### createImage(url,options) 绘制图片
| params              | Type             | Description                                         |
| ----------------| ----------------| ------------------------------------------|
| url             | String            | image url    |
| options             | Object            | width,height,left,top |

#### createTextbox(text,options) 绘制文本
| params              | Type             | Description                                         |
| ----------------| ----------------| ------------------------------------------|
| text             | String            | text content    |
| options             | Object            | width,left,top,fill,fontSize, |

#### createRect(width,height,fillColor,left,top) 绘制矩形
| params              | Type             | Description                                         |
| ----------------| ----------------| ------------------------------------------|
| left             | Number            | left    |
| top             | Number            | top |
| width             | Number            | Rect width    |
| height             | Number            | Rect height |
| fillColor             | String            | Rect fillColor |


#### createLine(x,y,x1,y1,fillColor,strokeColor) 绘制直线
| params              | Type             | Description                                         |
| ----------------| ----------------| ------------------------------------------|
| x,y,x1,y1             | Number            | line points,直线两点坐标    |
| fillColor             | String            | fillColor 填充颜色 |
| strokeColor             | String            | strokeColor 绘制颜色 |

## Changelog
### 2018.8.26
> v0.1.4 * 初始化组件库
