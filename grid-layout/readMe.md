# 创建网格
## 定义一个网格

display: grid
该属性只是会把布局设置网格布局，其中跟着的子项目会成为网格项


## 使用fr来灵活分配

fr 划分的是可用空间，不是所有空间。可用不是包括 已经被占用的空间。

## 网格间隙



## 重复构建行和列

使用repeat函数

比如
` grid-template-column: repeat(3,1fr)`


## 显式网格 隐式网格

使用grid-template-column grid-template-row 创建的网格是显式网格。

隐式网格 默认值 为auto，根据放入的内容自动调整。

## minmax()函数
minmax 函数为一个行/列的尺寸设置了取值范围
minmax()第一个值表示 至少的大小， 第二个值固定为 auto 表示根据内容自动调整。
\>=大于等于
尺寸就至少为 100 像素，并且如果内容尺寸大于 100 像素则会根据内容自动调整

## 自动使用多列填充。

# 基于线的元素放置。

分隔线
grid-column-start、grid-column-end、grid-row-start、grid-row-end  值为序号

简写： grid-column、grid-row  其中的值需要使用 '/' 来分隔开。其中 第一个为start 第二个为end



# 使用grid-template-area放置元素

## 规则
你需要填满网格的每个格子
对于某个横跨多个格子的元素，重复写上那个元素grid-area属性定义的区域名字
所有名字只能出现在一个连续的区域，不能在不同的位置出现
一个连续的区域必须是一个矩形
使用.符号，让一个格子留空