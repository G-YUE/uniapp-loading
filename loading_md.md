## 关于这个
- 一个普普通通的页面加载动画:-)
- 学习css动画

属性|类型|说明
:--|:--:|---
shadeShow|Boolean|是否显示遮罩层
shadeClick|Boolean|遮罩层是否可点击
custom|Boolean|是否自定义内容
type|Number|1：圆圈加载。2：矩形加载
width|String|弹出框框宽度
height|String|弹出框框高度
backgroundColor|String|弹出框框背景色
callback|Function|回掉函数

## 用法
```
<loading 
	ref="loading"
	:custom="false"
	:shadeClick="true"
	:type="1"
	@callback="callback()">
		<!-- <view class="test">自定义</view> -->
</loading>

js
close:function(){
	this.$refs.loading.close();
},
open:function(){
	this.$refs.loading.open();
},
callback(){
	console.log("回掉");
}
```