#如何協同開發(單純版)
以這份Repo為例，URL為 `https://github.com/d-d-x/d-d-x.github.io.git`
##複製Repo下來開發
1. Fork這個Repo到自己的帳號，右上角有按鈕
2. 到「自己」的Github頁面點開剛剛Forked的Repo
3. Clone到電腦裡：又右下角有Clone的URL，複製下來
4. 執行`git clone https://github.com/YOUR_USER_NAME/d-d-x.github.io.git`

##設定遠端同步點
1. 切到電腦裡剛剛Clone的專案目錄
2. 設定遠端同步點：執行`git remote add upstream https://github.com/d-d-x/d-d-x.github.io.git`

##把遠端Repo的最新狀態同步到本機端的Repo
1. `git fetch upstream`
2. `git checkout master`
3. `git merge upstream/master`

##在本機修改後，提交合併要求(Pull Request)
1. `git add .`
2. `git commit -m "my commit"`
3. `git push origin master`
4. 到自己的Repo頁面，選擇Create Pull Request
5. 大概就這樣