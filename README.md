# 基于 SVG 实现城市景观动态效果

注：设计图来源网络。

动画列表：

 - CSS：太阳的光芒、云朵、飞机、热气球、小汽车、摩天轮和字体。
 - SMIL：小鸟。

[体验地址>>](http://jdc.jd.com/lab/urban_landscape/)

预览图：

![城市景观](http://7xq7nb.com1.z0.glb.clouddn.com/jdc.jd.com-lab-urban_landscape-%28iPad%29%202.png)

实现过程：

 1. 将设计图源文件导入 AI/Sketch 等编辑器，然后对元素进行编辑（根据动画细粒度对元素进行分割）并导出为 SVG 文件。注：Sketch 操作简单，导出的 SVG 代码简洁且易于更改。
 2. （可选）将导出后的 SVG 代码在 [SVGOMG](https://jakearchibald.github.io/svgomg/) 进行优化。注意：优化会更改代码，若在添加动画后再优化可能会导致动画失效等问题。
 3. 将相关元素按需求进行手动编辑（如编组）。
 4. 对于变形（morphing）动画（如小鸟动画），要求**点**的数量相同，否则无过渡效果。当然，使用 [Snap.svg](http://snapsvg.io/) 之类的库可以免除此限制。
