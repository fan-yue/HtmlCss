# css边框

指定元素边框的样式、宽度和颜色。

1、每个内容后者元素外面都可以有一个边框。

2、边框分为上边框（top）,下边框（bottom），左边框（left）,右边框（right）。

3、每种边框有颜色(color),样式(style),宽度(width)三种属性 。

4、如果上下左右的边框表现不一样,可以分别定义上下左右边框,如果一样可以 统一使用border属性定义。



## border-style 边框类型

指定要显示的边框类型。

```
.one{
    border-style: solid;
}

选择器{
		border-style: solid;
		属性：border-style
		属性值：
				none : 	  默认值
        dotted ： 定义点线边框
        dashed ： 定义虚线边框
        solid ：  定义实线边框
        double ： 定义双边框
        groove ： 定义 3D 坡口边框。效果取决于 border-color 值
				ridge ： 定义 3D 脊线边框。效果取决于 border-color 值
				inset ： 定义 3D inset 边框。效果取决于 border-color 值
				outset ： 定义 3D outset 边框。效果取决于 border-color 值
				hidden ： 定义隐藏边框。
				
				混合边框： solid double dashed dotted;
				(
				如果提供全部四个参数值，将按上－右－下－左的顺序作用于四个边框。
				如果提供两个，第一个用于上－下，第二个用于左－右。
				
				如果提供三个，第一个用于上，第二个用于左－右，第三个用于下。)
}
```

### border-top-style

设置要显示的上边框的样式

```
border-top-style: solid;
border-right-style: dotted;
border-bottom-style: solid;
border-left-style: groove;
```

### border-right-style

设置要显示的右边框的样式

### border-bottom-style

设置要显示的下边框的样式

### border-left-style

设置要显示的左边框的样式



## border-width 边框宽度

指定四个边框的宽度。

```
.a{
    border-style: solid;
    border-width: 10px;
}
选择器{
		border-width: 10px;
		属性： border-width
		属性值：
          medium : 　默认宽度
      		thin : 	小于默认宽度
     		 	thick : 　大于默认宽度
      		数值（重点） :  由浮点数字和单位标识符组成的长度值。不可为负值。请参阅长度单位
      			混合宽度：1px 2px 3px 4px;
      			
      			(如果提供全部四个参数值，将按上－右－下－左的顺序作用于四个边框。
      			
      			如果提供两个，第一个用于上－下，第二个用于左－右。
				
						如果提供三个，第一个用于上，第二个用于左－右，第三个用于下。)
}

```

### border-top-width

设置上边框的宽度

```
border-top-width: 5px;
border-right-width: 10px;
border-bottom-width: 15px;
border-left-width: 20px;
```

### border-right-width

设置右边框的宽度

### border-bottom-width

设置下边框的宽度

### border-left-width

设置左边框的宽度

## border-color 边框颜色

可以通过以下方式设置颜色：

- name - 指定颜色名，比如 "red"
- 指定十六进制值，比如 "#ff0000"
- RGB - 指定 RGB 值，比如 "rgb(255,0,0)"

```
.a{
    border-color: aqua;
}
选择器{
		属性：border-color
		
		属性值：颜色
		
			混合颜色使用：aqua red green yellow;
			
			(如果提供全部四个参数值，将按上－右－下－左的顺序作用于四个边框。
      			
      如果提供两个，第一个用于上－下，第二个用于左－右。
				
			如果提供三个，第一个用于上，第二个用于左－右，第三个用于下。)
}
```

### border-top-color

设置上边框的颜色

```
border-top-color: yellow;
border-right-color: tomato;
border-bottom-color: violet;
border-left-color: blue;
```

### border-right-color

设置右边框的颜色

### border-bottom-color

设置下边框的颜色

### border-left-color

设置左边框的颜色

# border 复合属性，简写形式

```
.one{
   	border:1px solid black;	//不分先后顺序
   
}
选择器{
		属性：border
		
		属性值：
		
			宽度：数值,单位px
			
			边框属性：
				none : 	  默认值
        dotted ： 定义点线边框
        dashed ： 定义虚线边框
        solid ：  定义实线边框
        double ： 定义双边框
        
      边框颜色：颜色。
      	- name - 指定颜色名，比如 "red"
				- 指定十六进制值，比如 "#ff0000"
				- RGB - 指定 RGB 值，比如 "rgb(255,0,0)"
}
```

### border-top

顶部边框的复写属性

```
border-top: 1px solid green;
```

### border-right

```
border-rihgt: 1px solid green;
```

### border-bootom

```
border-bottom: 1px solid green;
```

### border-left

```
border-left: 1px solid green;
```



# border-radius

用于向元素添加圆角边框

```
.one{
   border-radius: 10px/10%;
}

选择器{
	属性：border-radius
	属性值：
		1、数值，单位px。(使用较多)
		2、百分比，%。
}
```

### border-top-right-radius

给边框右上角添加圆角边框

### border-top-left-radius

给边框左上角添加圆角边框

### border-bottom-right-radius

给边框右下角添加圆角边框

### border-bottom-left-radius

给边框左下角添加圆角边框