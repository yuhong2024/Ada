利用“括号算法”解决杂交方式中的图谱问题

**Solving the mapping problem in the hybridization method by using the “bracket algorithm”**

# 背景引入

最近写作业的时候遇到这样的问题

![image-20250330110923642](C:\Users\wang\AppData\Roaming\Typora\typora-user-images\image-20250330110923642.png)



而以前或许也只学过AxB这样的

![image-20250330111028382](C:\Users\wang\AppData\Roaming\Typora\typora-user-images\image-20250330111028382.png)

那么我们该如何从最基础的不断进阶到复杂，甚至通用的"算法"呢。

今天我们就提出了一种用于解决这种问题的“杂交图谱括号算法”。



# 基础知识

首先，了解我们的科学问题。

杂交问题的提出和目的

![image-20250330111240787](C:\Users\wang\AppData\Roaming\Typora\typora-user-images\image-20250330111240787.png)

杂交育种的概念

![image-20250330111252906](C:\Users\wang\AppData\Roaming\Typora\typora-user-images\image-20250330111252906.png)

杂交方式

![image-20250330111348738](C:\Users\wang\AppData\Roaming\Typora\typora-user-images\image-20250330111348738.png)



![image-20250330111402620](C:\Users\wang\AppData\Roaming\Typora\typora-user-images\image-20250330111402620.png)



![image-20250330111412410](C:\Users\wang\AppData\Roaming\Typora\typora-user-images\image-20250330111412410.png)



![image-20250330111422273](C:\Users\wang\AppData\Roaming\Typora\typora-user-images\image-20250330111422273.png)

![image-20250330111432289](C:\Users\wang\AppData\Roaming\Typora\typora-user-images\image-20250330111432289.png)



![image-20250330111448453](C:\Users\wang\AppData\Roaming\Typora\typora-user-images\image-20250330111448453.png)



# 算法介绍



![image-20250330111550305](C:\Users\wang\AppData\Roaming\Typora\typora-user-images\image-20250330111550305.png)



括号算法的核心思想是，定位、分割、分组、逆推

1. 定位分割：找到大于等于2的数字做定位，其中2用圆圈标注，大于2的用倒三角标注
2. 集团分组：从头到尾，以倒三角（≥3）为分割点，用中括号分为不同集团，在后面的写法中，就是不同的一小团
3. 括号分组：不同集团内，从头到尾，以圆圈（=2）为分割点，用括号分为不同小组，每个小组就是一次单交组，实现降维处理
4. 数字杂交：以数字1为一次单交，对应写法中的”x"，然后与相邻的圆圈（2）周围的小组二交，再和相邻的集团（≥3）进行复交，并且不断递推，实现升维处理。

The core idea of the bracketed algorithm is to locate, segment, group, and backward push：

1. **positioning segmentation**: find the number greater than or equal to 2 to do positioning, where 2 with a circle labeled, greater than 2 with an inverted triangle labeling
2. **group grouping**: from beginning to end, inverted triangles (≥ 3) as a division point, with parentheses into different groups, in the back of the write-up, is a different group of small groups
3. **bracket grouping**: different groups, from head to tail, with a circle (= 2) as the division point, with brackets into different groups, each group is a single cross group, to achieve the dimensionality reduction process
4. **Digital hybridization**: take the number 1 as a single intersection, corresponding to “x” in the writing method, and then intersect with the neighboring groups around the circle (2), and then intersect with the neighboring groups (≥3), and continuously recursive, to realize the upward dimension processing.



# 问题解决

![image-20250330112235331](C:\Users\wang\AppData\Roaming\Typora\typora-user-images\image-20250330112235331.png)



# 写在最后

复杂的问题都有方法。

本算法引用格式：



# 参考

部分课件引用：西南大学超星课程，张建奎，《作物育种学》https://www.xueyinonline.com/detail/200426399

