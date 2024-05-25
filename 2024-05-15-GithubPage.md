Github Page /w Jekyll
===
# everythin


## Jekyll:
This is [an Jekyll tutorial](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/adding-a-theme-to-your-github-pages-site-using-jekyll "DMC") link.

1. 在你的repository找到`_config.yml`檔案，因為我沒有照著github page的建立方式來做，所以我就得自己新建一個，*記得檔名要在最前面加一個底線呦*
2. 在`_config.yml`中可以按你的想法把設定細節寫在裡面，而我們這次則是要幫我們的部落格新增風格套件
3. 在[這篇文章](https://github.blog/changelog/2022-08-22-github-pages-deprecating-the-theme-picker/)可以看到，我們不再能夠直接在github page設定theme picker就好，因此我們得用別的方式添增Jekyll主題
4. 按照官網，先下載前置作業
* Ruby
* RubyGems
* GCC就麻煩了，
https://hackmd.io/@ShawnNTU-CS/HJj4EfGhp?utm_source=preview-mode&utm_medium=rec
https://sites.google.com/site/mycprogrammingbook/bu-chong-cai-liao/gccanzhuang
設定 -> 系統 -> 系統資訊 -> 進階系統設定 -> 進階 -> 環境變數 -> "系統變數"中找Path -> 點選編輯 -> 新增 D:\mingw64\bin -> 一路按確定
`gcc --version`和`g++ --version`檢查
* make呢，怎麼要選擇windows版本的 : Complete package, except sources -> C:\Program Files (x86)\GnuWin32 -> 同上 -> `make --version`


4. 因此，我們要新增一行程式碼 : `theme: jekyll-theme-minimal`來添增主題~~
5. 西卡西，新問題是，markdown的網頁是變好看了，但主業index.html可是完全沒變化阿，這可怎麼辦??



* 補充 : 要怎麼新增圖片阿?
* 補充 : github action





!!!!!!!!!!!!!!
google 表單
1. 本地端新建儲存庫
2. jekyll new .
3. .....

bundle exec jekyll serve的重要性
