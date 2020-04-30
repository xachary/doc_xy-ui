# directives - 指令

## xy-btn-act - 按钮动画

[效果示例](/demo/btn-act.html?_blank)

### 代码示例

#### 大小变化

``` html
<button v-xy-btn-act:style.scale>scale</button>
```

#### 颜色变化

``` html
<button v-xy-btn-act:style.color="'rgba(0, 0, 255, 0.2)'">color</button>
```

#### 颜色灰度

``` html
<button v-xy-btn-act:style.grayscale>grayscale</button>
```

#### 水波纹

``` html
<button v-xy-btn-act:style.wave="'rgba(255, 0, 0, 0.5)'">wave</button>
```

#### 禁用效果

``` html
<button v-xy-btn-act:style.scale disabled>disabled</button>
```

### 配置参数

v-xy-btn-act:style.[type]

选项|必填|说明
:-:|:-:|-
scale|是|大小变化
color|是|颜色变化
grayscale|是|颜色灰度
wave|是|水波纹

v-xy-btn-act:style.color = ""

参数|类型|必填|说明
:-:|:-:|:-:|-
color|CSS色值|是|点击按钮背景色变化效果

v-xy-btn-act:style.wave = ""

参数|类型|必填|说明
:-:|:-:|:-:|-
wave|CSS色值|是|点击按钮背景水波纹效果

## xy-pull-refresh - 下拉刷新

[效果示例](/demo/pull-refresh.html?_blank)

### 代码示例

``` html
<template>
  <div v-xy-pull-refresh="onPullRefresh">
  </div>
</template>

<script>
    export default {
        methods: {
            onPullRefresh(stop) {
                // 结束效果
                stop()
            }
        }
    }
</script>
```

### 配置参数

v-xy-pull-refresh = function(stop){}

类型|必填|说明
:-:|:-:|-
function|是|开始刷新回调

### 返回参数

类型|说明
:-:|-
function|结束效果方法

## xy-keep-top - 滚动保持置顶

[效果示例](/demo/keep-top.html?_blank)

### 代码示例

``` html
<template>
  <div>
      <div v-xy-keep-top></div>
  </div>
</template>
```

## xy-btn-loading - 按钮加载效果

[效果示例](/demo/btn-loading.html?_blank)

### 代码示例

``` html
<template>
    <button v-xy-btn-loading="loading" @click="onClick">Submit</button>

    <button v-xy-btn-loading.icon="loading" @click="onClick">Submit</button>

    <button v-xy-btn-loading.icon.keep="loading" @click="onClick">Submit</button>
</template>

<script>
    export default {
        data: {
            loading: false
        }
        methods: {
            onClick(stop) {
                loading = true
                // do somethind async
                loading = false
            }
        }
    }
</script>
```

### 配置参数

v-xy-btn-loading = true

类型|必填|说明
:-:|:-:|-
boolean|是|是否显示加载效果

v-xy-btn-loading.icon.keep = true

选项（可叠加）|说明
:-:|-
icon|只显示图标
keep|保持当前按钮宽度不变

## xy-loading - 内容加载过度动画

[效果示例](/demo/loading.html?_blank)

### 代码示例

``` html
<template>
    <div v-xy-loading="loading"></div>
    <div v-xy-loading="{loading:loading,color:#efefef}"></div>

    <div v-xy-loading.multiple="{loading:loading,color:#efefef,max:3,min:3}"></div>
</template>

<script>
    export default {
        data: {
            loading: false
        }
    }
</script>
```

### 配置参数

v-xy-loading = true

类型|必填|说明
:-:|:-:|-
boolean|是|是否显示加载效果

v-xy-loading = {loading:loading,color:#efefef}

参数|类型|必填|说明
:-:|:-:|:-:|-
loading|boolean|是|是否显示加载效果
color|CSS色值|否|加载填充背景色

v-xy-loading.multiple = {loading:loading,color:#efefef,max:3,min:3}

选项|说明
:-:|-
multiple|多行加载效果

参数|类型|必填|说明
:-:|:-:|:-:|-
loading|boolean|是|是否显示加载效果
color|CSS色值|否|加载填充背景色
max|number|是|区域最多的行数
min|number|否|加载填充效果的行数