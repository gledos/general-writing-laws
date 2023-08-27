# 通用写作律法

```yaml
标题: 通用写作律法
创建时间: 2023年8月26日
版本: 0.0.8-beta
```

<ruby>通用写作律法<rp>(</rp><rt>General Writing Laws</rt><rp>)</rp></ruby>是由
[Save The Web Project][] 设计的开放律法（标准），后文简称为《律法》。

[Save The Web Project]: https://github.com/saveweb

《律法》有多种设想的使用场景，分别是：

1.  阅读：寻找适合自己的写作规则。
2.  使用：完善自己的写作规则，不再模棱两可。
3.  共享：将精心选配的《律法》规则作为团队的写作规范。

《律法》出现的根本原因，是在不使用专业排版工具的情况时，以及无 CSS 自动优化的时候，
比如在 Twitter, Facebook 以及 Telegram 等地，纯粹的使用文本、符号和空格来让文字排版得美观易读。

并且每个人都有自己的习惯以及美学，要求他人使用某种固定的规范是不太现实的，
所以不如每个人遵守自己精心选配的《律法》，如果团队写作有需求使用相同的规范，
那么使用《律法》模块化的搭建一套规范，也能减少模棱两可的情况。

## 当前《律法》状态

其他书写系统的完整支持，以及《律法》翻译尚未完成。

Full support for other writing system, and _General Writing Laws_ translations are not yet complete.

目前暂未完成各项模块的情况，一定会有编号变动，甚至重构的情况。

## 简介

《律法》是为了将各种书写规范模块化，而诞生的规则，借鉴了一些 [BEP 0000][]（BitTorrent 增强建议索引）的设计。

[BEP 0000]: https://www.bittorrent.org/beps/bep_0.html

并且《律法》兼容多种书写系统，不仅仅是中文主体，而是要打造一套各种书写系统都通用的写作规则，
并且减少特例、例外的情况，让规范简单易懂。

因为《律法》是模块化的，所以可以选配各种不同的规范，然后生成仅包含这些规范的个性化《律法》。

## GWLM 0 通用写作律法模块

```yaml
标题: 通用写作律法模块
创建时间: 2023年8月26日
```

GWLM 0 是收录通用写作律法模块的清单，会收录所有的 GWLM（General Writing Laws Module，
通用写作律法模块）内容，并对可行性进行评议，每条 GWLM 都会被分类，分别是「正式」
「草案」「延期」和「拒绝」。[^bep0]

[^bep0]: 借用了许多 [BEP 0000][]（BitTorrent 增强建议索引）的设计。

### 正式的 GWLM

| 序号        | 标题                       |
| ----------- | -------------------------- |
| [0][gwlm-0] | [通用写作律法模块][gwlm-0] |
| [1][gwlm-1] | [词汇表][gwlm-1]           |
| [2][gwlm-2] | [书写系统空间][gwlm-2]     |
| [3][gwlm-3] | [书写系统规范][gwlm-3]     |
| [4][gwlm-4] | [兼容性][gwlm-4]           |
| [5][gwlm-5] | [表情][gwlm-5]             |

[gwlm-0]: #gwlm-0-通用写作律法模块
[gwlm-1]: #gwlm-1-词汇表
[gwlm-2]: #gwlm-2-书写系统空间
[gwlm-3]: #gwlm-3-书写系统规范
[gwlm-4]: #gwlm-4-兼容性
[gwlm-5]: #gwlm-5-表情

### 草案的 GWLM

| 序号                | 标题                               |
| ------------------- | ---------------------------------- |
| [15834][gwlm-15834] | [简体中文标点符号用法][gwlm-15834] |

[gwlm-15834]: #gwlm-15834-简体中文标点符号用法

### 延期的 GWLM

| 序号 | 标题   |
| ---- | ------ |
| x    | 占位符 |

### 拒绝的 GWLM

| 序号 | 标题   |
| ---- | ------ |
| x    | 占位符 |

## GWLM 1 词汇表

为了精确的描述以及理解，此章节用于定义／解释 GWLM 内的词汇。

+   GWLM 1-0：书写系统 (writing system)、字符 (character)

    指 Unicode 字符集中的所有字符，包含数字、文字（字母文字、象形文字）、标点符号和其他符号。

    使用方式：描述指向的是某一地区的字符，那么使用书写系统，比如「中文书写系统」「英文书写系统」，
    描述指向的的字符没有地区性质，那么使用字符，比如「全角字符」「半角字符」「所有的字符」「表意字符」

+   GWLM 1-1：数字

    这里是指狭义上的阿拉伯数字，包括半角 0123456789 以及全角０１２３４５６７８９。

+   GWLM 1-2：文字

    这里是指狭义上的文字，属于字符的子集，仅包含字母文字、象形文字等直接表意字符，即字典、
    词典收录的文字。

    使用方式：这里仅对书写系统进行规范，不会涉及狭义的语言，即口语，所以尽量减少「语言」一词，
    比如使用「英文」替代「英语」。

## GWLM 2 书写系统空间

```yaml
标题: 书写系统空间
创建时间: 2023年8月26日
```

「书写系统空间」是为文字的不同书写系统划分空间，并为各种部分指定「书写系统属地规范」。

### 划分空间

1.  标记「书名」「数字」以及「计量单位符号」等特殊的情况。

    ```text
             +======+==========+==========+==============+================+==+===+
        原文 | apple 是乔布斯传 steve jobs 中出现过的词语 电子版大小为不到 10 mb |
             +======+==========+==========+==============+================+==+===+
    特殊环境 |      ·          |   书名   |              ·                ·数·单位
             +------+----------+----------+--------------+----------------+--+---+
    ```

    备注：GitHub 的代码块并没有严格调用浏览器默认的等款字体，结果会造成排版错位，
    需要回到 GitHub 顶部，然后点击右上角的 Raw 按钮查看原始的等宽内容。

    关于特殊环境的详细处理方式，请参照 GWLM 3-5。

2.  标记外文的「片段环境」：

    ```text
             +======+==========+==========+==============+================+==+===+
        原文 | apple 是乔布斯传 steve jobs 中出现过的词语 电子版大小为不到 10 mb |
             +======+==========+==========+==============+================+==+===+
    特殊环境 |      ·          |   书名   |              ·                ·数·单位
             +------+----------+----------+--------------+----------------+--+---+
    片段环境 |  en  |          |    en    |              ·                ·  ·   |
             +------+----------+----------+--------------+----------------+--+---+
    ```

    这些外文片段的书写系统环境被称为「片段环境」。

3.  定义「书写系统环境」：

    通过标题和表意文字都是中文，能够给文章整体设下「简体中文」的「书写系统环境／环境变量」。

    ```text
             +======+==========+==========+==============+================+==+===+
        原文 | apple 是乔布斯传 steve jobs 中出现过的词语 电子版大小为不到 10 mb |
             +======+==========+==========+==============+================+==+===+
    特殊环境 |      ·          |   书名   |              ·                ·数·单位
             +------+----------+----------+--------------+----------------+--+---+
    片段环境 |  en  |          |    en    |              ·                ·  ·   |
             +------+----------+----------+--------------+----------------+--+---+
    书写系统环境    ·          ·          ·zh-Hans       ·                ·  ·   |
             +------+----------+----------+--------------+----------------+--+---+
    ```

### 文字属地规范

+   「片段环境」没有占满一句话时，不应该使用「片段环境」的属地语法，比如英语的句首大写。

+   在并列外语词语时，使用「书写系统环境」的属地语法的顿号，比如：

    > 我们的客户有 Yahoo、Facebook, Inc.、Microsoft Corporation 和 Google。

    > Our clients include “百度”, “腾讯”, “金山” and “奇虎360”.

    备注：是否使用引号包围外语，请参考《GWLM 3 兼容性》的〈[各种文字的兼容性](#各种文字的兼容性)〉
    章节。

## GWLM 3 书写系统规范

```yaml
标题: 书写系统规范
创建时间: 2023年8月26日
```

书写系统规范由词典、语法、正字法、标点符号用法标准以及其他细节组成。

+   简体中文以《[GB/T 15834-2011 标点符号用法标准][]》作为标点符号用法标准。

+   繁体中文以《[重訂標點符號手冊][]》作为标点符号用法标准。

[GB/T 15834-2011 标点符号用法标准]: http://www.moe.gov.cn/ewebeditor/uploadfile/2015/01/13/20150113091548267.pdf
[重訂標點符號手冊]: https://language.moe.gov.tw/001/Upload/FILES/SITE_CONTENT/M1/HAU/haushou.htm

其他地区的书写系统基本没有硬性规定的正字法、标点符号用法标准，所以暂不进行定义。

### 可选模块

+   GWLM 3-0：尊重产品名词等专有名词的书写规范。[^ccg_108]

    [^ccg_108]: sgalal, 《[關於中文與英文、中文與數字間添加間距的疑問 · Issue #108 · sparanoid/chinese-copywriting-guidelines](https://github.com/sparanoid/chinese-copywriting-guidelines/issues/108)》, GitHub, 2020-01-27. (参照 2023-08-27).

    产品名词可以参考官方网站、印刷品或者含有名称的地方，然后检查间距或书写情况，如果官方的使用混乱，
    视作没有规范。

    没有作者定义的专有名词，比如「维生素C」「U盘」「USBフラッシュドライブ」这类翻译而来的专有名词，
    视作没有规范。

+   GWLM 3-1：各书写系统的写作方法在能在片段环境中完整生效，例外：

    +   GWLM 3-1-1：句首大写。

+   GWLM 3-2：片段环境会影响首尾有成对的符号，例外：

    +   GWLM 3-2-1：括号。

    +   GWLM 3-2-2：引号。

    +   GWLM 3-2-4：书名号（包括使用斜体表示书名）。

+   GWLM 3-3：单位符号与数字之间需要增加空格，例外：

    +   GWLM 3-3-1：度数，例如 ° ℃ °C。

    +   GWLM 3-3-2：百分号、千分号和万分号，例如 % ％ ‰ ‱。

+   GWLM 3-4：全角与半角字符之间需要增加空格，例外：

    +   GWLM 3-4-1：全角阿拉伯数字。

    +   GWLM 3-4-2：全角标点符号，例如 ， 。 ； 《 等。

    +   GWLM 3-4-4：全角特殊符号，例如 ％ ＊ ￥ ／ 等。

+   GWLM 3-5：「特殊环境」的特殊处理：

    +   GWLM 3-5-0-1：对时间特殊处理（一）：

        将时间视作整体，不为「YYYY」「年」「MM」「月」「DD」「日」之间添加空格，并在前后添加空格，
        演示如下：[^ccg_102]

        [^ccg_102]: undeadway, 《[是否可以明确一下日期的书写格式 · Issue #102 · sparanoid/chinese-copywriting-guidelines](https://github.com/sparanoid/chinese-copywriting-guidelines/issues/102)》, GitHub, 2019-12-25. (参照 2023-08-27).

        > 有条 issues 在 2019 年 12 月 25 日 23 时 20 分 30 秒发布。

        > 有条 issues 在 2019年12月25日 23时20分30秒 发布。

        规则是「年月日」「时分秒」各为一组，如果缺少一个时间单位，依然特殊处理：

        > 有条 issues 在 12月25日 23时20分 发布。

        如果仅有一个时间单位，那么就不进行特殊处理：

        > 有条 issues 在 25 日 23 时发布。

        > 有条 issues 在 12月25日 23 时发布。

    +   GWLM 3-5-0-2：对时间特殊处理（二）：暂未使用的保留编号。

    +   GWLM 3-5-1-1：对链接特殊处理（一）：

        为链接的前后添加空格：

        > 埃佩克斯是位于 [北卡罗来纳州](#/) [韦克县](#/) 的一个镇，属于 [罗利](#/) [郊区](#/) 的一部份。

+   GWLM 3-6：CJK 标点符号替换：

    +   GWLM 3-6-1：替换「简体中文的弯引号」为「全角直角引号」。

        | 原始  | Unicode  | 修改后 | Unicode  |
        | :---: | :------: | :----: | :------: |
        |   “   | `U+201C` |   「   | `U+300C` |
        |   ”   | `U+201D` |   」   | `U+300D` |
        |   ‘   | `U+2018` |   『   | `U+300E` |
        |   ’   | `U+2019` |   』   | `U+300F` |

    +   GWLM 3-6-2：替换「全角单层直角引号」为「半角单层直角引号」。

        | 原始  | Unicode  | 修改后 | Unicode  |
        | :---: | :------: | :----: | :------: |
        |  「   | `U+300C` |   ｢    | `U+FF62` |
        |  」   | `U+300D` |   ｣    | `U+FF63` |

    +   GWLM 3-6-4：替换「CJK 通用全角括号」为「英文半角括号」。

        | 原始  | Unicode  | 修改后 | Unicode  |
        | :---: | :------: | :----: | :------: |
        |  （   | `U+FF08` |   (    | `U+0028` |
        |  ）   | `U+FF09` |   )    | `U+0029` |

    +   GWLM 3-6-8：替换「中日通用全角逗号」为「英文的半角逗号」。

        | 原始  | Unicode  | 修改后 | Unicode  |
        | :---: | :------: | :----: | :------: |
        |  ，   | `U+FF0C` |   ,    | `U+002C` |

    +   GWLM 3-6-16：替换「CJK 通用全角句号」为「CJK 通用半角句号」。

        | 原始  | Unicode  | 修改后 | Unicode  |
        | :---: | :------: | :----: | :------: |
        |  。   | `U+3002` |   ｡    | `U+FF61` |

    +   GWLM 3-6-32：替换「CJK 通用全角句号」为「英文的半角句号」。

        | 原始  | Unicode  | 修改后 | Unicode  |
        | :---: | :------: | :----: | :------: |
        |  。   | `U+3002` |   .    | `U+002E` |

+   GWLM 3-7：英语标点符号替换：

    +   GWLM 3-7-1：替换「英语的弯引号」为「全角直角引号」。

        | 原始  | Unicode  | 修改后 | Unicode  |
        | :---: | :------: | :----: | :------: |
        |   “   | `U+201C` |   「   | `U+300C` |
        |   ”   | `U+201D` |   」   | `U+300D` |
        |   ‘   | `U+2018` |   『   | `U+300E` |
        |   ’   | `U+2019` |   』   | `U+300F` |

备注：启用 GWLM 3-2 表示同时启用了 GWLM 3, GWLM 3-2；
启用 GWLM 3-4-7，就表示同时启用了 GWLM 3, GWLM 3-4, GWLM 3-4-1, GWLM 3-4-2, GWLM 3-4-4，
原理是部分模块使用 1, 2, 4, 8… 这样的序列递增，其实是二进制的位关系，所以可以相加。

| 十进制 | 二进制 | 含义（启用的模块） |
| ------ | ------ | ------------------ |
| 1      | 1      | 1                  |
| 2      | 10     | 2                  |
| 3      | 11     | 1, 2               |
| 4      | 100    | 4                  |
| 5      | 101    | 1, 4               |
| 6      | 110    | 1, 2               |
| 7      | 111    | 1, 2, 4            |

GWLM 3-6-1 与 GWLM 3-7-1 的结果看起来相同，当其作用的领域不同。GWLM 3-6 作用于 CJK 的标点符号，
即中日韩统一表意文字的标点符号。而 GWLM 3-7 作用于英语的标点符号。

### 示例

下面是启用一些模块后的效果：

| 启用的模块                     | 效果               | 效果                           |
| ------------------------------ | ------------------ | ------------------------------ |
| 原始                           | 用户打开qq音乐     | apple在传记steve jobs          |
| GWLM 3                         | 用户打开qq音乐。   | apple在传记《steve jobs》。    |
| GWLM 3-0                       | 用户打开QQ音乐。   | apple在传记《Steve Jobs》。    |
| GWLM 3-1                       | 用户打开Qq音乐。   | Apple在传记《Steve jobs》。    |
| GWLM 3-2                       | 用户打开qq音乐。   | apple在传记<i>steve jobs</i>。 |
| GWLM 3-4                       | 用户打开 qq 音乐。 | apple 在传记《 steve jobs 》。 |
| GWLM 3-4-3                     | 用户打开 qq 音乐。 | apple 在传记《steve jobs》。   |
| GWLM 3-2, GWLM 3-4-3           | 用户打开 qq 音乐。 | apple 在传记 _steve jobs_。    |
| GWLM 3-0, GWLM 3-2, GWLM 3-4-3 | 用户打开 QQ音乐。  | apple 在传记 _Steve Jobs_。    |

---

如果更改模块的排序，也会导致优先级改变，比如：

| 启用的模块         | 效果               |                              |
| ------------------ | ------------------ | ---------------------------- |
| 原始               | 用户打开qq音乐     | apple在传记steve jobs        |
| GWLM 3             | 用户打开qq音乐。   | apple在传记《steve jobs》。  |
| GWLM 3-0           | 用户打开QQ音乐。   | apple在传记《Steve Jobs》。  |
| GWLM 3-4           | 用户打开 qq 音乐。 | apple 在传记《Steve Jobs》   |
| GWLM 3-0, GWLM 3-4 | 用户打开 QQ音乐。  | apple 在传记《Steve Jobs》。 |
| GWLM 3-4, GWLM 3-0 | 用户打开 QQ 音乐。 | apple 在传记《Steve Jobs》。 |

---

启用 GWLM 3-2 后，如果提到了不同书写系统的作品名，那么需要使用当地书写系统的书名表达方式：

> 我听说过« Beispiel in Frankreich » «Beispiel in der Schweiz» »Beispiel in Deutschland und Österreich«
> 《十万个为什么》『吾輩は猫である』_Steve Jobs_ 这些书名。

分别是法文、瑞士、德国／奥地利、中文、日文和英文的书名号表示方式。[^53627]

[^53627]: 德语世界, 《[【学生园地】德语的引号问题](https://www.sohu.com/a/www.sohu.com/a/289535110_653627)》, 搜狐新闻／搜狐号, 2019-01-16. (参照 2023-08-26).

## GWLM 4 兼容性

```yaml
标题: 兼容性
创建时间: 2023年8月26日
```

### 各种文字的兼容性

各地文字之间存在兼容性，比如 DNA、NBA 和 FPS 这些英文缩写，以及 Apple、Google 和 Microsoft 这些知名公司，
都已经成为了事实上的中文 [外来语][]，属于直接使用的外来词，就像是香港常用的张 Sir 来表示张先生一样，
没有必要使用引号标注。

[外来语]: https://zh.wikipedia.org/wiki/外来语

但是如果是中文、俄文或者日文，出现在英文环境，就需要使用引号包围了。

### 兼容其他规范

简介里有提到因为《律法》是模块化的，所以可以选配各种不同的规范，所以现有的排版规范也可以使用《律法》来实现。

《[中文文案排版指北][]》是相当知名的中文文案、排版方案，可以通过启用部分《律法》模块来兼容《指北》，
具体是 GWLM 3-0, GWLM 3-1, GWLM 3-2-3, GWLM 3-3-3, GWLM 3-4-3, GWLM 3-6-1。

[中文文案排版指北]: https://github.com/sparanoid/chinese-copywriting-guidelines

## GWLM 5 表情

文字表情有多种形式，包括「假借文字表情」、颜文字和 Emoji 等等。

表情特殊的地方在于，可作为句号使用，例如：[^ccg_47]

[^ccg_47]: CatTail, 《[如何处理表情文本 · Issue #47 · sparanoid/chinese-copywriting-guidelines](https://github.com/sparanoid/chinese-copywriting-guidelines/issues/47)》, GitHub, 2016-10-01. (参照 2023-08-27).

> 今天出去 🛒，身上的 💰 竟然掉了，非常的 😫
>
> _(GWLM 3-4, GWLM 5)_

### 假借文字表情

在一些论坛，会在输入文字排版时，使用「233」或者「(bgm38)」这样的纯文本进行调用相应的表情图片，
比如「233」属于猫扑的 233 号表情，在输入时需要输入 233 这样的文字，久而久之 233 就获得了原本表情的含义。

「bgm38」也是相同的情况，这是 Bangumi 的第 38 号表情，可以在发布文字的框体中输入「(bgm38)」来调用相应的表情图片。

因为文字本身没有含义，主要是依靠这段文字能与表情产生关系，所以这里将「233」「bgm38」称作「假借文字表情」。

「假借文字表情」由常见的字符组成，所以受到 GWLM 3-4 控制，演示如下：

| 启用的模块       | 效果                |
| ---------------- | ------------------- |
| GWLM 3           | 这个视频真有趣233。 |
| GWLM 3, GWLM 5   | 这个视频真有趣233   |
| GWLM 3-4, GWLM 5 | 这个视频真有趣 233  |

### 颜文字

颜文字 (Kaomoji) 由许多半角或全角符号组成，所以应该将会分别检查首尾的全角／半角情况，
这受 GWLM 3-4 控制，演示如下：

| 启用的模块 | 效果                       |
| ---------- | -------------------------- |
| GWLM 3     | 颜文字♪（´▽｀）非常精妙。  |
| GWLM 3-4   | 颜文字 ♪（´▽｀）非常精妙。 |

### Emoji

Emoji 被视作半角字符，并且连续使用时，Emoji 之间也需要有空格：

> 🍣 🍤 🍙 🍘 这些料理正好吃！
>
> _(GWLM 3-4, GWLM 5)_

## GWLM 15834 简体中文标点符号用法

《GB/T 15834-2011 标点符号用法标准》这个标准存在一些模糊的情况，所以这里尝试使用更精确的模块替代部分标准。

### GWLM 15834-4-5 顿号

GGWLM 15834-4-5 是替代《GB/T 15834-2011 标点符号用法标准》4.5 小节的模块《律法》，描述了顿号的定义、
形式和基本用法。

+   4.5.1 定义：

    +   句内点号的一种，表示语段中并列词语之间或某些序次语之后的停顿。

+   4.5.2 形式：

    +   顿号的形式是「、」。

        | 符号  | Unicode  |
        | :---: | :------: |
        |  、   | `U+3001` |

+   4.5.3 基本用法：

    +   作为弱于逗号的停顿，示例：

        > 我准备讲两个问题：一、逻辑学是什么？二、怎样学好逻辑学？

        > 甲、题材；乙、用字；丙、表达；丁、色彩。

    +   作为「连词」的替代符号。[^cw]

        > 《Apex 英雄》是一款专注于角色、小队制的大逃杀射击游戏。

        > GDP、人均 GDP 和常住人口这项指标，可以划分出一、二、三线城市。[^ltcic]

        [^ltcic]:  xunyun, 《[Lower-tier_Cities_in_China/data/低线城市划分.md](https://github.com/xunyun/Lower-tier_Cities_in_China/blob/master/data/低线城市划分.md)》, GitHub, 2018-11-20. (参照 2023-08-27).

        如果本来就没有必要使用「连词」，那么也无需使用顿号，比如：

        > 我喜欢《Apex 英雄》《机器人总动员》《我兔斯基你》「东方 Project」这些作品。

        书名号或者引号已将这些内容间隔开了，所以不再需要使用「连词」或者顿号，但是如果这些词语的首尾符号不同，
        那么就需要使用顿号间隔，比如：

        > 我喜欢《Apex 英雄》（游戏）、《机器人总动员》（电影）、《我兔斯基你》（绘本）、「东方 Project」
        （文化）这些作品。

        因为括号属于夹注，能够推理出括号内容是对前文的注释，但是混排在一起就会缺少间隔，
        增加了理解句子的难度，下面是反例：

        > 我喜欢《Apex 英雄》（游戏）《机器人总动员》（电影）《我兔斯基你》（绘本）「东方 Project」（文化）
        这些作品。

[^cw]: 「连词」即连接两个词语的词语，比如「和」「跟」「与」及「或者」。
