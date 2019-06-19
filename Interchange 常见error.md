

### FATAL ERROR - 2083 

Description:

* Usually happens at the corner

```
FATAL ERROR - 2083 - Illogical channelization code for lane 1 of link (104,105).  Check Record Type 11
```



![image-20190619140727458](https://ws1.sinaimg.cn/large/006tNc79ly1g4725odhppj30b70d60sp.jpg)

**Reason**:

One direction turn movement can not be unresrited 

**Solution**:

Change lane channelization code according to `node` properties : eg.105  

Open Tno file

Search `<NumericLabel>105`

**List**:

~~*  FATAL ERROR - 2083 - Illogical channelization code for lane 1 of link (104,105).  Check Record Type 11~~

* ~~FATAL ERROR - 2083 - Illogical channelization code for lane 2 of link (140,141).  Check Record Type 11.~~

* ~~FATAL ERROR - 2083 - Illogical channelization code for lane 2 of link (6002,123).  Check Record Type 11.~~

* **~~FATAL ERROR - 2083 - Illogical channelization code for lane 1 of link (251,252).  Check Record Type 11~~**
* ~~FATAL ERROR - 2083 - Illogical channelization code for lane 2 of link (8006,292).  Check Record Type 11.~~
* ~~FATAL ERROR - 2083 - Illogical channelization code for lane 2 of link (8007,297).  Check Record Type 11.~~
* ~~FATAL ERROR - 2083 - Illogical channelization code for lane 1 of link (372,373).  Check Record Type 11.~~
* ~~FATAL ERROR - 2083 - Illogical channelization code for lane 1 of link (156,373).  Check Record Type 11~~
* ~~FATAL ERROR - 2083 - Illogical channelization code for lane 2 of link (156,373).  Check Record Type 11~~
* ~~FATAL ERROR - 2083 - Illogical channelization code for lane 1 of link (374,375).  Check Record Type 11.~~
* FATAL ERROR - 2083 - Illogical channelization code for lane 4 of link (8014,373).  Check Record Type 11.





### FATAL ERROR - 2084

```
FATAL ERROR - 2084 - Channelization code of 4 was entered for lane 2 on link (156,373).  Lane specified does not exist on this link.  Check Record Type 11.  Where channelization code: 0=unrestricted; 1=left turn only; 2= buses only; 3= closed; 4=right turn only; 5=carpool only; 6=carpools & busses; 7=right turns + (right, diagonal, and/or through); 8=left turns + (left, diagonal, and/or through); 9=all movements permitted by the geometry and adjacent lane channelization; 10 (or D)=diagonal traffic only; and 11 (or T)=through traffic only.

```



### FATAL ERROR - 2089 

```
FATAL ERROR - 2089 - A left receiver was specified for link (373,156) but the lane channelizations do not accommodate the left turn movement.
```

![image-20190619144238152](https://ws2.sinaimg.cn/large/006tNc79ly1g47368fbfcj30a808f3yo.jpg)

![image-20190619144714911](https://ws1.sinaimg.cn/large/006tNc79ly1g473b1f0n9j30f20893yf.jpg)

**Reasons**:

T intersection channeliztion 

**Solution**:

Same as `2089`

* Change channelization lane to one left and one right 

List

* FATAL ERROR - 2094 - A right receiver was specified for link (373,156) but the lane channelizations do not accommodate the right turn movement.





###  FATAL ERROR - 2091

```
 FATAL ERROR - 2091 - A diagonal receiver was specified for link (8014,373) but the lane channelizations do not accommodate the diagonal turn movement.
```

**Reasons**:

![image-20190619145828547](https://ws4.sinaimg.cn/large/006tNc79ly1g473mpkctbj30ah07mt8y.jpg)

**Solution**:

Change lane channelization like the intersection properties describes. eg.



### FATAL ERROR - 2094 

```
FATAL ERROR - 2094 - A right receiver was specified for link (373,156) but the lane channelizations do not accommodate the right turn movement.

```

**Reasons**:

T intersection channeliztion 

**Solution**:

Same as `2089`

- Change channelization lane to one left and one right 



****

### FATAL ERROR - 6500

Description:

```
FATAL ERROR - 6500 - Link (12,13) defined on Record Type 19 does not belong to any disjoint freeway segment.
```

![image-20190612103831686](https://ws3.sinaimg.cn/large/006tNc79ly1g3yssqtxcvj30u00eyjtd.jpg) 

Solution:







```
***** FATAL ERROR - 6500 - Link (28,2) defined on Record Type 19 does not belong to any disjoint freeway segment.

***** FATAL ERROR - 6500 - Link (11,7005) defined on Record Type 19 does not belong to any disjoint freeway segment.

***** FATAL ERROR - 6500 - Link (22,18) defined on Record Type 19 does not belong to any disjoint freeway segment.

***** FATAL ERROR - 6500 - Link (13,27) defined on Record Type 19 does not belong to any disjoint freeway segment.

***** FATAL ERROR - 6500 - Link (11,12) defined on Record Type 19 does not belong to any disjoint freeway segment.

***** FATAL ERROR - 6500 - Link (7007,22) defined on Record Type 19 does not belong to any disjoint freeway segment.

***** FATAL ERROR - 6500 - Link (6,7001) defined on Record Type 19 does not belong to any disjoint freeway segment.

***** FATAL ERROR - 6500 - Link (6,11) defined on Record Type 19 does not belong to any disjoint freeway segment.

***** FATAL ERROR - 6500 - Link (12,13) defined on Record Type 19 does not belong to any disjoint freeway segment.

***** FATAL ERROR - 6500 - Link (18,28) defined on Record Type 19 does not belong to any disjoint freeway segment.

***** FATAL ERROR - 6500 - Link (27,18) defined on Record Type 19 does not belong to any disjoint freeway segment.

***** FATAL ERROR - 6500 - Link (7008,29) defined on Record Type 19 does not belong to any disjoint freeway segment.

***** FATAL ERROR - 6500 - Link (29,27) defined on Record Type 19 does not belong to any disjoint freeway segment.

***** FATAL ERROR - 6500 - Link (2,31) defined on Record Type 19 does not belong to any disjoint freeway segment.

***** FATAL ERROR - 6500 - Link (31,8008) defined on Record Type 19 does not belong to any disjoint freeway segment.

***** FATAL ERROR - 6500 - Link (32,6) defined on Record Type 19 does not belong to any disjoint freeway segment.

***** FATAL ERROR - 6500 - Link (8001,32) defined on Record Type 19 does not belong to any disjoint freeway segment.
```

![image-20190614133215312](https://ws4.sinaimg.cn/large/006tNc79ly1g4191j19bdj30kg0m8q60.jpg)

[http://sites.poli.usp.br/ptr/lemt/CORSIM/CORSIMUsersGuide.pdf](http://sites.poli.usp.br/ptr/lemt/CORSIM/CORSIMUsersGuide.pdf) 





