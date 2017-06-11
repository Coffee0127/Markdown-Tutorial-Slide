# Markdown

#### Bo-Xuan Fan

---

Markdown 是什麼？ <img style="vertical-align: middle" src="images/Markdown-mark.png" alt="Markdown" title="Markdown mark">
* 輕量級標記語言 (Markup Language)
* 使用易讀易寫的純文字格式編寫文件，然後轉換成 HTML 語法

---

為什麼要用 Markdown？
1. 使用普通文字編輯器即可撰寫
2. 語法簡單
3. 不用學 HTML 即可寫出標記語言格式
4. 易讀性高
5. ~~拿來寫會議紀錄~~

Notes:
易讀性，沒有轉化成 HTML 結構前即容易理解

---

所以 Markdown 跟 HTML 到底什麼關係？
* HTML 是一種**發佈**的格式
* Markdown 是一種**編寫**的格式
    + Markdown 的目標是實現「易讀易寫」

---

哪邊可以用呢？
* [GitHub](https://github.com/)
* [GitBook](https://www.gitbook.com/)
* [GitLab](https://gitlab.com)
* [HackMD](https://hackmd.io/)
* ~~[hackpad](https://hackpad.com/)~~ (已被 Dropbox 併購)
* [Dropbox Paper](https://www.dropbox.com/paper)
* [Hexo](https://hexo.io/)
* ...

Notes:
Hackpad 已被 Dropbox Paper 收購

---

我該怎麼命名檔案呢？
* *.md
* *.markdown

任君挑選 (=´∀｀)人(´∀｀=)

---

Markdown Syntax

---

標題與段落

----

#### 標題 (#)
內容前面加上 1 ~ 6 個 `#`

```md
# H1 字體最大的標題
## H2 字體二大的標題
...
###### H6 字體第六大的標題
```

# H1 字體最大的標題
## H2 字體第二大的標題
...
###### H6 字體第六大的標題

----
`#` 可以使用 `=` 區隔  
`##` 可以使用 `-` 區隔

```md
H1 字體最大的標題
================
H2 字體二大的標題
----------------
```

H1 字體最大的標題
================
H2 字體二大的標題
----------------

----
#### 區塊引言
內容前面加上 `>`

```md
> 在非洲，每六十秒，就有一分鐘過去（參見非洲時間）
```

> 在非洲，每六十秒，就有一分鐘過去（參見非洲時間）

----
#### 段落
內容後面加上兩個空白  
(當然要加 `<br />` 也可以，只是很亂...)

---

清單

----
#### 無序清單
內容前面加上 `*` 或 `+` 或 `-` 即可

```md
下午茶
* 雞排
+ 珍珠奶茶
- 甜不辣
```

下午茶
* 雞排
+ 珍珠奶茶
- 甜不辣

----
#### 有序清單
內容前面加上 `1. ` 即可

```md
想看的電影
1. 神鬼奇航
1. 神力女超人
1. 神鬼傳奇
```

想看的電影
1. 神鬼奇航
2. 神力女超人
3. 神鬼傳奇

Notes:
在寫有序清單時，不需要排現在是第幾筆，全部都用 `1.` 會自動排序

---

連結

----
#### 超連結
```md
[連結名稱](URL)
[Google](https://www.google.com/)
```

[Google](https://www.google.com/)

----
#### 圖片
跟超連結一樣，只是前面加上 `!`
```md
![連結名稱](URL)
![Google](https://www.google.com.tw/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png)
```

![Google](https://www.google.com.tw/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png)

---

其他文字效果 (強調)

----
#### 粗體
使用 `**` 或 `__` 把文字包起來
```md
因為很**重要**，所以要粗體
```
因為很**重要**，所以要粗體

----
#### 斜體
使用 `*` 或 `_` 把文字包起來
```md
比薩_斜_塔
```
比薩_斜_塔

----
#### 粗體 + 斜體
~~摻在一起做撒尿牛丸~~
```md
**很重要的比薩_斜_塔**
```
**很重要的比薩_斜_塔**  

----
#### 刪除線
使用 `~~` 把文字包起來
```md
~~被刪除了QQ~~
```
~~被刪除了QQ~~

---

程式碼  

###### Markdown 的重要應用！！

----
#### 行內程式碼
使用 `‵` 把程式碼包起來
```md
變數名稱 ‵foo‵
```

變數名稱 `foo`

----
#### 程式碼區塊
使用 `‵‵‵` 把程式碼區塊包起來  
寫上程式語言名稱 (Optional)
```md
‵‵‵js
var foo = function() {
  console.log('Hello World');
};
‵‵‵
```

```js
var foo = function() {
  console.log('Hello World');
};
```

---

表格

_非 Markdown 標準_

----
#### 表格
使用 `|` 切割欄  
使用 `-` 切割標題列

```md
First Header | Second Header
------------ | -------------
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column
```

First Header | Second Header
------------ | -------------
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column

---

更多 Markdown 語法
* [Markdown 語法說明](http://markdown.tw/)
* [Github Markdown 語法](https://guides.github.com/pdfs/markdown-cheatsheet-online.pdf)
* [GitLab Markdown 語法](https://docs.gitlab.com/ee/user/markdown.html)
* [Emoji (不是都能使用)](https://www.webpagefx.com/tools/emoji-cheat-sheet/)

----
Ｑ：Markdown 沒有我要的語法怎麼辦？  

Ａ: 純手工打造 HTML (無誤)  
因為最後語法都會被轉成 HTML 檔案
<!-- .element: class="fragment" data-fragment-index="1" -->

---

哪些編輯器可以用呢？
* ~~記事本~~
* [Visual Studio Code](https://code.visualstudio.com/)
* [Atom](https://atom.io/)
* [Sublime](https://www.sublimetext.com/)
    + 需額外安裝 [View In Browser](https://packagecontrol.io/packages/View%20In%20Browser)
* [Github](https://github.com/)
* [HackMD](https://hackmd.io/)

Notes:
VSCode、Atom 內建即時預覽

---

#### 休(ㄕˊ)習(ㄗㄨㄛˋ)時間
[Markdown Tutorial](http://commonmark.org/help/tutorial/index.html)

---

Q & A
