---
layout: article
author: bing0ne
date: "2018-07-23T20:49:30+08:00"
slug: "leetcode-02"
title: "LeetCode 02. Add Two Numbers"
tags: ["GO","LeetCode","ALGO"]
description: "这是LeetCode题库中的第二题。两个列表分别代表两个数。将两个数进行相加，返回一个数，并使用列表的形式输出。"
categories: ["Dev"]
---

You are given two non-empty linked lists representing two non-negative integers. The digits are stored in reverse order and each of their nodes contain a single digit. Add the two numbers and return it as a linked list.

You may assume the two numbers do not contain any leading zero, except the number 0 itself.

Example
```
Input: (2 -> 4 -> 3) + (5 -> 6 -> 4)
Output: 7 -> 0 -> 8
Explanation: 342 + 465 = 807.
```

## Solution:
只需要遍历两个列表，并注意处理当两个数相加大于10的情况，以及当一个列表为空的情况。

**时间复杂度**: O(max(m,n))  
**空间复杂度**: O(max(m,n)) 

```go
/**
 * Definition for singly-linked list.
 * type ListNode struct {
 *     Val int
 *     Next *ListNode
 * }
 */
func addTwoNumbers(l1 *ListNode, l2 *ListNode) *ListNode {
    carry := 0
    head := new(ListNode)
    curr := head 
    for l1 != nil || l2 != nil  {
        n1, n2 := 0,0 
        if( l1 != nil){
            l1, n1 = l1.Next, l1.Val
        }
        if( l2 != nil) {
            l2, n2 = l2.Next, l2.Val
        }
        sum := n1 + n2 + carry
        carry = sum / 10
        curr.Next = &ListNode{Val:sum%10,Next:nil}
        curr = curr.Next
        if (carry > 0) {
            curr.Next = &ListNode{Val:1,Next:nil}
        }
    }
    return head.Next
}
```

