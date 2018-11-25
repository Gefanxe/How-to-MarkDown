# mk語法-git寫法

目錄
* 小技巧
* 標題-h1~h6
* 強調-粗斜體、劃線
* 清單-ul>li、 ol<li
* 引用圖片
* 引用網址連結
* 引述別人論點
* 小區塊-HightLight 提示 高亮
* 大區塊-程式碼
* checkbox 打勾勾
* table 欄位

## 小技巧

先把小技巧放上面，比較好查詢@@
* shift+enter 可以直接第一位置，
有時候enter會延續縮排的效果。

* 單一enter並非到下一行，而是沒有效果，跟程式語言一樣。

* 其實引用圖片，可以引用git的內容喔！使用相對路徑寫法


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
*這是範例1*
_這是範例2_

```
粗體
**前後各加 2 個米字號**
__前後各加 2 個底線__
```
**這是範例1**
__這是範例2__

```
劃線
~~前後各加 2 個波浪~~
```
~~這是範例~~

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
* 範例 1 前面加個米字號或是 槓 -
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

1. 項目 1
131400. 項目 2
99999. 項目 3
          1. 項目 3a
          1. 項目 3b
1. 項目 4


```
3. 項目1 //從3開始，結果如下
3. 項目2
```
3. 項目1
3. 項目2


## 引用圖片

公式：!+[]+()

替代文字：圖片連結未顯現時，所出現的畫面會改用文字
```
![替代文字](連結)
```
![範例](http://pluspng.com/img-png/free-tag-png-free-256.png)

![連結失敗範例](/images/logo.png)


## 引用網址連結

公式1： 直接上網址，前後空格
公式2：[]+()
```
1.
http://github.com

2.
[顯現文字](網址)
[範例](http://github.com)
```

文字文字 http://github.com 文字文字

[範例](http://github.com)


## 引述別人論點

_**清單 採用 前 標點符號**_

前面加1個 大於符號，加空格，其實很多地方可以看出來MarkDown寫起來很直覺，這個寫法又更加明顯。

要注意的是，如果引用兩人的論述，記得不要直接按下enter劃到下一行，要在空一行，也就是enter兩次

```
> 這裡可以寫敘述
       // 空行
> 然後下一行也需要再加 大於 標點符號
```
> 第一行 範例

> 第二行 範例


## 小區塊-HightLight 提示 高亮

公式：前後加 反引號 `

這邊就有個小問題了，對於打注音的使用者，通常打出反引號時，需要特別注意，按下反引號後，立即按下enter，不然接下來會出現"非正式"的英文。
```
`範例1`
`<範例2>`
```
`範例1`
`<範例2>`


## 大區塊-程式碼

公式1： 前後加 三個反引號```
公式2：4個空個，然後，直接上function

此為大區塊，適合寫下程式碼，沒人想用純文字寫下程式碼吧!?

```
(不需要空格)```程式語言 // 直接3個反引號+內容要呈現的語言 (可選)
內容內容內容
(不需要空格)``` // 最後再以3個反引號收尾
```
```
內容內容內容
``` 


```
輸出
    function fancyAlert(arg) {
      if(arg) {
        $.facebox({div:'#foo'})
      }
    }
 
```

結果

    function fancyAlert(arg) {
      if(arg) {
        $.facebox({div:'#foo'})
      }
    }
    

## checkbox 打勾勾

_**清單 採用 前 標點符號**_

要預設打勾，就直接在中括號裡面，寫個x，超直覺的吧

```
- [x] 這是項目1
- [ ] 這是項目2
```
- [x] 這是項目1
- [ ] 這是項目2


## table 欄位


這個也很直覺
只有首欄才用兩個槓做區隔 --，記得是2個喔，1個就變成清單寫法
```
頭1 | 頭2
--|--
身體 1 | 身體 2
身體 1.2 | 身體 2.2
```
頭1 | 頭2
--|--
身體 1 | 身體 2
身體 1.2 | 身體 2.2
