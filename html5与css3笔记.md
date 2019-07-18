# 前段笔记
---
#### html5与css3的基础<br>
1. animation 动画，<br>
2. border-repeat:repeat 背景图像在纵向和横向上平铺<br>
3. z-index 元素堆叠<br>
4. box-shodw 阴影类型<br>
5. box-shodw：10px 20px 10px blue；
第一个值是x轴长度，第二个值是y轴长度，第三个值是阴影模糊半径，第四值是阴影颜色<br>
##### css新增知识<br>
1. 旋转rotate（50deg）元素顺时针旋转45度<br>
2. 变动skew（xdeg）水平方向弯曲，x轴不动，y轴逆时针旋转xdeg
3. 位移translate（）<br>
4. 变大变小scale（）<br>
##### 过度效果<br>
transition: width 2s linear 0.5s;为transition设置了四个值：第一个值是设置过渡属性;第二个值是设置过渡时间;第三个值是设置过渡函数，这个函数可以设置过渡效果是以怎么样的方式运动，linear表示运输运动。第四个值表示延时时间，在上面的例子中，鼠标悬浮后经过0.5秒后元素才开始运动。<br>
##### 动画效果<br>
###### css3动画的基本语法：<br>
1. 我们需要用@keyframes定义一个动画，在上面的代码中，我们定义的动画名字为anim。<br>
2. 在花括号中定义动画的具体细节，0%位起始状态，100%为结束状态，我们也可以用其他的百分比定义动画在不同阶段的不同状态。<br>
3. 需要在元素选择器中调用这个动画，animation属性可以调用动画，第一个值是动画名称，后面的三个值分别是动画的时间，动画函数和延时时间，这个与我们之前学的过渡效果设置方法很类似。<br>
###### 动画效果<br>
1. 定义动画  @keyframes定义一个简单的动画<br>
2. 循环动画  nimation-iteration-count属性设置动画播放的次数，如果值为infinite<br>
3. 停止动画 animation-play-state属性让动画停止
