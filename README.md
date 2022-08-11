# zen-algorithm
当头棒喝，以求顿悟

## [354](https://leetcode.cn/problems/russian-doll-envelopes/) 俄罗斯套娃信封问题

二维平面的最长子序列问题

> 宽度升序，保证一维包含
> 
> 高度降序，保证二维不包含重复宽度（同样宽度下，高度前面的高度只可能比它大，所以不会重复）

参考：https://labuladong.github.io/article/fname.html?fname=动态规划设计：最长递增子序列

## [34](https://leetcode.cn/problems/find-first-and-last-position-of-element-in-sorted-array/) 在排序数组中查找元素的第一个和最后一个位置

区间的裁剪

参考：https://labuladong.github.io/article/fname.html?fname=二分查找详解

## [77](https://leetcode.cn/problems/combinations/) 组合

k个元素的组合是子集树的k层节点

> len(val)决定层数，而不是num(idx+1)，那只是选择

参考：https://labuladong.github.io/article/fname.html?fname=子集排列组合

## [90](https://leetcode.cn/problems/subsets-ii/) 子集 II

值相同的相邻树枝会产生重复

> 排序，num[i-1] != num[i]

参考：https://labuladong.github.io/article/fname.html?fname=子集排列组合

## [47](https://leetcode.cn/problems/permutations-ii/) 排列 II

左相邻元素没有用过就跳过

> 相同元素相对位置固定，2 -> 2' -> 2''

参考：https://labuladong.github.io/article/fname.html?fname=子集排列组合

## [21](https://leetcode.cn/problems/merge-two-sorted-lists/) 合并两个有序链表

把较小的节点接到结果链表上

参考：https://labuladong.github.io/article/fname.html?fname=链表技巧

## [19](https://leetcode.cn/problems/remove-nth-node-from-end-of-list/) 删除链表的倒数第N个节点

双指针构成一条定长绳

参考：https://labuladong.github.io/article/fname.html?fname=链表技巧

## [876](https://leetcode.cn/problems/middle-of-the-linked-list/) 中间值

一步两步

参考：https://labuladong.github.io/article/fname.html?fname=链表技巧

## [160](https://leetcode.cn/problems/intersection-of-two-linked-lists/) 两个链表的第一个公共节点

a+b=b+a

## [76](https://leetcode.cn/problems/minimum-ascent-path/) 最小路径和

right可行解，left局部最优解

参考：https://labuladong.github.io/article/fname.html?fname=滑动窗口技巧进阶

## [567](https://leetcode.cn/problems/permutation-in-string/) 字符串的排列

True: 长度和valid

参考：https://labuladong.github.io/article/fname.html?fname=滑动窗口技巧进阶

## [3](https://leetcode.cn/problems/longest-substring-without-repeating-characters/) 最长无重复字符的子串

不需要need的滑动窗口

参考：https://labuladong.github.io/article/fname.html?fname=滑动窗口技巧进阶

## [206](https://leetcode.cn/problems/reverse-linked-list/) 链表反转

last = self.reverseList(head.next)

参考：https://labuladong.github.io/article/fname.html?fname=递归反转链表的一部分

## [92](https://leetcode.cn/problems/reverse-linked-list-ii/) 链表反转 II

successor相当与链表全反最后的null，调到开始处，反转前k个

参考：https://labuladong.github.io/article/fname.html?fname=递归反转链表的一部分

## [25](https://leetcode.cn/problems/reverse-nodes-in-k-group/) 反转链表中的每个组

不停地反转前k个

参考：https://labuladong.github.io/article/fname.html?fname=k个一组反转链表

## [1109](https://leetcode.cn/problems/corporate-flight-bookings/) 公司飞机票

[a,b] -> [a,b-a] -> [a,(b-a)+a]

[a,b] -> [a+3,b-a] -> [a+3,(b-a)+(a+3)]

> 从而完成加一个元素就提供了加一串数组的方法

参考：https://labuladong.github.io/article/fname.html?fname=差分技巧

## [1094](https://leetcode.cn/problems/car-pooling/) 公司可用车辆

同拆分数组，但先下后上

参考：https://labuladong.github.io/article/fname.html?fname=差分技巧

## [48](https://leetcode.cn/problems/rotate-image/) 旋转图像

先后沿斜和竖对称翻转

参考：https://labuladong.github.io/article/fname.html?fname=花式遍历

## [54](https://leetcode.cn/problems/spiral-matrix/) 螺旋矩阵

四指针

> 每次遍历前的if也太不优雅了，但一时间内没有想到更好的解法

参考：https://labuladong.github.io/article/fname.html?fname=花式遍历

## [99](https://leetcode.cn/problems/recover-binary-search-tree/) 恢复二叉搜索树

中序遍历得到仅一对错误的有序数组，通过双指针恢复

参考：插件内labuladong思路

## [124](https://leetcode.cn/problems/binary-tree-maximum-path-sum/) 二叉树的最大路径和

和二叉树宽度类似，但需要将小于0的路径置为0

参考：插件内labuladong思路

## [226](https://leetcode.cn/problems/invert-binary-tree/) 翻转二叉树

left,right=right,left

参考：二叉树递归基本操作
