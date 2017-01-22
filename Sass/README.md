# Sass

## Sass vs Scss

Sass 不用寫大括號，Scss 要。

Scss 比較貼近原生 css 的寫法。

## 安裝

要先安裝 node.js。(也有ruby版，暫且不提。)

以下以 Mac OS X 為操作範例，centOS 或 ubuntu 應該也差不多，只是管理工具 yum、apt-get、brew 差異。

### 安裝 node.js

```bash
brew install node
```

新版的 node.js 會已經包了 npm ，不用再另外安裝。

### 安裝 node-sass

```bash
npm install node-sass -g
```

-g 會將套件安裝在全域的套件資料夾

--save-dev 則是安裝在專案的資料夾裡

### 語法

[SCSS 15分鐘入門](http://eddychang.me/blog/others/91-scss-15-mins.html)

### 整合

```bash
node-sass [scss檔案路徑] [目的css檔案路徑] --output-style compressed
```

--output-style compressed 參數會壓縮產生的 css 檔案。
