## xy-pop - alert - 提示框

### 使用

```javascript
vm.$xyPop.alert( content, [options] )
```

### 配置参数

参数|类型|说明|默认值
:-|:-:|-|:-:
content|string/html|内容|''
options|Object|配置|
└─ showTitle|Boolean|是否显示标题|true
└─ title|string|标题|'提示'
└─ confirmText|string|确定按钮文字|'确定'
└─ confirmNotHide|Boolean|手动确认|false
└─ onConfirm|Function|确认回调|

### 返回值

类型|说明
:-:|-
Boolean|是否确认

### slot

类型|说明
:-:|-
默认|内容处
title|标题处
btns|按钮处


### 代码示例

<iframe
     src="https://codesandbox.io/embed/romantic-glade-br789?fontsize=14&hidenavigation=1&initialpath=%2F%23%2Falert&module=%2Fsrc%2Fviews%2Falert.vue&theme=dark"
     style="width:100%; height:750px; border:0; border-radius: 4px; overflow:hidden;"
     title="romantic-glade-br789"
     allow="accelerometer; ambient-light-sensor; camera; encrypted-media; geolocation; gyroscope; hid; microphone; midi; payment; usb; vr; xr-spatial-tracking"
     sandbox="allow-autoplay allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"
   ></iframe>

## xy-pop - confirm - 确认框

### 使用

```javascript
vm.$xyPop.confirm( content, [options] )
```

### 配置参数

参数|类型|说明|默认值
:-|:-:|-|:-:
content|string/html|内容|''
options|Object|配置|
└─ showTitle|Boolean|是否显示标题|true
└─ title|string|标题|'提示'
└─ confirmText|string|确定按钮文字|'确定'
└─ cancelText|string|取消按钮文字|'取消'
└─ confirmNotHide|Boolean|手动确认|false
└─ onConfirm|Function|确认回调|
└─ onCancel|Function|取消回调|

### 返回值

类型|说明
:-:|-
Boolean|是否确认

### slot

类型|说明
:-:|-
默认|内容处
title|标题处
btns|按钮处

### 代码示例

<iframe
     src="https://codesandbox.io/embed/romantic-glade-br789?fontsize=14&hidenavigation=1&initialpath=%2F%23%2Fconfirm&module=%2Fsrc%2Fviews%2Fconfirm.vue&theme=dark"
     style="width:100%; height:750px; border:0; border-radius: 4px; overflow:hidden;"
     title="romantic-glade-br789"
     allow="accelerometer; ambient-light-sensor; camera; encrypted-media; geolocation; gyroscope; hid; microphone; midi; payment; usb; vr; xr-spatial-tracking"
     sandbox="allow-autoplay allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"
   ></iframe>

## xy-pop - toast - 消息提示

### 使用

```javascript
vm.$xyPop.toast( content, [options] )
```

### 配置参数

参数|类型|说明|默认值
:-|:-:|-|:-:
content|string/html|内容|''
options|Object|配置|
└─ time|number|持续时间|1500
└─ type|'success'/'fail'/'warn'|类型|''
└─ img|string|图片地址|''

### slot

类型|说明
:-:|-
默认|内容处
icon|图标处

### 代码示例

<iframe
     src="https://codesandbox.io/embed/romantic-glade-br789?fontsize=14&hidenavigation=1&initialpath=%2F%23%2Ftoast&module=%2Fsrc%2Fviews%2Ftoast.vue&theme=dark"
     style="width:100%; height:750px; border:0; border-radius: 4px; overflow:hidden;"
     title="romantic-glade-br789"
     allow="accelerometer; ambient-light-sensor; camera; encrypted-media; geolocation; gyroscope; hid; microphone; midi; payment; usb; vr; xr-spatial-tracking"
     sandbox="allow-autoplay allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"
   ></iframe>

## xy-pop - loading - 加载提示

### 使用

```javascript
vm.$xyPop.loading( [options] )
```

### 配置参数

参数|类型|说明|默认值
:-|:-:|-|:-:
options|Object|配置|
└─ msg|string|内容|''
└─ mask|Boolean|是否显示遮罩层|false
└─ img|string|图片地址|''

### 代码示例

<iframe
     src="https://codesandbox.io/embed/romantic-glade-br789?fontsize=14&hidenavigation=1&initialpath=%2F%23%2Floading&module=%2Fsrc%2Fviews%2Floading.vue&theme=dark"
     style="width:100%; height:750px; border:0; border-radius: 4px; overflow:hidden;"
     title="romantic-glade-br789"
     allow="accelerometer; ambient-light-sensor; camera; encrypted-media; geolocation; gyroscope; hid; microphone; midi; payment; usb; vr; xr-spatial-tracking"
     sandbox="allow-autoplay allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"
   ></iframe>

## xy-lazyload - 图片懒加载

## xy-image-pop - 图片查看器

## xy-slider - 轮播容器

## xy-list-status - 列表加载状态栏

## xy-html-viewer - html容器

## xy-spinner - 加载指示器

## xy-scroll-bottom - 页面滚动到底

## xy-timer - 当前时间

## xy-timing - 计时

## xy-timing - 持续时间

## xy-countdown - 倒计时