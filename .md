
[返回首页](http://www.caoyangyang.cn/)
# ng-if or ng-show
最近几次总是掉入同一个坑，就是关于一个很简单的指令
ng-if以及ng-show，被坑的原因在于每次都忘记了ng-if会创建一个独立的scope（和很多自定义指令一样哦）
上来那个张图，注意观察scope的id，以及parent scope的id，一切明了

![ng-show-example](http://caoyangyang.cn/img/demo/ng-show.png)

![ng-if-example](http://caoyangyang.cn/img/demo/ng-if.png)

真相大白了吧，ng-if确确实实创建了一个scope，然后它的parent还是上层parent的root。

测试页面
[test](http://caoyangyang.cn/demo/compare-ng-if-and-ng-show.html)

