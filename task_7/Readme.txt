1.动画过渡，color
	-webkit-transition:color 0.4s ease-in-out;
    -moz-transition:color 0.4s ease-in-out;
    transition:color 0.4s ease-in-out;
2.背景图片自适应的问题：
	background-image: url(../image/cha.jpg);
	background-size: 100% 100%;
	宽高都设为100%！
3.margin设置外边框，想让盒子左右居中显示，上下固定，
如果margin: 10px auto;无效的话，可以这样margin: 10px 45%;
margin的属性值可以是百分数。
4.选中ul下面的每一个li用nth-child()，如：
			.part2_icon li:nth-child(1) span{				
				background-image: url(../image/beetle.png);	
			}
			.part2_icon li:nth-child(2) span{				
				background-image: url(../image/llama.png);
			}
			.part2_icon li:nth-child(3) span{				
				background-image: url(../image/monkey.png);
			}
			.part2_icon li:nth-child(4) span{				
				background-image: url(../image/dogg.png);
			}
5.其他属性选择器也可以这么玩，如：
			.part4_mes p:first-child {
				font-size: 35px;
			}
			.psrt4_mes p:last-child {
				font-size: 25px;
			}
6.表单的下拉选择：input的list属性和datalist的id属性一样就可以了，datalist是HTML5 的特性，虽然使用起来比较简单，但是在设置样式的时候比较复杂，我尝试了很多种方法都不行
			<label for="">
				<input type="text" list="country" placeholder="国家">
			</label>
			<datalist id="country">
				<option value="中国"></option>
				<option value="美国"></option>
			</datalist>
7.图片自适应div的方法：
			.part5_img img {
				width: auto;
				height: auto;
				max-width: 100%;
				max-height: 100%;
			}
4行的意思是：
width:auto;图片的宽度自己适应(图片有多宽就显示多宽)
height:auto;图片的高度自己适应(图片有多高就显示多高)
width:auto;和height:auto;一起使用就代表着显示图片的原始尺寸(可以理解为没有什么作用)
max-width:100%;图片的宽度不能超过图片所在的空间的宽度
max-height:100%;图片的高度不能超过图片所在的空间的高度
max-width:100%;max-height:100%;一起使用就代表这图片的宽高尺寸最大不能超过它所在的空间的宽高。

8.box-sizing:border-box;
	为元素设定的宽度和高度决定了元素的边框盒。
	就是说，为元素指定的任何内边距和边框都将在已设定的宽度和高度内进行绘制。
	通过从已设定的宽度和高度分别减去边框和内边距才能得到内容的宽度和高度。
 box-sizing:content-box;
 	宽度和高度分别应用到元素的内容框。
	在宽度和高度之外绘制元素的内边距和边框。

9.z-index: 10;
	z-index堆叠顺序，高的堆叠顺序的元素在前面

10.vertical-align 属性设置元素的垂直对齐方式。