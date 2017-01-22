# webpack

以整合 ReactJS script 為例

## 安裝

要先安裝 node.js。

以下以 Mac OS X 為操作範例，centOS 或 ubuntu 應該也差不多，只是管理工具 yum、apt-get、brew 差異。

### 安裝 node.js

```bash
brew install node
```

新版的 node.js 會已經包了 npm ，不用再另外安裝。

### 建立 package.json

在專案目錄下建立 package.json (如果沒有的話)

可以用 npm 指令建立

```bash
npm init
```

會問一連串問題，全部用預設值即可

### 安裝所需套件

```bash
npm install babel-loader babel-core babel-preset-latest babel-preset-react react react-dom webpack --save-dev
```

babel、babel-core 都是 babel 的必要套件

babel-preset-es2015 如果不壓縮 js 檔案可以不用裝

如果有用到es2016、es2017的新功能，那改安裝 babel-preset-latest，latest包含es2015、es2016、es2017

babel-preset-react、react、react-dom(如果是用react dom去render dom就要裝)

這些套件不能安裝在全域，都必須安裝在本地的專案資料夾裡，會自動產生 node_modules

## 編譯

```bash
webpack -p
```

-p 會壓縮產生的 js 檔案




