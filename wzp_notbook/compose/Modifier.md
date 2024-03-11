# modifier作用
1. [[#修改Compose控件的尺寸，布局，行为和式样]]
2. [[#为Compose控件添加额外的信息]]
3. [[#处理用户的输入]]
4. [[#4 添加上层交互逻辑]]


# 1: 修改Compose控件的尺寸，布局，行为和式样
![[Pasted image 20240130162056.png]]

 使用说明：Compose的外观都是由Modifier控制，当需要更改外观时，应使用此属性。


# 2: 为Compose控件添加额外的信息

一般是为Accessibility和Test使用

# 3: 处理用户的输入

该输入不是用户文本的输入，而是指的是用户的手指在屏幕上进行滑动，各种点击操作时的动作（它被视为一种输入）
![[Pasted image 20240130170306.png]]


# 4: 添加上层交互逻辑
## 使控件可点击、滚动、拖拽

让一个控件可点击，不一定必须使用pointerInput()函数，clickable()函数也能做到
![[Pasted image 20240130170654.png]]

## 使控件可滚动

![[Pasted image 20240130170906.png]]

## 拖动

![[Pasted image 20240130172419.png]]
注意⚠️：此种方式只适用于在一个方向上滑动，水平或者垂直方向

## 任意方向滑动应使用较底层的pointerInput()实现

![[Pasted image 20240130173352.png]]

# 注意事项

1. [串接顺序](https://guolin.blog.csdn.net/article/details/132253342)
2. 任何一个Composable函数它的第一个非强制参数都应该是Modifie


