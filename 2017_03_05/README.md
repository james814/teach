# 如何使用github架設個人網站 

網頁設計的目的，就是要放在網路上給大家瀏覽，而一般的解決方式 就是將網頁存放在虛擬主機並申請 DNS(網域名稱)，然後透過ftp上傳更新檔案，但這樣的流程，初期可能需要花一點錢，申請虛擬主機的步驟也很繁鎖，而一般在資訊領域，我們會使用一種叫作git版本控管的技術來管理團隊專案的程式碼，但其實版本控管對於管理其他領域的檔案 也是有很大的幫助性，例如你的個人網頁檔案、doc文件、甚至是ps設計檔 等，如果不了解版本控管可以先去google一下版本控管大致的觀念，這部份的網路中文資源也已經相當完備，而本篇最主要就是教導你，如何利用版本控管服務商 github來管理你的個人網站 並利用 github 提供的配套功能 來架設你個人網站。
<br />
如果你熟悉了這一整套流程，架站的費用除了申請個人網域的成本之外 將趨進於0，並且可以有效的控管你網頁檔案，速度也相當穩定的，甚至可以用這個網站去提供額外的個人服務，比如說宣傳資訊、給人下載檔案等等。

## 以下列出本次教學的流程

1、申請一個github帳號<br />
2、重github new一個 Repository儲存庫<br />
3、下載sourcetree<br />
4、將 github 與 sourcetree 做連接 ，配置一個本地 Repository<br />
5、先熟悉在本地端進行版本控管的流程 (branches 支線、commit、還原檔案等等)<br />
6、將更新完的動作 傳到遠方的github Repository上<br />
7、反向思考，如果遠端的github 在其他地方有更改過，你可以用pull把你更改的東西拉回來，了解多人團隊工作的原理<br />
8、了解基本的github 使用方式，你可以將別人的專案clone 回來，別人也可以透過這個方式去clone 你的檔案 ，達到開源與團隊分工的目的。<br />
9、用github 申請個人網頁<br />
	wayne1894.github.io  可以設定全域性的

10、與你的dns做綁定 (他的支線在mester)<br />

10流程<br />
	1、向dns服務商申請一個dns 
	<br />
	2、打開設定dns的管理介面
	<br />
		 將A記錄指向github的ip地址  192.30.252.153  , 192.30.252.154   有兩組ip
		 <br />
		 設定 CNAME 指向 your-username.github.io (還不確定要不要實作)
		  <br />
		 到github 根目錄放一個CANME的檔案 ，其中包含您的域名
		 到github settings Custom domain  設定 你新的網址，Source 選 master
		  <br />
		 還有一個如何增加https
		 https://sheharyar.me/blog/free-ssl-for-github-pages-with-custom-domains/
		 https://blog.ccjeng.com/2016/04/CloudFlare.html
		https://blog.dmoon.tw/github-pages-with-free-ssl/
## 參考資源：

git觀念：http://www.mrmu.com.tw/2011/05/06/git-tutorial-for-beginner/<br />
git觀念：http://www.ithome.com.tw/news/95283<br />
github 建立個人網頁 ：http://ithelp.ithome.com.tw/articles/10171911<br />
