# Flex 布局





## 主轴

### 知识

1. **什么是主轴 ？**

```
子元素排列的方向 
```

2. 常用排列方向有哪些 ？

```
row 水平
column 垂直
```

3. 如何设置主轴的方向

```css
flex-direction: row;
```



### Example 1

水平排列

```css
.container {
    /* 此处省略基础样式 */
    display: flex;
    flex-direction: row;
}
```

完整代码 [10.html](https://github.com/demodeom/flex/blob/main/10.html)

![image-20231230174021712](https://blog.image.codedemo.vip/image-20231230174021712.png)

### Example 2

垂直排列

完整代码 [11.html](https://github.com/demodeom/flex/blob/main/11.html)

![image-20231230175805397](https://blog.image.codedemo.vip/image-20231230175805397.png)

## 主轴元素排列方式

### 知识

1. 常用的排列方式

```
center	居中
space-between 两端对齐
space-around 
space-evenly 平均分配
flex-start 起点对齐
flex-end 重点对齐
```

2. 如何设置对齐方式

```css
justify-content: flex-end;
```



### Example 1

完整代码 [21.html](https://github.com/demodeom/flex/blob/main/21.html)

![image-20231230180427443](https://blog.image.codedemo.vip/image-20231230180427443.png)

### Example 2

完整代码 [22.html](https://github.com/demodeom/flex/blob/main/22.html)

![image-20231230180532749](https://blog.image.codedemo.vip/image-20231230180532749.png)

### Example 3

完整代码 [23.html](https://github.com/demodeom/flex/blob/main/23.html)

![image-20231230180650898](https://blog.image.codedemo.vip/image-20231230180650898.png)

### Example 4

完整代码 [24.html](https://github.com/demodeom/flex/blob/main/24.html)

![image-20231230181032614](https://blog.image.codedemo.vip/image-20231230181032614.png)

### Example 5

完整代码 [25.html](https://github.com/demodeom/flex/blob/main/25.html)

![image-20231230181127234](https://blog.image.codedemo.vip/image-20231230181127234.png)

### Example 6

完整代码 [26.html](https://github.com/demodeom/flex/blob/main/26.html)

![image-20231230181227859](https://blog.image.codedemo.vip/image-20231230181227859.png)

## 交叉轴

### 知识

**交叉轴**  垂直与主轴， 随主轴方向的变化而变化

### Example 1

完整代码 [31.html](https://github.com/demodeom/flex/blob/main/31.html)

![image-20231230181757178](https://blog.image.codedemo.vip/image-20231230181757178.png)

### Example 2

完整代码 [32.html](https://github.com/demodeom/flex/blob/main/32.html)

![image-20231230182005980](https://blog.image.codedemo.vip/image-20231230182005980.png)

## 交叉轴元素排列方式

### Example 1

完整代码 [33.html](https://github.com/demodeom/flex/blob/main/33.html)

![image-20231230184821608](https://blog.image.codedemo.vip/image-20231230184821608.png)

### Example 2

完整代码 [34.html](https://github.com/demodeom/flex/blob/main/34.html)

![image-20231230185002986](https://blog.image.codedemo.vip/image-20231230185002986.png)

### Example 3

完整代码 [35.html](https://github.com/demodeom/flex/blob/main/35.html)

![image-20231230185301365](https://blog.image.codedemo.vip/image-20231230185301365.png)



## 主轴上子元素换行



### Example 1

完整代码 [42.html](https://github.com/demodeom/flex/blob/main/42.html)

![image-20231230185553921](https://blog.image.codedemo.vip/image-20231230185553921.png)

### Example 2

完整代码 [43.html](https://github.com/demodeom/flex/blob/main/43.html)

![image-20231230185722268](https://blog.image.codedemo.vip/image-20231230185722268.png)

## 交叉轴元素排列方式（多轴）

> 当主轴元素换行之后， 相当于产生多条主轴， 对应的交叉轴也有多条

`aligin-content` 和 `align-item` 都可是设置交叉轴对齐方式

`aligin-content` 只有多轴的情况下才会生效

`align-item` 可用的属性值

- `start`
- `center`
- `end`

`aligin-content` 可用的属性值

- `flex-start`
- `space-between`
- `space-around`
- `space-evenly`
- `center`
- `flex-end`

```css
align-content: flex-start;
```


### Example 1 align-content

```css
.container {
    /* 此处省略基础样式 */
    display: flex;
    flex-direction: row;
    align-content: flex-start;
}
```

完整代码 [61.html](https://github.com/demodeom/flex/blob/main/61.html)

![火狐截图_2024-01-18T17-53-44.303Z](https://blog.image.codedemo.vip/火狐截图_2024-01-18T17-53-44.303Z.png)

### Example 2 align-content

完整代码 [62.html](https://github.com/demodeom/flex/blob/main/62.html)


```css
.container {
    /* 此处省略基础样式 */
    display: flex;
    flex-direction: row;
    align-content: flex-end;
}
```

![火狐截图_2024-01-18T17-54-00.667Z](https://blog.image.codedemo.vip/火狐截图_2024-01-18T17-54-00.667Z.png)

### Example 3 align-content

完整代码 [63.html](https://github.com/demodeom/flex/blob/main/63.html)

```css
.container {
    /* 此处省略基础样式 */
    display: flex;
    flex-direction: row;
    align-content: center;
}
```

![火狐截图_2024-01-18T17-54-10.424Z](https://blog.image.codedemo.vip/火狐截图_2024-01-18T17-54-10.424Z.png)

### Example 4 align-content

```css
.container {
    /* 此处省略基础样式 */
    display: flex;
    flex-direction: row;
    align-content: space-between;
}
```

完整代码 [64.html](https://github.com/demodeom/flex/blob/main/64.html)
![火狐截图_2024-01-18T17-54-24.041Z](https://blog.image.codedemo.vip/火狐截图_2024-01-18T17-54-24.041Z.png)

### Example 5 align-content

```css
.container {
    /* 此处省略基础样式 */
    display: flex;
    flex-direction: row;
    align-content: space-around;
}
```

完整代码 [65.html](https://github.com/demodeom/flex/blob/main/65.html)

![火狐截图_2024-01-18T17-59-42.479Z](https://blog.image.codedemo.vip/火狐截图_2024-01-18T17-59-42.479Z.png)

### Example 6 align-content

```css
.container {
    /* 此处省略基础样式 */
    display: flex;
    flex-direction: row;
    align-content: space-evenly;
}
```

完整代码 [66.html](https://github.com/demodeom/flex/blob/main/66.html)

![火狐截图_2024-01-18T17-59-55.556Z](https://blog.image.codedemo.vip/火狐截图_2024-01-18T17-59-55.556Z.png)



### Example 7 align-items

完整代码 [51.html](https://github.com/demodeom/flex/blob/main/51.html)



```css
.container {
    /* 此处省略基础样式 */
    display: flex;
    flex-direction: row;
    align-items: start;
}
```

![微信截图_20240119013621](https://blog.image.codedemo.vip/微信截图_20240119013621-1705602082722-10.png)



### Example 8 align-items

完整代码 [52.html](https://github.com/demodeom/flex/blob/main/52.html)

```css
.container {
    /* 此处省略基础样式 */
    display: flex;
    flex-direction: row;
    align-items: center;
}
```

![微信截图_20240119013757](https://blog.image.codedemo.vip/微信截图_20240119013757.png)

### Example 9 align-items



完整代码 [53.html](https://github.com/demodeom/flex/blob/main/53.html)

```css
.container {
    /* 此处省略基础样式 */
    display: flex;
    flex-direction: row;
    align-items: end;
}
```

![微信截图_20240119013716](https://blog.image.codedemo.vip/微信截图_20240119013716.png)

## 放大

### 知识

> 当主轴有剩余空间， 可以使用 `flex-grow` 属性放大元素， 默认值为 0 表示不放大

子元素放大后尺寸计算公式
$$
子元素放大后的尺寸 = \frac{主轴实际尺寸-子元素尺寸和}{子元素放大份数和} * 当前子元素放大份数 + 当前子元素的尺寸
$$








### Example 1

完整代码 [71.html](https://github.com/demodeom/flex/blob/main/71.html)

蓝色背景元素宽度放大结算结果

$$
蓝色背景元素最终宽度 = \frac{1280-(100+100+100+100)}{(1+1+1+1)} * 1 + 100 = 320
$$

![image-20240119013451302](https://blog.image.codedemo.vip/image-20240119013451302.png)



### Example 2



完整代码 [72.html](https://github.com/demodeom/flex/blob/main/72.html)


$$
蓝色背景元素最终宽度 = \frac{1280-(100+100+100+100)}{(3+1+1+1)} * 3 + 100 = 540
$$

![image-20240119013507226](https://blog.image.codedemo.vip/image-20240119013507226.png)

## 缩小


### 知识

> 当主轴空间不足时， 可以使用 `flex-shrink` 属性缩小元素， 默认值为 1，

子元素缩小后尺寸计算公式
$$
子元素放大后的尺寸 = \frac{主轴实际尺寸-子元素尺寸和}{子元素缩小份数和} * 当前子元素缩小的份数 + 当前子元素的尺寸
$$




### Example 1

完整代码 [81.html](https://github.com/demodeom/flex/blob/main/81.html)

蓝色背景元素宽度放大结算结果

$$
蓝色背景元素最终宽度 = \frac{1280-(500+500+500+500)}{(1+1+1+1)} * 1 + 500 = 320
$$



![image-20240119013405380](https://blog.image.codedemo.vip/image-20240119013405380.png)

### Example 2



完整代码 [82.html](https://github.com/demodeom/flex/blob/main/82.html)


$$
蓝色背景元素最终宽度 = \frac{1280-(500+500+500+500)}{(3+1+1+1)} * 3 + 500 = 140
$$



![image-20240119013429067](https://blog.image.codedemo.vip/image-20240119013429067.png)












