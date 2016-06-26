# CSSsprite
css sprite(雪碧)图案例
### 学到的要点：
  * 1.雪碧图，就是将一个页面中所有涉及到的零星图片都包含到一张大图中，然后通过background-position 来设置坐标，注意，坐标应该是每个图片的高度，比如一个图片高度是24px；则第一张图片是background-position: 0 0;第二张图片就是background-position: 0 -24px;而且坐标一定是负值。
  * 2.适用的图片：静态图片，不随用户信息的变化而变化；小图片，图片容量较小；加载量比较大；一些大图不建议拼成雪碧图。
  * 3.拼成背景图的小图的坐标（x,y）一定为负值。
  
#### 用到雪碧图的好处：
* 1.能很好地减少网页的http请求，从而大大的提高页面的性能，这是CSS Sprites最大的优点。因为没请求一次，就会和服务器链接一次，建立链接需要额外的时间的。
* 2.解决了网页设计师在图片命名上的困扰，只需对一张集合的图片命名，不需要对每一个小图片进行命名，从而提高了网页制作效率。
* 3.只需要修改一张或少张图片的颜色或样式来改变整个网页的风格。
* 4.能减少图片的字节。


#### 缺点：
* 1.图片合并时，需要把多张图片有序的合理的合并成一张图片，并留好足够的空间防止版块出现不必要的背景
* 2.图片定位繁琐：开发时需要通过工具测量计算每个背景单元的精确位置。

demo的效果：http://htmlpreview.github.io/?https://github.com/yanjungan/CSSsprite/blob/master/demo.html

index1的效果：http://htmlpreview.github.io/?https://github.com/yanjungan/CSSsprite/blob/master/index1.html
