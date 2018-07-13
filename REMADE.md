### CSS3的复习
#### CSS3的伪类选择器
* :frist-child 选择元素的第一个子元素
* :last-child 选择元素的最后一个子元素
* :nth-child() 括号中填写数字，选择当前元素中的某个指定子元素
* :nth-last-child() 同上，但是是从下往上找
* :nth-of-type()  指定的同类元素的第几个
* :nth-last-of-type() 同上，但是从后往前
* :first-of-type 选择 指定元素的第一个
* :last-of-type 选择指定元素的最后一个
* :only-child 选择的子元素是唯一的
* :only-of-type 选择一个元素是父元素下的唯一一个类型的子元素
* :empty 选择的元素没有任何内容

* :first-letter 第一个文字
* :first-line 第一行
* :after
* :before 如果使用这个。first-就会失效

#### CSS3transform
* border-radius 减少了网站维护量，提高了行呢，增加了美观
* transform属性
    > rotate() // 角度
    
    > skew() //倾斜

    > translate() // 偏移

    > scale() //  缩放

#### css3的渐变
* linear-gradient   线性渐变 如果不写方向，默认从上到下
* radial-gradient   径向渐变 默认从内到外

* 在之前加repeating实现重复
```
.item7{
        border-radius: 0;
        background: repeating-linear-gradient(red 0px,green 10px,yellow 20px);
    }
    .item8{
        background: repeating-radial-gradient(red 0px,green 5px,yellow 10px)
    }

```

#### css3的transition属性
* transition-property   过渡属性 （默认all） 
* transtion-duration    过度持续时间 (默认值为0)
* transition-timing-function 过度函数（ease，ease-out）
* transtion-delay  过度延迟时间

#### CSS3的animate
* @keyframes  定义动画
* animation-name        动画名称
* animation-duration    动画时间
* animation-timing-function 动画
* animation-delay   延迟(如果要动画更流畅就可以设置负值)
* animation-iteration-count  循环动画可以设置循环次数
* animation-direction   动画反过来（normal和alternate）
* animation-fill-mod    动画完成以后的状态(none,forwards,backwards,both )

#### CSS3的 字体效果
* text-shadow 阴影
* text-overflow 解决文字排版问题
```
<!-- 通过3行代码实现省略号 -->
text-overflow:ellipsis;
overflow:hidden;
white-spance:nowrap;

<!-- 多行文本溢出省略 -->
overflow : hidden;
text-overflow: ellipsis;
display: -webkit-box;
-webkit-line-clamp: 2;
-webkit-box-orient: vertical;
```