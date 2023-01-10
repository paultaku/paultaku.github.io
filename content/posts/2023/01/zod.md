---
title: "Zod - 透過定義 Schema 以驗證資料的套件，可以彌補 TypeScript 的弱點"
date: 2023-01-09T17:58:09+08:00
draft: false
---

### 介紹

Typescript 轉譯成 Javascript 之後，執行程式碼就無法驗證資料的型態是否是正確的。在三大框架裡面有許多好用的驗證套件。但是 Zod 是一個可以透過宣告 Schema 去驗證資料的 Typescript 的函式庫。透過宣告的方式，補足了執行從 Typescript 轉譯之後的程式卻無法驗證資料型別的不足。

### 使用情境

1. 從 API 取得資料之後
2. 要驗證表單輸入資料是否正確時

我用電商網站的商品作為例子:

假設這是電商網站上產品的物件型別

![product_interface_image](/images/zod/product_interface.png)

### 宣告型別

透過定義各個欄位型別，會有一個最後的 schema object。可以透過 schema object 做資料格式的判斷。

![product_schema_image](/images/zod/product_schema.png)

如果資料錯誤就會丟出 ZodError，ZodError 的格式如下圖:

![zod_error](/images/zod/type_error.png)

也可以客製化錯誤訊息

![zod_custom_error](/images/zod/custom_error.png)

### 結論

1. Zod 可以彌補 Typescript 的不足。原生瀏覽器目前是沒有辦法直接執行 Typescript 的，會需要透過 Webpack 等之類的打包工具去轉譯成原生瀏覽器可以支援的格式。所以 Typescript 目前可以做到的型別檢查還是在還沒轉譯之前，透過檢查的方式判斷變數的資料型別對不對。
2. Zod 做好資料格式方面的驗證，而且支援客製化錯誤訊息。不過在表單的資料驗證，還會有需要做跨表單的驗證或是資料邏輯方面的驗證。這是使用 Zod 需要特別注意的地方。

#### 參考資料

1. [Github Source](https://github.com/colinhacks/zod)
2. [Typescript: 他實際上沒有驗證你的型別](https://vocus.cc/article/62fa1e9dfd89780001139aef)
