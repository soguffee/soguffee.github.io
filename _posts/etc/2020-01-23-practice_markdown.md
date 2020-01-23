---
title:  "マークダウン記法"
excerpt: "Github Blog"

categories:
  - etc
tags:
  - Study
  - Markdown
last_modified_at: 2020-01-23T12:00:00-00:00
---

# 1. マークダウンに関して
## 1.1.　マークダウンとは？
[**Markdown**](http://whatismarkdown.com/)はテキスト基盤のマークアップ言語で、2004年ジュン・グルーバーに作られて、より読み書きやすいしHTMLへの返還もできる。


## 2.1. ヘッダー
* 大タイトル
  ```
  This is an H1
  =============
  ```
  This is an H1  
  =============

* 小タイトル：副タイトル
  ```
  This is an H2
  -------------
  ```
  This is an H2  
  -------------

* 文頭:1~6まで
```
# This is a H1
## This is a H2
### This is a H3
#### This is a H4
##### This is a H5
###### This is a H6
```
# This is a H1
## This is a H2
### This is a H3
#### This is a H4
##### This is a H5
###### This is a H6

## 2.2 BlockQuote

```
> This is a first blockquote
>   > This is a second blockquote
>   >   > This is a third blockquote
```
> This is a first blockquote
>   > This is a second blockquote
>   >   > This is a third blockquote

この中では他のマークダウン要素が含まれる。
> ### This is a H3
> * List
>   ```
>   code
>   ```

## 2.3. リスト
### ● 順番のあるリスト

```
1. 一番目
2. 二番目
3. 三番目
```
1. 一番目
2. 二番目
3. 三番目

**番号を並べ替えてもに入力しても降順される。**

```
1. 一番目
3. 三番目
2. 二番目
```
1. 一番目
3. 三番目
2. 二番目

### ● 順番のないリスト
```
* あか
  * みどり
    * あお

+ あか
  + みどり
    + あお

- あか
  - みどり
    - あお
```
* あか  
  * みどり  
    * あお  

+ あか  
  + みどり  
    + あお  

- あか  
  - みどり  
    - あお    

混ぜて使用することもできる。

```
* 1段階
  - 2段階
    + 3段階
      + 4段階
```

* 1段階
  - 2段階
    + 3段階
      + 4段階

## 2.4. コード

### 2.4.1. インデント
```
This is a normal paragraph:
    
    This is a code block.

end code block
```  

例：

*****
This is a normal paragraph:
    
    This is a code block.

end code block
*****

<br/>

> 一間飛ばないと認識しない問題が発生

```
This is a normal paragraph:
    This is a code block.
end code block.
```

例：

*****
This is a normal paragraph:    
    This is a code block.
end code block
*****

### 2.4.1. コードブロック
コードブロックは次の2つ方法を作用できます。

* `<pre><code>{code}</code></pre>`

```
<pre>
<code>
public class Hello {
  public static void main(String[] args) {
    System.out.println("Hello, World");
  }
}
</code>
</pre>
```

<pre>
<code>
public class Hello {
  public static void main(String[] args) {
    System.out.println("Hello, World");
  }
}
</code>
</pre>

* \`\`\`を利用する方法
<pre>
<code>
```
public class Hello {
  public static void main(String[] args) {
    System.out.println("Hello, World");
  }
}
```
</code>
</pre>

```
public class Hello {
  public static void main(String[] args) {
    System.out.println("Hello, World");
  }
}
```

