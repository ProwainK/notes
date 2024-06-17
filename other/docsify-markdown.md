# Docsify Markdown 語法

這邊可以參考 Docsify 所使用的 Markdown 語法。


## 主標題

>標題
>===

標題的語法，個人比較偏好使用 # H1

```
標題
===
```


## 副標

>副標
>---

副標的語法，個人比較偏好使用 ## H2

```
副標
---
```


## 字體大小

># H1
>## H2
>### H3
>#### H4
>##### H5

```
# H1
## H2
### H3
#### H4
##### H5
```


## 字體效果

>*斜體字*
>**粗體字**
>***斜粗體***
>~~刪除線~~
>_斜體2_
>__斜粗2__ 不支援
>正常<sup>上標</sup>
>正常<sub>下標</sub>
><ins>ins 底線</ins>
><u>u 底線</u>
><mark>螢光標記</mark>

```
*斜體字*
**粗體字**
***斜體兼粗體***
~~刪除線~~
_斜體2_
__斜粗2__
正常<sup>上標</sup>
正常<sub>下標</sub>
<ins>ins 底線</ins>
<u>u 底線</u>
<mark>螢光標記</mark>
```

* `<u>` 為文字樣式 (style) 的標籤 (tag)，`<ins>` 則是結構上標記插入哪些文字

## 引文

縮排語法

> 第一層
>> 第二層
>>> 第三層

```
>第一層
>>第二層
>>>第三層
```


## 標號

1. 數字標號
2. 數字標號
3. 數字標號
- 其他標號
+ 其他標號
* 其他標號

```
1. 數字標號
2. 數字標號
3. 數字標號
- 其他標號
+ 其他標號
* 其他標號
```

---

## 同時縮排和換行

不支援。


## 巢狀標號

- 無序清單
- 無序清單
    - 無序清單子清單
        - 無序清單子子清單

1. 有序清單
2. 有序清單
    1. 有序清單子清單
    2. 有序清單子清單
        1. 有序清單子子清單
        2. 有序清單子清單

```MD
- 無序清單
- 無序清單
    - 無序清單子清單
        - 無序清單子子清單

1. 有序清單
2. 有序清單
    1. 有序清單子清單
    2. 有序清單子清單
        1. 有序清單子子清單
        2. 有序清單子清單
```

---

## 名詞定義、解釋

<dl>
  <dt><strong>Coffee</strong></dt>
  <dd>Black hot drink</dd>

  <dt><strong>Milk</strong></dt>
  <dd>White cold drink</dd>
</dl>

<dfn>The Discovery of India</dfn> was written by <abbr title= "The first Prime Minister of India">  Pt. Jawahar Lal Nehru. </abbr>

```
<dl>
  <dt><strong>Coffee</strong></dt>
  <dd>Black hot drink</dd>

  <dt><strong>Milk</strong></dt>
  <dd>White cold drink</dd>
</dl>

<dfn>The Discovery of India</dfn> was written by <abbr title= "The first Prime Minister of India">  Pt. Jawahar Lal Nehru. </abbr>
```

| Tag | 描述 |
| --- | ---- |
| dl   | 描述清單元素
| dt   | 定義術語元素
| dd   | 描述詳細資料元素
| dfn  | 定義元素
| abbr | 縮寫元素 (標記這裡有縮寫)


## 連結

>[連結名稱](https://google.com "游標顯示")

```
[連結名稱](https://google.com "游標顯示")
```


## 簡易超連結

網址直接貼上就好。

> https://google.com

> text@email.com


## 分隔線

1.

---

2.

***

3.

- - -

4.

* * *

```
1.

---

2.

***

3.

- - -

4.

* * *
```


## 程式碼

```cpp
#include <stdio.h>

int main(){

    printf("Hello World");

    return 0;
}
```

\```程式類型
程式碼
\```

```cpp showLineNumbers
#include <stdio.h>

int main(){

    printf("Hello World");

    return 0;
}
```

\```程式類型 showLineNumbers
行號 + 程式碼
\```

```cpp title="C++ 語法測試"
#include <stdio.h>
// TODO
```

\```程式類型 title="標題"
程式碼
\```


## 單純顯示圖片

![圖片](https://i1.wp.com/mrcodingroom.freesite.host/wp-content/uploads/2019/01/Drawing.png "哈")

```md
![圖片名稱](連結 "游標顯示")
```


## 圖片 + 連結

[![圖片](https://i1.wp.com/mrcodingroom.freesite.host/wp-content/uploads/2019/01/Drawing.png)](https://mrcodingroom.freesite.host/)

```md
[![圖片](圖片網址)](連結網址)
```

## YouTube 圖片 + 連結

```
Docsify 寫法
[![](http://img.youtube.com/vi/u5_hDQ7H98w/maxresdefault.jpg ":size=360")](https://youtu.be/u5_hDQ7H98w)
```

```
[![](http://img.youtube.com/vi/u5_hDQ7H98w/maxresdefault.jpg" :size=360")](https://youtu.be/u5_hDQ7H98w)
```

共通寫法
[<img src="http://img.youtube.com/vi/u5_hDQ7H98w/maxresdefault.jpg" width="360" />](https://youtu.be/u5_hDQ7H98w)

```
[<img src="http://img.youtube.com/vi/u5_hDQ7H98w/maxresdefault.jpg" width="360" />](https://youtu.be/u5_hDQ7H98w)
```


## 表格

| 欄位1 | 欄位2 | 欄位3 |
|:----- |:-----:| -----:|
| 置左  | 置中  | 置右  |
| $100  | $100  | $100  |
| $10   | $10   | $10   |
| $1    | $1    | $1    |

```
| 欄位1 | 欄位2 | 欄位3 |
|:----- |:-----:| -----:|
| 置左  | 置中  | 置右  |
| $100  | $100  | $100  |
| $10   | $10   | $10   |
| $1    | $1    | $1    |
```


## 短區塊

> `內容`

\`內容`


## CheckBox

> - [ ] uncheck
> - [x] check

```md
 - [ ] uncheck
 - [x] check
```


## 跳脫字元

\##
\```

```md
\+任意符號
```

---
## 區塊標籤標註

> [name=MingRay] [time=now] [color=#B40431]
>> [name=MingRay] [time=now] [color=#333333]
```md
>[name=MingRay] [time=now] [color=#B40431]
>>[name=MingRay] [time=now] [color=#333333]
```
---

## Emojis

😏 :smirk:
🉑 :accept:
👍 :+1:

```
😏 :smirk:
🉑 :accept:
👍 :+1:
```

https://emojidb.org/remark-emojis
https://www.npmjs.com/package/remark-emoji


## 標籤

###### tags: `標籤 1` `標籤 2`

```
###### tags: `標籤 1` `標籤 2`
```

---

## 註腳

註腳1[^1].
註腳2[^2].
行內註腳[^行內註腳]定義
重複的註腳2[^2].

[^1]:註腳1  定義
[^2]:註腳2: 定義
重複的註腳2: 定義
[^行內註腳]: 行內註腳: 定義

```md
註腳1[^1].
註腳2[^2].
行內註腳[^行內註腳]定義
重複的註腳2[^2].

[^1]:註腳1  定義
[^2]:註腳2: 定義
    重複的註腳2: 定義
        
[^行內註腳]: 行內註腳: 定義

```

---

## 外部媒體

### Youtube

```
{%youtube PykOBwo_iTI %}
```

```
{%youtube v=?後的id %}
```

### Vimeo

```
{%vimeo 124148255 %}
```

```
{%vimeo 網址最後的數字id %}
```

### Gist

```
{%gist MingRay98/0b4d70945b5259a209b72e486bc2a1e3%}
```

```
{%gist github後的連結/"%}
```

### PDF

**注意：請使用 https 的網址，否則可能會被您的瀏覽器阻擋載入**

```
{%pdf https://papers.nips.cc/paper/5346-sequence-to-sequence-learning-with-neural-networks.pdf %}
```

```
{%pdf pdf的連結 %}
```


## LaTeX 數學式

Mathematical equations can be rendered using KaTeX.
https://docusaurus.io/zh-CN/docs/markdown-features/math-equations


## > 提示色塊 Admonitions

> [!NOTE]
> An alert of type 'note' using global style 'callout'.

> [!TIP]
> An alert of type 'tip' using global style 'callout'.

> [!IMPORTANT]
> An alert of type 'important' using global style 'callout'.

> [!WARNING]
> An alert of type 'warning' using global style 'callout'.

> [!ATTENTION]
> An alert of type 'attention' using global style 'callout'.

```
> [!NOTE]
> An alert of type 'note' using global style 'callout'.

> [!TIP]
> An alert of type 'tip' using global style 'callout'.

> [!IMPORTANT]
> An alert of type 'important' using global style 'callout'.

> [!WARNING]
> An alert of type 'warning' using global style 'callout'.

> [!ATTENTION]
> An alert of type 'attention' using global style 'callout'.
```

https://github.com/fzankl/docsify-plugin-flexible-alerts

!> Deprecated as of v4.13. Docsify no longer requires this plugin for full emoji support.

?> Deprecated as of v4.13. Docsify no longer requires this plugin for full emoji support.

```
!> Deprecated as of v4.13. Docsify no longer requires this plugin for full emoji support.

?> Deprecated as of v4.13. Docsify no longer requires this plugin for full emoji support.
```


## ::: 提示色塊

:::note
Some **content** with _Markdown_ `syntax`. Check [this `api`](#).
optional: **note**
:::

:::info
Some **content** with _Markdown_ `syntax`. Check [this `api`](#).
optional: **info / important**
:::

:::tip
Some **content** with _Markdown_ `syntax`. Check [this `api`](#).
optional: **tip / success**
:::

:::warning
Some **content** with _Markdown_ `syntax`. Check [this `api`](#).
optional: **warning / caution**
:::

:::danger
Some **content** with _Markdown_ `syntax`. Check [this `api`](#).
optional: **danger**
:::

```
:::色塊選項
色塊內容
:::
```

* note / info / success / warning / danger 分別會對應不同顏色
* 冒號後面 **記得不要加空格**

## 收折文字內容

<details>
This is the detailed content.
</details>

```
<details>
This is the detailed content.
</details>
```

<details>
  <summary>收折標籤名稱</summary>

This is the detailed content 1.
This is the detailed content 2.
This is the detailed content 3.

</details>

```
<details>
  <summary>收折標籤名稱</summary>

This is the detailed content 1.
This is the detailed content 2.
This is the detailed content 3.

</details>
```

* 使用 summary 需要注意換行，和隱藏內容隔開

<details>
  <summary></summary>

This is the detailed content 1.

</details>

```
<details>
  <summary></summary>

This is the detailed content 1.

</details>
```

* 空白標籤名稱


## 【Remark 插件】remark-breaks

強制換行 (Hard breaks)，推薦使用。

1. `npm i remark-breaks` 安裝插件到專案
2. 修改 docusaurus.config.js
```ts
// 新增下面這個到檔案開頭區域
import remarkBreaks from 'remark-breaks'

  presets: [
    [
      'classic',
      {
        docs: {
          // 新增下面這個到 presets classic docs 這裡
          remarkPlugins: [remarkBreaks],
        },
      },
    ],
  ],
```
3. 重開專案 Server

https://www.npmjs.com/package/remark-breaks


---

# 參考資料

Markdown Features | Docusaurus
https://docusaurus.io/docs/markdown-features

docusaurus/website/_dogfooding/_pages tests/markdown-tests-mdx.mdx at main · facebook/docusaurus
https://github.com/facebook/docusaurus/blob/main/website/_dogfooding/_pages%20tests/markdown-tests-mdx.mdx


---
