<<<<<<< HEAD
<<<<<<< HEAD
## [剑指 Offer 62. 圆圈中最后剩下的数字](https://leetcode-cn.com/problems/yuan-quan-zhong-zui-hou-sheng-xia-de-shu-zi-lcof/)

0,1,···,n-1这n个数字排成一个圆圈，从数字0开始，每次从这个圆圈里删除第m个数字（删除后从下一个数字开始计数）。求出这个圆圈里剩下的最后一个数字。

例如，0、1、2、3、4这5个数字组成一个圆圈，从数字0开始每次删除第3个数字，则删除的前4个数字依次是2、0、4、1，因此最后剩下的数字是3。

**示例 1：**

```
输入: n = 5, m = 3
输出: 3
```

解法：

只有一个人，胜利者的下标就为0，需要逆推得到最初的位置

**关注胜利者的下标位置是怎么变的**

每次杀掉一个人，就会把胜利的位置往前移动m位

因为每次都会从杀掉的人后面一个开始重新报数（C 为被杀的，G 为最后胜利者）

![img](D:\前端\力扣leecode\offer.assets\1646543417-fDTqmX-image.png)

把 A 和 B 接到 H 后面形成一个新的队列，并且以 D 为新的队伍头

![img](D:\前端\力扣leecode\offer.assets\1646543431-VUFQRr-image.png)

![img](D:\前端\力扣leecode\offer.assets\1646543440-jEqIpM-image.png)

**一开始 G 在数组中下标是 6，删除元素后下标变为了3**

```js
var lastRemaining = function (n, m) {
    let pos = 0;//i=1，既只有一个人参赛
    for (let i = 2; i <= n; i++) {
        pos = (pos + m) % i;//等于少一个人比赛胜利的位置往右移m个再模当前的长度
    }
    return pos;
};
```

=======
## [剑指 Offer 62. 圆圈中最后剩下的数字](https://leetcode-cn.com/problems/yuan-quan-zhong-zui-hou-sheng-xia-de-shu-zi-lcof/)

0,1,···,n-1这n个数字排成一个圆圈，从数字0开始，每次从这个圆圈里删除第m个数字（删除后从下一个数字开始计数）。求出这个圆圈里剩下的最后一个数字。

例如，0、1、2、3、4这5个数字组成一个圆圈，从数字0开始每次删除第3个数字，则删除的前4个数字依次是2、0、4、1，因此最后剩下的数字是3。

**示例 1：**

```
输入: n = 5, m = 3
输出: 3
```

解法：

只有一个人，胜利者的下标就为0，需要逆推得到最初的位置

**关注胜利者的下标位置是怎么变的**

每次杀掉一个人，就会把胜利的位置往前移动m位

因为每次都会从杀掉的人后面一个开始重新报数（C 为被杀的，G 为最后胜利者）

![img](D:\前端\力扣leecode\offer.assets\1646543417-fDTqmX-image.png)

把 A 和 B 接到 H 后面形成一个新的队列，并且以 D 为新的队伍头

![img](D:\前端\力扣leecode\offer.assets\1646543431-VUFQRr-image.png)

![img](D:\前端\力扣leecode\offer.assets\1646543440-jEqIpM-image.png)

**一开始 G 在数组中下标是 6，删除元素后下标变为了3**

```js
var lastRemaining = function (n, m) {
    let pos = 0;//i=1，既只有一个人参赛
    for (let i = 2; i <= n; i++) {
        pos = (pos + m) % i;//等于少一个人比赛胜利的位置往右移m个再模当前的长度
    }
    return pos;
};
```

>>>>>>> 80016a86f0a17524ea5664f33d447f44cd769a36
=======
## [剑指 Offer 62. 圆圈中最后剩下的数字](https://leetcode-cn.com/problems/yuan-quan-zhong-zui-hou-sheng-xia-de-shu-zi-lcof/)

0,1,···,n-1这n个数字排成一个圆圈，从数字0开始，每次从这个圆圈里删除第m个数字（删除后从下一个数字开始计数）。求出这个圆圈里剩下的最后一个数字。

例如，0、1、2、3、4这5个数字组成一个圆圈，从数字0开始每次删除第3个数字，则删除的前4个数字依次是2、0、4、1，因此最后剩下的数字是3。

**示例 1：**

```
输入: n = 5, m = 3
输出: 3
```

解法：

只有一个人，胜利者的下标就为0，需要逆推得到最初的位置

**关注胜利者的下标位置是怎么变的**

每次杀掉一个人，就会把胜利的位置往前移动m位

因为每次都会从杀掉的人后面一个开始重新报数（C 为被杀的，G 为最后胜利者）

![img](D:\前端\力扣leecode\offer.assets\1646543417-fDTqmX-image.png)

把 A 和 B 接到 H 后面形成一个新的队列，并且以 D 为新的队伍头

![img](D:\前端\力扣leecode\offer.assets\1646543431-VUFQRr-image.png)

![img](D:\前端\力扣leecode\offer.assets\1646543440-jEqIpM-image.png)

**一开始 G 在数组中下标是 6，删除元素后下标变为了3**

```js
var lastRemaining = function (n, m) {
    let pos = 0;//i=1，既只有一个人参赛
    for (let i = 2; i <= n; i++) {
        pos = (pos + m) % i;//等于少一个人比赛胜利的位置往右移m个再模当前的长度
    }
    return pos;
};
```

>>>>>>> 80016a86f0a17524ea5664f33d447f44cd769a36
