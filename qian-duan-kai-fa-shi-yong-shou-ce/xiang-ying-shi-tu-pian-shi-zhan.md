# 响应式图片实战

### 什么是响应式图片

响应式图片是指在不同设备或不同屏幕尺寸下，为网页或应用程序中的图片提供不同大小或分辨率的优化版本，以便在各种设备上显示最佳效果。响应式图片的目的是在保持图片视觉质量的同时，提高页面加载速度和用户体验。



### 如何使用srcset属性来优化图片加载

使用srcset可以为图片提供不同分辨率和大小的版本，浏览器会根据设备屏幕分辨率自动选择最优图片进行加载。

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>scrset 响应式图片</title>
</head>
<body>
  <img
    src="./assest/xlarge.png"
    srcset="./assest/small.png 480vw,
            ./assest/medium.png 768vw,
            ./assest/large.png 1200vw,
            ./assest/xlarge.png 1600vw"
    sizes="(max-width: 480px) 100vw,
            (max-width: 768px) 50vw,
            33.3vw"
    alt="响应式图片"
  />
</body>
</html>
```
