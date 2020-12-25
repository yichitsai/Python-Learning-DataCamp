# Matplotlib
> ### Visualization
> ### Data structure
> ### Control structures



---

## Line Plot
```
import matplotlib.pyplot as plt
plt.plot(x,y) # x:x-axis ; y:y-axis
plt.show()
```
```
pyplot is subpackage of matplotlib
```

#### Show the plot
```
plt.show()
```

### Change to a logarithmic scale
```
object = plt.xscale('log')
```



---

## Histogram
> ### Explore Dataset
> ### Get idea about distribution

---

![](https://i.imgur.com/bGsRfGY.png)

---
```
import matplotlib.pyplot as plt
```
```
plt.hist(values,bins)
```
#### Clean up plot
```
plt.clf()
```

### 註解：
```
arr: 需要計算直方圖的一維陣列

bins: 直方圖的柱數，可選項，預設為10

normed: 是否將得到的直方圖向量歸一化。預設為0

facecolor: 直方圖顏色

edgecolor: 直方圖邊框顏色

alpha: 透明度

histtype: 直方圖型別，‘bar’, ‘barstacked’, ‘step’, ‘stepfilled’

```

#### Compare
```

```