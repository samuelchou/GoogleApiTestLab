# Hello!

這是一個用來測試 Google Api / Firebase Cloud Functions 的專案。
與此同時，下方會記錄我個人的安裝設定過程。

# 如何安裝與啟動 Firebase 於此專案

大前提：你要有一個 Firebase 專案（廢話XD）

- 為了使用 Cloud Functions, 請為專案開啟 Blaze 以上付費方案。

接下來開始設定環境。

首先，安裝 node.js + npm. (推薦使用 nvm)

再來，安裝 Firebase tools:

```
npm install -g firebase-tools
```

然後到專案資料夾下方，進行 Firebase 登入綁定：

```
firebase login
```

好啦！你可以開始用了。

## 安裝 Cloud Functions

要完成 Cloud Functions 設置，請執行以下指令：

```
firebase init functions
```

然後照著互動完成專案設置。
（該專案已經完成設置，請勿重複執行）


## 我還想使用 Firestore

一些場合會需要使用 Firestore.
如果要使用 Firestore, 請執行以下指令：

```
firebase init firestore
```

然後照著互動完成專案設置。
（該專案已經完成設置，請勿重複執行）

# 執行虛擬機

請執行以下指令：

```
firebase emulators:start
```

你可能會需要將本地 Java 更新到 8 以上的版本。

好啦，現在 Emulators 會告訴你這些 Functions (API) 的位址。