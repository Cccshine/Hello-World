# 360度立体展示

该demo实现随鼠标的拖拽而展示物品的不同角度
主要原理是利用onmousedown、onmousemove、onmouseup事件结合clientX实现拖拽，在拖拽过程中根据鼠标移动的像素值相应的显示不同的图片以实现旋转
由于图片比较多，所以采用预加载图片来提高流畅度
由于图片切换非常频繁，所以没有采用切换图片的src来实现视觉上的旋转，而是采用创建所有图片，然后隐藏其他图片显示当前图片的方式来实现视觉上的旋转
具体实现可以参见源码，注释写的很详细