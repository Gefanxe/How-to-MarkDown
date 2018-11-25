# mk語法-git寫法

目錄
* 標題-h1~h6
* 強調-粗斜體
* 清單-ul>li、 ol<li
* 引用圖片
* 引用網址連結
* 引述別人論點
* 小區塊-HightLight 提示 高亮
* 大區塊-程式碼
* checkbox 打勾勾
* table 欄位

## 標題 h1~h6

_**標題 採用 前 標點符號**_

凡#標號後空格，才會顯現，且單行控制

#是H1，##是h2，###是h3，####是h4，#####是h5，######是h6
```
# H1
## h2
### h3
#### h4
##### h5
###### h6
```

# h1
## h2
### h3
#### h4
##### h5
###### h6



## 粗斜體
_**粗斜體 採用 前後 標點符號**_
```
斜體
*前後各加 1 個米字號*
_前後各加 1 個底線_
```
*這是範例*
_這是範例_

```
粗體
**前後各加 2 個米字號**
__前後各加 2 個底線__
```
**這是範例**
__這是範例__


```
粗斜體混搭
_你**可以**試著混搭_
```
_你**可以**試著混搭_


## 清單-ul>li、 ol<li

### ul>li (未標號)

_**清單 採用 前 標點符號**_

凡*標號後空格，才會顯現，且子清單縮排(2個空格)

注意! 在寫第三排的時候，字會變成紅色乃為 _正常_，

但是寫第四排時候，變成紅色為 _不正常_

依順序，實心圓、空心圓、實心方
```
* 範例 1 前面加個米字號
* 範例 2
  * 範例 2a
  * 範例 2b
       * 範例 3 (這裡的字會變成紅色)
         * 範例4 (此為黑色 正常)
* 範例 5
```

* 範例 1
* 範例 2
  * 範例 2a
  * 範例 2b
       * 範例 3
         * 範例4
* 範例 5

### ol>li (標號)

這邊寫法很特別

最重要的是第一個項目，假設要從1開始
則1.這邊要記得使用標點符號(點)，然後空格，

接著特別的地方來了，後面的項目數字隨便你寫，不管寫多少，他都會自動幫你排列

更特別的是，如果子項目要開始**必定**從1開始，

然後 還記得前面說數字隨便寫嗎？ 
這是有關連的，每寫一個數字，其子項目要空格數量+2。
事實上，可以隨便寫，但是牽扯到子項目的話，_似乎_最多填寫5個數字

**但是數字太大還是會有例外喔**，還是乖乖的照規矩來就好
```
1. 項目 1
131400. 項目 2
99999. 項目 3 //5個數字
          1. 項目 3a //10個空格
          1. 項目 3b
1. 項目 4 //數字一樣也可
```

1. 範例 1
131400. 範例 2
99999. 範例 3
          1. 範例 3a
          1. 範例 3b
1. 範例 4


```
3. 項目1 //從3開始，結果如下
3. 項目2
```
3. 範例1
3. 範例2

## 引用圖片

![GitHub Logo](/images/logo.png)
Format: ![Alt Text](url)


http://github.com - automatic!
[GitHub](http://github.com)


As Kanye West said:

> We're living the future so
> the present is our past.

I think you should use an
`<addr>` element here instead.


```javascript
function fancyAlert(arg) {
  if(arg) {
    $.facebox({div:'#foo'})
  }
}
```


    function fancyAlert(arg) {
      if(arg) {
        $.facebox({div:'#foo'})
      }
    }
    
    
    
def foo():
    if not bar:
        return True



- [x] @mentions, #refs, [links](), **formatting**, and <del>tags</del> supported
- [x] list syntax required (any unordered or ordered list supported)
- [x] this is a complete item
- [ ] this is an incomplete item



First Header | Second Header
------------ | -------------
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column
