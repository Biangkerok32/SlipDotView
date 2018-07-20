# SlipDotView
## 说明
###### *这是一个自定义view+发布+编写readme的练习*<br>
参考了网上的各种教程写了一个viewpager下面的小圆点，样式如下<br>
<img src="https://github.com/whcGH/SlipDotView/blob/master/slip_dot_view_example.jpg" width="108" height="192" alt="图片加载失败"/><br>
## 使用
首先
```
 allprojects {
    repositories {
        ...
        maven { url 'https://jitpack.io' }
    }
}
```
然后
```
  dependencies {
        implementation 'com.github.whcGH:SlipDotView:v1.0.4'
    }
```
布局
```
<com.test.library.SlipPointView
        android:id="@+id/spv"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content" />
```
## 属性说明
|属性名称|布局属性|对应方法|说明|
|:---|:---|:---|:---|
|半径|radius|setRadius()|圆点半径|
|间距|offsetSize|setOffsetSize()|圆点之间的距离|
|移动点长度|expendSize|setExpendSize()|不包括移动点两头的半径长度|
|个数|count|setCount()|圆点个数（包括被移动点覆盖的那一个）|
|圆点颜色|p_color|setPointColor()||
|移动点颜色|mp_color|setMovePointColor()||

## 版本说明
v1.0.4    --第一个发布成功的版本

###### *第一次发布，版本没有很好地控制，浪费了好几个版本号，所以从1.0.4开始...<br>从此知道了版本控制的重要性....<br>希望以后能顺利点.....*
