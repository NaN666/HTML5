# CSS3 复习总结
### 1.伪类
- E:nth-child(n/2n/odd/even) E元素中的第（n/2n/奇数、偶数）个节点；
- E:nth-last-child(n/2n/odd/even) 从后往前

- E:nth-of-type(n/2n/odd/even) 表示E父元素中的第n个子节点，且类型为E
- E:first-child/last-child    
- E:first-of-type/last-of-type
- E:after/before  生成内容在元素最前/最后
- E:not(选择器) 排除
- E~F 表示E后面的F元素
### 2.弹性盒模型
display：box 定义弹性和模型    
- **box-orient**：horizontal/vertical 水平/垂直  方向  
- **box-direction**：normal/reverse  正序/反序    
- **box-direction-group**  设置元素的具体排列顺序

```
<style>
    div{display:box;box-orient:horizontal;}
    div:nth-child(1){box-direction-group:3}
    div:nth-child(2){box-direction-group:1}
    div:nth-child(3){box-direction-group:2}
</style>
```
- **box-flex** 弹性和模型的弹性空间（用于==自适应屏幕==）  
- **box-pack** 水平富余空间管理（start/end/center/justify）    
    - start 》左浮动  end 》右浮动 center 》居中 justify 》富余空间在元素之间平局分布    
- **box-align** 垂直方向的富裕空间管理    
- **box-shadow**：  [inset] x y 模糊半径 [扩展半径] 颜色    
- **box-reflect**： 倒影 
    - direction方向  above | below | left | right
距离   渐变（可选）
- **resize**： 自由缩放 both / horizontal / vertical
- box-sizing 盒模型解析
    - content-box  标准盒模型 width/height = border + padding + content
    - border-box 怪异盒模型 width=content

### 别的一些
- **text-overflow**：文字溢出显示省略号   
    - clip：无省略号；    
    - ellipsis:有省略号；（配合overflow：hidden与- while-space：nowrap强制一行使用）
- **background：lineaer-gradient（）；** 线性渐变
    - （起点，点，点）； 
- **background：radial-gradient** 圆心渐变
- **background-origin**：border-box | padding-box | content-box 从什么位置开始显示背景
- **background-clip**：border-box | padding-box | content-box | text 从什么地方那个开始显示背景
- mask 遮罩 
    - img position repeat