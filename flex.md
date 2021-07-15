
 父级:display:flex;
justify-content属性将这只青蛙引导到右侧的 lilypad，该属性将项目水平对齐并接受以下值：
flex-start：项目与容器的左侧对齐。
flex-end：项目与容器的右侧对齐。
center：项目在容器的中心对齐。
space-between：项目以相等的间距显示。
space-around：项目以相等的间距显示。

align-items
align-items是设置子元素(伸缩项)在侧轴方向上的对齐方式
##父元素设置的属性
center 设置在侧轴方向上居中对齐
flex-start 设置在侧轴方向上顶对齐
flex-end 设置在侧轴方向上底对齐
stretch 拉伸
让子元素在侧轴方向上进行拉伸，填充满整个侧轴方向，
注意盒子不要有高度值
baseline文本基线
align-self设置单个元素在侧轴上的对齐方式


flex-flow
flex-flow:=flex-wrap: + flex-direction:

简写属性
flex-wrap:控制子元素是否换行显示，默认不换行
nowrap不换行，仍然收缩显示
wrap换行

flex-direction:设置子元素的排列方向

就是用来设置主轴(默认横轴)方向
默认主轴方向是row
row水平方向排列，从左至右
row-reverse水平方向排列，从右至左
column垂直方向排列，从下至上
column-reverse垂直方向排列，从上至下
有时候元素显示排版有问题，可以互换 
flex-grow:可以来扩展子元素的宽度

对子元素进行设置
flex-grow:的默认值为0:说明子元素不会去占据剩余的空间
具体是用来设置当前元素占据剩余空间的比例值
比例值计算 : (当前空间的flex-grow)/(所有兄弟元素的flex-grow的和)
{order:数值}