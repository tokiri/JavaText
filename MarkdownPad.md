# 标题
## 标题
### 标题

一级标题
=
二级标题
-

>引用
>
>引用

## 加粗
**粗体**
*斜体*

## 多层嵌套
>aaaaaa
>>bbbbbbb
>>>ccccc

## 插入链接
[百度](https://www.baidu.com/)

## 图片
![df][01]
[01]:https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1548688722885&di=6aeccfd333a86c51b574ae5310f03657&imgtype=0&src=http%3A%2F%2Fimg.mp.itc.cn%2Fupload%2F20170526%2Ffff3cde171b64d65a0f63338f0613ff0_th.jpg '描述'
![avatar](https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1548688722885&di=6aeccfd333a86c51b574ae5310f03657&imgtype=0&src=http%3A%2F%2Fimg.mp.itc.cn%2Fupload%2F20170526%2Ffff3cde171b64d65a0f63338f0613ff0_th.jpg)

## 序表
### 有序
1. one
2. two

### 无序
* one
* two
- three

## 代码
	第一段
	第二段

## 表格

| 字段一        |         字段二 | 字段三 |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

***
---
* * *
- - -

flow
st=>start: Start|past:>http://www.google.com[blank]
e=>end: End:>http://www.google.com
op1=>operation: get_hotel_ids|past
op2=>operation: get_proxy|current
sub1=>subroutine: get_proxy|current
op3=>operation: save_comment|current
op4=>operation: set_sentiment|current
op5=>operation: set_record|current

cond1=>condition: ids_remain空?
cond2=>condition: proxy_list空?
cond3=>condition: ids_got空?
cond4=>condition: 爬取成功??
cond5=>condition: ids_remain空?

io1=>inputoutput: ids-remain
io2=>inputoutput: proxy_list
io3=>inputoutput: ids-got

st->op1(right)->io1->cond1
cond1(yes)->sub1->io2->cond2
cond2(no)->op3
cond2(yes)->sub1
cond1(no)->op3->cond4
cond4(yes)->io3->cond3
cond4(no)->io1
cond3(no)->op4
cond3(yes, right)->cond5
cond5(yes)->op5
cond5(no)->cond3
op5->e
