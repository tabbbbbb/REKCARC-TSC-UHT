


**时间限制：** 1 秒 


**空间限制：** 512 MB

**相关文件：** 题目目录





## 题目描述

生活在在外星球X上的小Z想要找一些小朋友组成一个舞蹈团，于是他在网上发布了信息，一共有 $n$ 个人报名面试。

**面试必须按照报名的顺序**依次进行。小Z可以选择在面试完若干小朋友以后，在所有**已经面试过**的小朋友中进行任意顺序的挑选，以组合成一个舞蹈团。

虽然说是小朋友，但是外星球X上的生态环境和地球上的不太一样，这些小朋友的身高可能相差很大。小Z希望组建的这个舞蹈团要求**至少**有 $m$ 个小朋友，并且这些小朋友的最高身高和最低身高之差不能超过 $k$ 个长度单位。

现在知道了这些小朋友的身高信息，问小Z至少要面试多少小朋友才能在已经面试过的小朋友中选出不少于 $m$ 个组成舞蹈团。

## 输入格式

从标准输入读入数据。

第一行 $3$ 个整数 $n,m,k$，意义见题面描述；$1 \le m \le n \le 10^{5}; 0 \le k \le 10^{5}$；

第二行 $n$ 个整数，第 $i$ 个数 $h_i$ 表示第 $i$ 个报名面试的小朋友的身高， $1 \le h_i \le 10^{5}$。

## 输出格式

输出到标准输出。

如果可以选出舞蹈团，输出**至少**要面试多少人；否则输出 `impossible`。






## 样例1输入

```plain
6 3 5
170 169 175 171 180 175

```



## 样例1输出

```plain
4

```


## 样例1解释
当面试了前$4$个小朋友之后，这些小朋友的身高分别为$170,169,175,171$，可选出身高为$170,175,171$的小朋友组成舞蹈团，故只用面试$4$个小朋友即可。






## 样例2输入

```plain
6 4 5
170 169 175 171 180 175

```



## 样例2输出

```plain
6

```


## 样例2解释
在这个样例中，小Z需要面试所有小朋友，才能选出身高为$170,175,171,175$的小朋友组成舞蹈团。






## 样例3输入

```plain
6 5 5
170 169 175 171 180 175

```



## 样例3输出

```plain
impossible

```


## 样例4

见题目目录下的 *4.in* 与 *4.ans*。

## 子任务

**本题目一共 $20$ 个测试点，所有测试点均不开启O2优化。**

 
	


<table class="table table-bordered"><thead><tr><th rowspan="1">测试点编号</th><th rowspan="1">$n, m$</th><th rowspan="1">$h_i, k$</th></tr></thead><tbody><tr><td rowspan="1">1,2</td><td rowspan="1">$1 \le m \le n \le 100$</td><td rowspan="1">$k=0;1 \le h_i \le 100$</td></tr><tr><td rowspan="1">3,4</td><td rowspan="3">$1 \le m \le n \le 2\times 10^3$</td><td rowspan="1">$0 \le k \le 50;1 \le h_i \le 100$</td></tr><tr><td rowspan="1">5,6,7,8</td><td rowspan="1">$0 \le k \le 100;1 \le h_i \le 5\times 10^3$</td></tr><tr><td rowspan="1">9,10,11,12</td><td rowspan="1">$0 \le k \le 5\times 10^3;1 \le h_i \le 5\times 10^3$</td></tr><tr><td rowspan="1">13,14</td><td rowspan="1">$1 \le m \le n \le 2\times 10^3$</td><td rowspan="1">$0 \le k \le 10^5;1 \le h_i \le 10^5$</td></tr><tr><td rowspan="1">15,16</td><td rowspan="1">$1 \le m \le n \le 10^5$</td><td rowspan="1">$0 \le k \le 100;1 \le h_i \le 10^5$</td></tr><tr><td rowspan="1">17,18,19,20</td><td rowspan="1">$1 \le m \le n \le 10^5$</td><td rowspan="1">$0 \le k \le 10^5;1 \le h_i \le 10^5$</td></tr></tbody></table> 