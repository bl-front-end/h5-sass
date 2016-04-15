# h5-sass

_h5-btn.scss按钮的使用方法

* 引用已经定义好的按钮

``` sass
// button-primary行内按钮
.button-primary {
	@extend %button-small-primary;
}

or

// block-small块状按钮
.block-button-primary {
	@extend %block-button-small-primary;
}

or

// 圆角按钮small按钮
.outline-button-radius-primary {
	@extend %outline-button-small-radius-primary;
}

or

// outline-block按钮
.outline-block-button-primary {
	@extend %outline-block-button-small-primary;
}
```

* 自己组件按钮样式，先要引入基础的按钮样式，再分别引入％bg-color-primary、％color-primary、％button-small、％font-size-small、％border-radius-small，分别定义的是背景颜色、文字颜色、按钮padding、字体大小、边框圆角、

``` sass
.button-primary {
	@extend %button-small-primary;
	@extend %bg-color-primary;
	@extend %color-primary;
	@extend %button-small;
	@extend %font-size-small;
	@extend %border-radius-small; /* 不加border-radius-small默认无圆角 */
}
```

** 按钮大小定义了三种small、middle、big，按钮颜色定义了primary、danger、dark三种颜色 **
