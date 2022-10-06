# markdown格式速查

## 标题

要创建标题，请在单词或短语前面添加井号 (`#`) 。`#` 的数量代表了标题的级别。例如，添加三个 `#` 表示创建一个三级标题 (`<h3>`) (例如：`### My Header`)。

| Markdown语法               | HTML                       | 预览效果                               |
| ------------------------ | -------------------------- | ---------------------------------- |
| `# Heading level 1`      | `<h1>Heading level 1</h1>` | Heading level 1<br>=============== |
| `## Heading level 2`     | `<h2>Heading level 2</h2>` | Heading level 2<br>--------------- |
| `### Heading level 3`    | `<h3>Heading level 3</h3>` | ### Heading level 3                |
| `#### Heading level 4`   | `<h4>Heading level 4</h4>` | #### Heading level 4               |
| `##### Heading level 5`  | `<h5>Heading level 5</h5>` | ##### Heading level 5              |
| `###### Heading level 6` | `<h6>Heading level 6</h6>` | ###### Heading level 6             |

## 段落

要创建段落，请使用空白行将一行或多行文本进行分隔。

## 换行

要创建段落，请使用空白行将一行或多行文本进行分隔。

## 强调

要加粗文本，请在单词或短语的前后各添加两个星号（asterisks）或下划线（underscores）。如需加粗一个单词或短语的中间部分用以表示强调的话，请在要加粗部分的两侧各添加两个星号（asterisks）。

| Markdown语法                   | HTML                                      | 预览效果                       |
| ---------------------------- | ----------------------------------------- | -------------------------- |
| `I just love **bold text**.` | `I just love <strong>bold text</strong>.` | I just love **bold text**. |
| `I just love __bold text__.` | `I just love <strong>bold text</strong>.` | I just love **bold text**. |
| `Love**is**bold`             | `Love<strong>is</strong>bold`             | Love**is**bold             |

## 引用

要创建块引用，请在段落前添加一个 `>` 符号。

    > Dorothy followed her through many of the beautiful rooms in her castle.

渲染效果如下所示：

> Dorothy followed her through many of the beautiful rooms in her castle.

### 多个段落的块引用

块引用可以包含多个段落。为段落之间的空白行添加一个 `>` 符号。

    > Dorothy followed her through many of the beautiful rooms in her castle.
    >
    > The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.

渲染效果如下：

> Dorothy followed her through many of the beautiful rooms in her castle.
> 
> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.

### 嵌套块引用

块引用可以嵌套。在要嵌套的段落前添加一个 `>>` 符号。

    > Dorothy followed her through many of the beautiful rooms in her castle.
    >
    >> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.

渲染效果如下：

> Dorothy followed her through many of the beautiful rooms in her castle.
> 
> > The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.

### 带有其它元素的块引用

块引用可以包含其他 Markdown 格式的元素。并非所有元素都可以使用，你需要进行实验以查看哪些元素有效。

    > #### The quarterly results look great!
    >
    > - Revenue was off the chart.
    > - Profits were higher than ever.
    >
    >  *Everything* is going according to **plan**.

渲染效果如下：

> #### The quarterly results look great!
> 
> * Revenue was off the chart.
> * Profits were higher than ever.
> 
> _Everything_ is going according to **plan**.

## 列表

### 有序列表

要创建有序列表，请在每个列表项前添加数字并紧跟一个英文句点。数字不必按数学顺序排列，但是列表应当以数字 1 起始。

| Markdown语法                                                                                                           | HTML                                                                                                                                                                                   | 预览效果                                                                                                           |
| -------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- |
| `1. First item<br>2. Second item<br>3. Third item<br>4. Fourth item`                                                 | `<ol><br><li>First item</li><br><li>Second item</li><br><li>Third item</li><br><li>Fourth item</li><br></ol>`                                                                          | 1. First item<br>2. Second item<br>3. Third item<br>4. Fourth item                                             |
| `1. First item<br>1. Second item<br>1. Third item<br>1. Fourth item`                                                 | `<ol><br><li>First item</li><br><li>Second item</li><br><li>Third item</li><br><li>Fourth item</li><br></ol>`                                                                          | 1. First item<br>2. Second item<br>3. Third item<br>4. Fourth item                                             |
| `1. First item<br>8. Second item<br>3. Third item<br>5. Fourth item`                                                 | `<ol><br><li>First item</li><br><li>Second item</li><br><li>Third item</li><br><li>Fourth item</li><br></ol>`                                                                          | 1. First item<br>2. Second item<br>3. Third item<br>4. Fourth item                                             |
| `1. First item<br>2. Second item<br>3. Third item<br>    1. Indented item<br>    2. Indented item<br>4. Fourth item` | `<ol><br><li>First item</li><br><li>Second item</li><br><li>Third item<br><ol><br><li>Indented item</li><br><li>Indented item</li><br></ol><br></li><br><li>Fourth item</li><br></ol>` | 1. First item<br>2. Second item<br>3. Third item<br>  1. Indented item<br>  2. Indented item<br>4. Fourth item |

### 无序列表

---------------------------------------------------------------------------------------------

要创建无序列表，请在每个列表项前面添加破折号 (-)、星号 (*) 或加号 (+) 。缩进一个或多个列表项可创建嵌套列表。

| Markdown语法                                                                                                     | HTML                                                                                                                                                                                   | 预览效果                                                                                                     |
| -------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- |
| `- First item<br>- Second item<br>- Third item<br>- Fourth item`                                               | `<ul><br><li>First item</li><br><li>Second item</li><br><li>Third item</li><br><li>Fourth item</li><br></ul>`                                                                          | * First item<br>* Second item<br>* Third item<br>* Fourth item                                           |
| `* First item<br>* Second item<br>* Third item<br>* Fourth item`                                               | `<ul><br><li>First item</li><br><li>Second item</li><br><li>Third item</li><br><li>Fourth item</li><br></ul>`                                                                          | * First item<br>* Second item<br>* Third item<br>* Fourth item                                           |
| `+ First item<br>+ Second item<br>+ Third item<br>+ Fourth item`                                               | `<ul><br><li>First item</li><br><li>Second item</li><br><li>Third item</li><br><li>Fourth item</li><br></ul>`                                                                          | * First item<br>* Second item<br>* Third item<br>* Fourth item                                           |
| `- First item<br>- Second item<br>- Third item<br>    - Indented item<br>    - Indented item<br>- Fourth item` | `<ul><br><li>First item</li><br><li>Second item</li><br><li>Third item<br><ul><br><li>Indented item</li><br><li>Indented item</li><br></ul><br></li><br><li>Fourth item</li><br></ul>` | * First item<br>* Second item<br>* Third item<br>  * Indented item<br>  * Indented item<br>* Fourth item |

### 在列表中嵌套其他元素

要在保留列表连续性的同时在列表中添加另一种元素，请将该元素缩进四个空格或一个制表符，如下例所示：

#### 段落

    *   This is the first list item.
    *   Here's the second list item.
    
        I need to add another paragraph below the second list item.
    
    *   And here's the third list item.

渲染效果如下：

* This is the first list item.

* Here's the second list item.
  
  I need to add another paragraph below the second list item.

* And here's the third list item.

#### 引用块

    *   This is the first list item.
    *   Here's the second list item.
    
        > A blockquote would look great below the second list item.
    
    *   And here's the third list item.

渲染效果如下：

* This is the first list item.

* Here's the second list item.
  
  > A blockquote would look great below the second list item.

* And here's the third list item.

#### 代码块

通常采用四个空格或一个制表符缩进。当它们被放在列表中时，请将它们缩进八个空格或两个制表符。

    1.  Open the file.
    2.  Find the following code block on line 21:
    
            <html>
              <head>
                <title>Test</title>
              </head>
    
    3.  Update the title to match the name of your website.

渲染效果如下：

1. Open the file.

2. Find the following code block on line 21:
   
   <html>
        <head>
          <title>Test</title>
        </head>

3. Update the title to match the name of your website.

#### 图片

    1.  Open the file containing the Linux mascot.
    2.  Marvel at its beauty.
    
        ![Tux, the Linux mascot](/assets/images/tux.png)
    
    3.  Close the file.

渲染效果如下：

1. Open the file containing the Linux mascot.

2. Marvel at its beauty.
   
   ![Tux, the Linux mascot](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAGQAAAB5CAMAAAD4dHQjAAAArlBMVEX////Hx8ePj49XV1c7OzsfHx9JSUlzc3Orq6vx8fHj4+MtLS2BgYG5ubnV1dVlZWWdnZ3///9xXymZeBfClhWnghZwWxpzb2RVRxzdqhP4vhE6Mx2Mbxi0jBUtKR7qtBJxYzhXU0hJRTpIPRzPoBRjURt+ZRl+aShya1WBfXJyZ0b8/Pz5+fn9/f329vbu7u7p6enm5ubv7+/6+vro6Oj39/fz8/Ps7Oz09PTr6+uCz11jAAAAAXRSTlMAQObYZgAABuxJREFUeAG1mgd/ozwShy3gD4g+a/DZgsDeubwlcXq2fP8vdvEAgRCDUthne8EPoxkNI35ZfAhhmBZqbMeVi/nxHB+vcbyZFdLBGYJZHaGPs9gzrpmLIfNbQoxjz5VyH0Pmz4uJSaI5HALTmHNIYmiYYbtI6AhmKV8N1kyr9adTb0FL8mUJ9MSzFLA+KfNLbCcw0eerkqT+WNNHiy/oGc9Gh/iixGg+VjqtIyJG2vNKBJ2IwYTUIP2ZyoslZv9DbXrBQIvxdYlLNQ7Q/MFNOC1zSjyiMJFEIe/u2ubQM9aMEl4pp7lzIopamTmXJAGIXACSqJFwLoy+xPz6Zqw/VrxI4j8hEZyN0Pi2TNNs9R83aCXWjJKAq3e9UTVZ3uTEw1ySCLBOSSnUxbpQqlhfKFWUSDg3s7VhXpokU2pZVEpVxVIpVWXfDa83KRkzSPDfVA3ZFP/DrJJ1pc5QbWeTSGClzrDbqaqcKycCpcqqt47yQqn1fCW8Vau9GpCVmepJ/K/3rk213b+Kpdrn6emX2YZIB9irarXddYqiPLDzmz3XU8sCZ35ZFlVTuuVqw66/omSmU4rHef2+UZtVuS6KwzY/sEJlf3vkzTRE8s0aMjjlOc2Ki10dzuFv8eqpBecrEruZHdy/VEfxj0dMMMvAEgHNtBJ9awss/VdQQzTLUcjBCTrh/VOklUqX313qsGaYuj30pyAvMYwkopbBevnRl46kAY0Sff1IH4IJaRwb+FqFtXMoTZCgh/v5g1xME8gvnuvapLo0hYMevvzkqdeXNIX4yvucyEeNQ9NYwGeT3x1xBE2TfP4k7KDBIg3SxyeTH6IlIQ2c+sD9eFo8H13adXjcUzpL8JF2Yvj6tDMOW4IPdn3OpcV9ySM9og45RoMl391OhIP6TKqHAze7CjDe205iT1u/gw3phh+YkOpLvLgLRIszWDDzfY91R4y0rcur4/kCAwzv3bl360DMtxvxeH1ze3fi9v76eDYU572hWBxI9CaQh/u7Ho/3l29DSXShDALh2u9H0So65HFYYHbX+GN9ICb59QG35enx7i23D/RCWN/b+wrM7VWjpJYfd+e5HnT8hPR7pS0tn8N2qIWXSmMxwJd02143MTp8X2HfobV49TInaIk0jxFX9tMu7xidxeZrBPTr5ddJE73Vur6b5qG/XiT1w3EIhkS3SS4fNZLbIzFRHT1emJ6CTJZ4xPy803FDNT73OmiTYnUSi5hfd3quiIkBpy8Jx14MdJK43uiPd3puX5LikoQu86KVSMDQV9agwqQwJAmtxGglZCPkrOsFXShMZOkkAWqIEghdIINQ+Ih0usi1piUmagRJX+oyMgjFxQnf8Tg5WgkXidHfh3oeukntWRP5Wkk30f1+r+PxIUGHwRaNhEPp0q7n5igd9HB48YRGArfbiHruKfTxCleOP7Zi5EVR7Hnq1HWUjt/kgi/qMGn0gRJgValndts6lnfW1lWETBXo43hjx6EQ+/4rzFgeb97j+EnmXqkdhljh2eNCXqm+xQ95ftDxFGGnlMrRsUzTtMjPnSFs/r9Me2OxvNRX8dHI1TMZWsqseYeIYSwyxlL1WNUhR3SvX61DewWzbu+1yl/n3gt8HFSfDWpcnUUSMsUc8Mw+VS8U/eeWawPbVL2mQE2isfzw0F5apengRo1WEVnIDzs1oHt9bUxbrgQqNUJutg6fE/WWZbf7f09JXKgxVmhbSbkbuw80RFMTy6VRqjGWEHUgKNQIGRqskVmYIWOtxtg0W8VAqsZYo8E9fk6itr6sJWqUFA023YxLzAlJiriW7NRE4hrG1+uRO9coB+6TLlI1SpVrJLzhCzUB9xaBCzXODkxMvzUbfuI+fbmQdXVNVpgjr8Z7sMBGTZGetj32aooVQj4xanrwBFtrsbDWmv9j09NkD16paQroJVUZTBTwk8SFXuLhoKZJEY5Nkj8fKIDSkFuLBDulofDl5c05xRVF9nRK+fmYLMxSacktQVdDzf0V8WuLpZoiyxFoi4tJgTiiy1837ar9vn86UuTgxG5KsYZ/es6jUHrWAEzXI6KrZy6JKDIsMOVkFL4hF++VZGDs2DCESIzA9NEyWpsXtYLBSumpMMrIPW7WjYIxy0rp+ahkCQSyfxbNL2aXrGBHwy9tLfdFlu70zVgvaR2OHM6OblznsVyvlunE4GLFRij4ak+4RmxyfR3OOhZD2qsCvqpcDT08bxpJ/fFD7FzvGCKSGNhevLlMjL/oW77Nx0KLNHzky6pXjXsEi1HscjdoVTGHrNdYwLpINyfDxWr6dWLk9y1Z2d2QltDx0RJzNU5ZijruKsthicVHiFzjRKgN3jOB9f6w3gJWt8lnRzg2ANMJF+f5P0W+bcQV1sTgAAAAAElFTkSuQmCC)

3. Close the file.

#### 列表

    1. First item
    2. Second item
    3. Third item
        - Indented item
        - Indented item
    4. Fourth item

渲染效果如下：

1. First item
2. Second item
3. Third item
   * Indented item
   * Indented item
4. Fourth item

## 代码

要将单词或短语表示为代码，请将其包裹在反引号 (`` ` ``) 中。

| Markdown语法                              | HTML                                             | 预览效果                                |
| --------------------------------------- | ------------------------------------------------ | ----------------------------------- |
| ``At the command prompt, type `nano`.`` | `At the command prompt, type <code>nano</code>.` | At the command prompt, type `nano`. |

### 转义反引号

如果你要表示为代码的单词或短语中包含一个或多个反引号，则可以通过将单词或短语包裹在双反引号(` `` `)中。

| Markdown语法                                    | HTML                                               | 预览效果                                  |
| --------------------------------------------- | -------------------------------------------------- | ------------------------------------- |
| ``` ``Use `code` in your Markdown file.`` ``` | ``<code>Use `code` in your Markdown file.</code>`` | ``Use `code` in your Markdown file.`` |

## 分隔线

要创建分隔线，请在单独一行上使用三个或多个星号 (`***`)、破折号 (`---`) 或下划线 (`___`) ，并且不能包含其他内容。

    ***
    
    ---
    
    _________________

以上三个分隔线的渲染效果看起来都一样：

## 链接

链接文本放在中括号内，链接地址放在后面的括号中，链接title可选。

超链接Markdown语法代码：`[超链接显示名](超链接地址 "超链接title")`

对应的HTML代码：`<a href="超链接地址" title="超链接title">超链接显示名</a>`

    这是一个链接 [Markdown语法](https://markdown.com.cn)。

渲染效果如下：

这是一个链接 [Markdown语法](https://markdown.com.cn/)。

### 给链接增加 Title

链接title是当鼠标悬停在链接上时会出现的文字，这个title是可选的，它放在圆括号中链接地址后面，跟链接地址之间以空格分隔。

    这是一个链接 [Markdown语法](https://markdown.com.cn "最好的markdown教程")。

渲染效果如下：

这是一个链接 [Markdown语法](https://markdown.com.cn/ "最好的markdown教程")。

### 网址和Email地址

使用尖括号可以很方便地把URL或者email地址变成可点击的链接。

    <https://markdown.com.cn>
    <fake@example.com>

渲染效果如下：

[https://markdown.com.cn](https://markdown.com.cn/)  
[fake@example.com](mailto:fake@example.com)

### 带格式化的链接

强调链接, 在链接语法前后增加星号。 要将链接表示为代码，请在方括号中添加反引号。

    I love supporting the **[EFF](https://eff.org)**.
    This is the *[Markdown Guide](https://www.markdownguide.org)*.
    See the section on [`code`](#code).

渲染效果如下：

I love supporting the **[EFF](https://eff.org/)**.  
This is the _[Markdown Guide](https://www.markdownguide.org/)_.  
See the section on [`code`](https://markdown.com.cn/basic-syntax/links.html#code).

### 引用类型链接

引用样式链接是一种特殊的链接，它使URL在Markdown中更易于显示和阅读。参考样式链接分为两部分：与文本保持内联的部分以及存储在文件中其他位置的部分，以使文本易于阅读。

#### 链接的第一部分格式

引用类型的链接的第一部分使用两组括号进行格式设置。第一组方括号包围应显示为链接的文本。第二组括号显示了一个标签，该标签用于指向您存储在文档其他位置的链接。

尽管不是必需的，可以在第一组和第二组括号之间包含一个空格。第二组括号中的标签不区分大小写，可以包含字母，数字，空格或标点符号。

以下示例格式对于链接的第一部分效果相同：

* `[hobbit-hole][1]`
* `[hobbit-hole] [1]`

#### 链接的第二部分格式

引用类型链接的第二部分使用以下属性设置格式：

1. 放在括号中的标签，其后紧跟一个冒号和至少一个空格（例如`[label]:`）。
2. 链接的URL，可以选择将其括在尖括号中。
3. 链接的可选标题，可以将其括在双引号，单引号或括号中。

以下示例格式对于链接的第二部分效果相同：

* `[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle`
* `[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit lifestyles"`
* `[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle 'Hobbit lifestyles'`
* `[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle (Hobbit lifestyles)`
* `[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> "Hobbit lifestyles"`
* `[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> 'Hobbit lifestyles'`
* `[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> (Hobbit lifestyles)`

可以将链接的第二部分放在Markdown文档中的任何位置。有些人将它们放在出现的段落之后，有些人则将它们放在文档的末尾（例如尾注或脚注）。

## 图片

要添加图像，请使用感叹号 (`!`), 然后在方括号增加替代文本，图片链接放在圆括号里，括号里的链接后可以增加一个可选的图片标题文本。

插入图片Markdown语法代码：`![图片alt](图片链接 "图片title")`。

对应的HTML代码：`<img src="图片链接" alt="图片alt" title="图片title">`

    ![这是图片](/assets/img/philly-magic-garden.jpg "Magic Gardens")

渲染效果如下：

![这是图片](https://markdown.com.cn/assets/img/philly-magic-garden.9c0b4415.jpg "Magic Gardens")

### 链接图片

给图片增加链接，请将图像的Markdown 括在方括号中，然后将链接添加在圆括号中。

    [![沙漠中的岩石图片](/assets/img/shiprock.jpg "Shiprock")](https://markdown.com.cn)

渲染效果如下：

[![沙漠中的岩石图片](https://markdown.com.cn/assets/img/shiprock.c3b9a023.jpg "Shiprock")](https://markdown.com.cn/)

## 转义字符

要显示原本用于格式化 Markdown 文档的字符，请在字符前面添加反斜杠字符 \ 。

    \* Without the backslash, this would be a bullet in an unordered list.

渲染效果如下：

* Without the backslash, this would be a bullet in an unordered list.

### [#](https://markdown.com.cn/basic-syntax/escaping-characters.html#%E5%8F%AF%E5%81%9A%E8%BD%AC%E4%B9%89%E7%9A%84%E5%AD%97%E7%AC%A6)可做转义的字符

以下列出的字符都可以通过使用反斜杠字符从而达到转义目的。

| Character | Name                                                                                                                               |
| --------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| \         | backslash                                                                                                                          |
| `         | backtick (see also [escaping backticks in code](https://markdown.com.cn/basic-syntax/escaping-characters.html#escaping-backticks)) |
| *         | asterisk                                                                                                                           |
| _         | underscore                                                                                                                         |
| { }       | curly braces                                                                                                                       |
| [ ]       | brackets                                                                                                                           |
| ( )       | parentheses                                                                                                                        |
| #         | pound sign                                                                                                                         |
| +         | plus sign                                                                                                                          |
| -         | minus sign (hyphen)                                                                                                                |
| .         | dot                                                                                                                                |
| !         | exclamation mark                                                                                                                   |
| \|        | pipe (see also [escaping pipe in tables](https://markdown.com.cn/extended-syntax/escaping-pipe-characters-in-tables.html))         |

## HTML标签

对于 Markdown 涵盖范围之外的标签，都可以直接在文件里面用 HTML 本身。如需使用 HTML，不需要额外标注这是 HTML 或是 Markdown，只需 HTML 标签添加到 Markdown 文本中即可。

行级內联标签
-----------------------------------------------------------------------------------------------------------------

HTML 的行级內联标签如 `<span>`、`<cite>`、`<del>` 不受限制，可以在 Markdown 的段落、列表或是标题里任意使用。依照个人习惯，甚至可以不用 Markdown 格式，而采用 HTML 标签来格式化。例如：如果比较喜欢 HTML 的 `<a>` 或 `<img>` 标签，可以直接使用这些标签，而不用 Markdown 提供的链接或是图片语法。当你需要更改元素的属性时（例如为文本指定颜色或更改图像的宽度），使用 HTML 标签更方便些。

HTML 行级內联标签和区块标签不同，在內联标签的范围内， Markdown 的语法是可以解析的。

    This **word** is bold. This <em>word</em> is italic.

渲染效果如下:

This **word** is bold. This _word_ is italic.

区块标签
---------------------------------------------------------------------------------------------

区块元素──比如 `<div>`、`<table>`、`<pre>`、`<p>` 等标签，必须在前后加上空行，以便于内容区分。而且这些元素的开始与结尾标签，不可以用 tab 或是空白来缩进。Markdown 会自动识别这区块元素，避免在区块标签前后加上没有必要的 `<p>` 标签。

例如，在 Markdown 文件里加上一段 HTML 表格：

    This is a regular paragraph.
    
    <table>
        <tr>
            <td>Foo</td>
        </tr>
    </table>
    
    This is another regular paragraph.

请注意，Markdown 语法在 HTML 区块标签中将不会被进行处理。例如，你无法在 HTML 区块内使用 Markdown 形式的`*强调*`。



## 注

转载自[Markdown 官方教程](https://markdown.com.cn/)


