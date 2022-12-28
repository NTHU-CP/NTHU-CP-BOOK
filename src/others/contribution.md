# Contribute to NTHU CP Book

> 非常歡迎大家一同協作此專案！想新增或修改什麼就直接開 Issue 或者是 Pull Request 吧！

NTHU CP Book 是由 mdBook 製作而成，搭配 Github Action，將網站的最新版本部署到 Github Pages。

以下提供一個簡單的步驟給想要編輯此專案，但又不熟悉 Git 以及 GitHub workflow 的人。請先 fork [NTHU-CP-Book](https://github.com/NTHU-CP/NTHU-CP-Book) 這個 repository。

![](image/fork.png)

接著 clone 一份下來到你的本地環境，checkout 到一個新的 branch，名稱可以自訂，通常是與你要做的修改有關。

![](image/clone.png)

```
git clone https://github.com/your_username/NTHU-CP-Book.git
git checkout -b your_branch_name
```

接著即可開始修改他囉！檔案架構與格式可以參考 [mdBook Documentation](https://rust-lang.github.io/mdBook/)。修改途中/完成時，也記得要把他 render 出來確認自己的改動格式沒問題（需要安裝 mdBook）。

```
mdbook serve --open
```

改動完成後，就 commit 並 push 到存 fork 出來存放在 GitHub 上的 repository。請不要將 mdBook render 出來的內容或者是一些非改動相關的檔案加進來。Commit message 請使用英文一句話描述此次的修改，盡量不要超過 50 字，首字母大寫。

```
git add file_you_changed
git commit -m "Commit message"
git push origin your_branch_name
```

push 上去之後應該就能在 NTHU CP Book 的 repository 或者是 fork 出來的 repository 上看到可以 Compare & pull request。大膽地按下去。
![](image/pr.png)

你可以在這邊瀏覽一下自己的 commit 或者是寫一些話給要 review 的人。都沒問題後就可以按下 Create pull request 並等人來 review 囉！

![](image/create_pr.png)

建議需要熟悉 Git 的操作，但也不需要擔心會把整個 repository 搞砸，因為你是在 fork 出來的那份上編輯，也需要通過 review 才能被 merge 進去。

以下附上一些可能有用的參考資料：
- [連猴子都能懂的Git入門指南](https://backlog.com/git-tutorial/tw/)
- [與其它開發者的互動 - 使用 Pull Request（PR）- 為你自己學Git](https://gitbook.tw/chapters/github/pull-request)
