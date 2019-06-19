



## Base map

![1000](/Users/jinsanity/OneDrive - UWM/Documents/Uproduct/TSIS/Taiyuan/1000.bmp)

Marker size: 1



### Base map 导出分辨率，比例设置 

* 1000dpi
* 37.901418823 N; 37.790607907 S;
* 112.478512273 W ; 112.610530348 E；

![image-20190529160630797](/Users/jinsanity/Library/Application Support/typora-user-images/image-20190529160630797.png)

![image-20190605104342717](https://ws2.sinaimg.cn/large/006tNc79ly1g3qplhxih7j30lg0huk8k.jpg)

![image-20190605104753767](https://ws4.sinaimg.cn/large/006tNc79ly1g3qpppi77dj30lu0h2tpj.jpg)

太原经纬度(北纬，东经)

37.8706° N, 112.5489° E

### Distance calculator 

* [Distance Calculator | Distance Between Coordinates](https://gps-coordinates.org/distance-between-coordinates.php) 
* [Coordinate Distance Calculator](http://boulter.com/gps/distance/) 

长度：

From

* N 37.901418823 W 112.478512273 

To

* S 37.790607907 W 112.478512273 



Result from [Distance Calculator | Distance Between Coordinates](https://gps-coordinates.org/distance-between-coordinates.php)   



GPS Coordinates 1

| **Latitude**  | 37.901418823  |
| ------------- | ------------- |
| **Longitude** | 112.478512273 |

GPS Coordinates 2

| **Latitude**  | 37.790607907  |
| ------------- | ------------- |
| **Longitude** | 112.478512273 |

The distance is between the two gps coordinates is 
**12.32** KM or 
**7.66** Miles or 
**6.65** Nautical miles or 
**12321.61** meters 

= 40425.229659 feet



宽度(WE)：

Result from [Distance Calculator | Distance Between Coordinates](https://gps-coordinates.org/distance-between-coordinates.php)   



GPS Coordinates 1

| **Latitude**  | 37.901418823  |
| ------------- | ------------- |
| **Longitude** | 112.478512273 |

GPS Coordinates 2

| **Latitude**  | 37.901418823  |
| ------------- | ------------- |
| **Longitude** | 112.610530348 |

The distance is between the two gps coordinates is 
**11.58** KM or 
**7.20** Miles or 
**6.25** Nautical miles or 
**11583.33** meters

= 

38003.051181 feet



### 将base map 导入 TSIS







## TSIS 建网

### 主干道

辅助点作图法：

![image-20190529170205521](https://ws3.sinaimg.cn/large/006tNc79ly1g3ix6xqgj6j308406p76l.jpg)



国道307 

89之后

![image-20190530152650614](https://ws2.sinaimg.cn/large/006tNc79ly1g3k023z0awj30mu0scamh.jpg)



* 264 高架 + 交叉口	
  * 265；266；267；269；143；154
* ![image-20190603141959539](https://ws1.sinaimg.cn/large/006tNc79ly1g3okls7c77j309e09xjvv.jpg) 

## 国道

[国道、省道、高速区别？如何快速识别高速,一些驾驶小常识？ - 知乎](https://www.zhihu.com/question/23458682) 

太原：

* G307
* G108



- [x] 绿波协调干线2



### 南北向主干道

* QGIS 中新列信息 [Using the Field Calculator](https://docs.qgis.org/3.4/en/docs/user_manual/working_with_vector/attribute_table.html#id31)[¶](https://docs.qgis.org/3.4/en/docs/user_manual/working_with_vector/attribute_table.html#using-the-field-calculator) 

从东往西第二条： WE02

![image-20190530151504434](https://ws3.sinaimg.cn/large/006tNc79ly1g3jzpwc1q0j30gg0dhwti.jpg)

![image-20190530151528332](https://ws3.sinaimg.cn/large/006tNc79ly1g3jzq938t4j30sy0pkn9c.jpg)



从东往西第三条： WE03 finished 

![image-20190603103929635](https://ws4.sinaimg.cn/large/006tNc79ly1g3oe8m1m97j30m40it1i6.jpg)

Corsim 中途补充点:

* 编号从6001 开始

![image-20190603104228003](https://ws1.sinaimg.cn/large/006tNc79ly1g3oebgz201j304z07gdhh.jpg)

从东往西第六条： WE06 finished

![image-20190603113008423](https://ws2.sinaimg.cn/large/006tNc79ly1g3ofp1zaeaj30vv0bhtqa.jpg)



国道 G208

One way or two-way ？？？

WE04 finished



WE05 finished  施工中🚧？？？



![image-20190603135310645](https://ws1.sinaimg.cn/large/006tNc79ly1g3ojtvxkjfj30ix0h8nf5.jpg)











WE07 

复杂路段；交叉口高架



难点

* 立交和路面道路高度重合
* 

![image-20190605144719150](https://ws2.sinaimg.cn/large/006tNc79ly1g3qwmt6uj3j30fg0caq5r.jpg)





## 新增OSM 节点路网文件

* 技术路线

  1. 筛选指定范围内（中环）的节点

  2. 区分freeway 和 surface

     1. node
     2. link

  3. 查看并测试trf文件中网络的基本组成单位

     1. as

  4. 根据已有道路网信息生成trf文件，

     1. ![image-20190604155522064](https://ws2.sinaimg.cn/large/006tNc79ly1g3pszam486j30tf0mf0v3.jpg)
     2. 挑战： 只有流量信息完全无误的网络才能被translate

  5. 根据trf 文件生成tno文件

     1. 直接用xml文件写回 tno格式
        ![image-20190605133618992](https://ws2.sinaimg.cn/large/006tNc79ly1g3qukxn45rj30p00r8ag6.jpg)

     2. Python  XML parser

        [document](/Users/jinsanity/OneDrive - UWM/Documents/Uproduct/TSIS/TNO/TNO_manipulation.md) 







![image-20190604132048159](https://ws4.sinaimg.cn/large/006tNc79ly1g3poigy53gj30c5078gm8.jpg)

![image-20190604132710841](https://ws2.sinaimg.cn/large/006tNc79ly1g3pop3y7srj30dg0g6402.jpg)

![image-20190604132629723](https://ws3.sinaimg.cn/large/006tNc79ly1g3pooedi5fj30ba03pjrh.jpg)

![image-20190604132138815](https://ws1.sinaimg.cn/large/006tNc79ly1g3pp8y6l0uj30bl03swel.jpg)





上下游节点关系



![image-20190604134604165](https://ws2.sinaimg.cn/large/006tNc79ly1g3pp8s1ys3j30sl0f9wm0.jpg)



* 下游： 4054893247 ； v
* 上游： 1397244273 ；u

导出bitmap

Node size: 0.2

Line size: 0.03

Scale !!!!: 29353



![image-20190605105542742](https://ws3.sinaimg.cn/large/006tNc79ly1g3qpxt7r3qj30gu0degnb.jpg)

### 立交的图形化展示

* 

![image-20190605161024737](https://ws3.sinaimg.cn/large/006tNc79ly1g3qz19tpxgj30yq0ro4dn.jpg) 

![image-20190605161043076](https://ws1.sinaimg.cn/large/006tNc79ly1g3qz1k5rxqj30ad0cm74m.jpg)





## Interchange bugs

[Interchange tutorials ](/Users/jinsanity/OneDrive - UWM/project/Summer campus/CORSIM Materials/Lab mterials/Sim Lab Session 5 - instruction.pdf) 



* Ramp divergence
  * ![image-20190612101434853](https://ws2.sinaimg.cn/large/006tNc79ly1g3ys3faw1qj30kl0ih0th.jpg)
  * ![image-20190612101505461](https://ws2.sinaimg.cn/large/006tNc79ly1g3ys3prp1zj30ei0fxwmy.jpg)把ramp上的分叉节点当变成mainline上的两个节点来处理
  * 

