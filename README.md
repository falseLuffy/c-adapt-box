### 概览
    该组件提供了自适应屏幕尺寸，更好显示平铺布局；

### 参数
    gutter Number 必须  组件内块的间隙尺寸
    size   Number 必须  组件内块的宽度
    offset Number 非必须 表示该组件的父元素高度相对于屏幕总高度的偏移 如果希望组件可以自适应屏幕的高度，可传入该参数，


### 使用方法
```
    <adapt-box :data="data" :property="property"></adapt-box>

    import adaptBox from './adapt-box.js';

    {
      components:{
        adaptBox
      }
    }
```
```
  <adapt-box :gutter="30" :size="300" :offset="140">
    <div class="item"></div>
    <div class="item"></div>
    <div class="item"></div>
    <div class="item"></div>
    <div class="item"></div>
  </adapt-box>

  new Vue({
    el:'#app',
    methods:{

    },
    components:{
      AdaptBox:AdaptBox
    }
  })
```