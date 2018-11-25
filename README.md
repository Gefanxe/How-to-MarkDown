# mk語法-git寫法

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

### 標題 h1~h6

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



### 粗斜體

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


### 清單-ul>li、 ol<li

```
粗斜體混搭
_你**可以**試著混搭_
```

* Item 1
* Item 2
  * Item 2a
  * Item 2b
  
  
  
1. Item 1
1. Item 2
1. Item 3
   1. Item 3a
   1. Item 3b
   
   
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
