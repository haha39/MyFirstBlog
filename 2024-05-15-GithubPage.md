---
layout: default
title: "A simple blog built with Github Page and Jekyll"
date: 2024-05-24 17:35:06 +0800
categories: [jekyll update]
---

# Github Page /w Jekyll

# everythin

## Jekyll:

This is [an Jekyll tutorial](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/adding-a-theme-to-your-github-pages-site-using-jekyll "DMC") link.

1. 在[這篇文章](https://github.blog/changelog/2022-08-22-github-pages-deprecating-the-theme-picker/)可以看到，我們不再能夠直接在 github page 設定 theme picker 就好，因此我們得用別的方式添增 Jekyll 主題
2. 按照官網，先下載前置作業
   1. Ruby
   2. RubyGems
   3. GCC 就麻煩了，
      - 來看看這些[參考網址 1](https://hackmd.io/@ShawnNTU-CS/HJj4EfGhp?utm_source=preview-mode&utm_medium=rec)吧
      - 來看看這些[參考網址 2](https://sites.google.com/site/mycprogrammingbook/bu-chong-cai-liao/gccanzhuang)吧
      - 設定 -> 系統 -> 系統資訊 -> 進階系統設定 -> 進階 -> 環境變數 -> "系統變數"中找 Path -> 點選編輯 -> 新增 D:\mingw64\bin -> 一路按確定
      - 最後，使用`gcc --version`和`g++ --version`檢查是否安裝完成
   4. make 呢，怎麼要選擇 windows 版本的 : Complete package, except sources -> C:\Program Files (x86)\GnuWin32 -> 同上 -> `make --version`
3. 用 Github Desktop 新建 repository
4. 在 repository 中， 呼叫你的終端機，輸入`jekyll new .`，把檔案全改成`.md`就對了
5. 讓我們來直接看 Jekyll 的官方教學網站吧 :

   - `bundle exec jekyll serve的重要性!!!!`，人家是即時變動的喔，當然，變更完要 reload 你的網頁
   - 在 `\_config.yml` 中，將 baseurl 和 url 改成我們的 Github 網址
   - Liquid 是蝦米
   - front matter 的重要性
   - Creating a layout，來，見鬼了，沒有 font matter 而且那個 `content` 又是啥阿，那是一個模板，建立完後，其他網站只要輸入 `layout: default`，就可以套用 default 的布局，有點像 LAB 的感覺
   - there’s no way to navigate between pages. Let’s fix that. => THE MIGHTY Includes -> 要開始建立網頁(page)與網頁之間的導向(導航)了，這邊要特別記住的點是，因為我們有多`/MyFirstBlog/`這個子連結，所以在`_includes/navigation.html`中建立連結的時候要多加注意，才不會導覽錯方向開錯路，點開來只會有 404 等著你。
   - 但如果你的文章逐漸多了起來，你開始想要一個迴圈來幫忙了 -> Data files are a great way to separate content from source code to make the site easier to maintain. -> available to you at site.data.navigation ->
   - 是說，導航的時候，markdown 檔案不需要`.md`喔，貼完相對路徑記得把`.md`刪除掉
   - 來吧，我們心心念念的嵌入圖片，總算來到我們的 assets 章節 -> Sass 來也 -> 挖哩，遇到問題了，`styles.scss`總是會坍縮到一行，目前下載*Prettier - Code formatter*讓他不被格式化，可惜了，先跳掉吧。
   * 再來，總算來到了我們的部落格主題!!

   - 來看看這些[參考網址 3](https://gist.github.com/abearxiong/8ae3caa6728e26565fec4a146344a065)吧
   - 來看看這些[參考網址 4](https://jekyllrb.com/docs/step-by-step/01-setup/)吧

- 補充 : 遇到的問題
- 補充 : github action
