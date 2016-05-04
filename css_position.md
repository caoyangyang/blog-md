[返回首页](http://www.caoyangyang.cn/)
#几句话说CSS的position
position 属性有四，字面意思很简单，就是负责页面元素定位的
* static
* relative
* absolute
* fixed

```
static为默认的 ，可以理解为常规顺序的布局方式
relative 相对，相对于原来默认的位置，重新定位
absolute 绝对，其实也是相对，相对于最近的一个position属性为relative父元素进行定位，这句话有点绕，
fixed 固定，其实还是相对，相对于视窗位置，所以看上去是绝对。
```

其实就是一个默认，三个相对，只是相对的元素不一样，有的是`默认原来的`那个自己，有的相对的是`外面`某个罩着自己的老大（父元素），有的相对的是`看得见`的部分 。





