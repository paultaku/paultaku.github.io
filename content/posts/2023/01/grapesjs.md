---
title: "Grapesjs - 開源而且可以擴充的 Web Page Builder "
date: 2023-01-27T18:09:43+08:00
draft: false
---

## 介紹
Web Page Builder 在網頁前端世界裡是一個很多人在做開發的題目。
而且甚至有許多商業用的 Wordpress 主題或是外掛作為相關的營業項目。像是 [Avada](https://themeforest.net/item/avada-responsive-multipurpose-theme/2833226) 或是 [Wix.com](https://www.wix.com/)，都是相當知名的 Page Builder。

GrapeJS 是一個開源的 Web Page Builder，透過這次的研究。希望可以激發大家對於網頁前端及開發有更多的想像。

以下簡介主要編輯部分的功能:

|  種類 | |
|  ----  | ----  |
| 區塊管理 | blockManager   |
| 樣式管理 | styleManager or selectorManager|
| 特徵管理 | traitManager   |
| 裝置管理 | deviceManager  |
| 圖層管理 | layerManager   |
| 儲存管理 | storageManager |

## 區塊管理

主要是可以透過拖拉區塊的方式拉進去編輯器裡面，然後就可以產生出相對應的 html 程式碼。拖拉進去 GrapeJS 的編輯器之後，就會形成一個元件。GrapeJS 還有提供可以客製化區塊管理員的功能。

## 樣式管理

在點選每一個圖層之後，他就可以顯示每個圖層當前的 class 或是 style。就可以在控制面板新增或是修改該個元件或是圖層的樣式。

## 特徵管理

可以在每一個頁面上透過新增屬性(Attributes)增加HTML DOM 的活用度。其中的特徵值也可以顯示在輸出頁面的資料上。

## 裝置管理

可以自行設定該網站想要支援的寬度，可以直接在瀏覽器上查看不同寬度下畫面的呈現。

## 圖層管理

可以透過拖拉的方式去排序和重新架構開發者所希望的畫面上的呈現。

## 儲存管理

主要用途是用來儲存頁面上的操作記錄，可以透過取消上一步的方式(Ctrl+Z)，回覆到想要的狀態。


## 延伸思考
1. 如何整合 grapeJS 和現有的 css 框架?
其實在像是 bootstrap 或是 tailwind css 都是現代前端工程師習慣的 css 框架。如果能好好整合，對前端開發人員是很有幫助的，他可以透過新增 class 就可以修改樣式，也不用特地學習 css 語法。
2. 如何整合網頁開發流程?
在原本設計師交付設計稿給前端工程師之後，是全部由工程師刻畫 html 和 css 去做畫面上的呈現。但是透過 grapeJS 和 figam 的整合，是不是有機會可將設計稿轉換成 html code 的流程簡化，是很值得思考的。透過網頁前端架構的設計，可以讓相關的前端產品的彈性更好，也能夠更好地重複使用。


## 測試網站
[GrapeJS Demo](https://grapesjs.com/demo.html)


## 參考文章
- [GrapeJS Doc](https://grapesjs.com/docs/getting-started.html)

