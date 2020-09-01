# 更新方法
1. 他人の変更を反映する
	- `git pull`で他人の変更を反映する

1. issueを立てる
	- ブラウザでgitのページへ飛び，リポジトリのissueから`New Issue`をクリックする．
	- その後，issueのタイトルと説明文を追加．

1. ブランチを切る
	- 「index.htmlを加える」のなら，"feature/add-index"みたいな感じ

1. issueに合わせて作業する
	- 普通に作業する

1. 変更部分の確認をする
	- `git status`や`git diff`で確認(目視)

1. 変更箇所をコミットしてプッシュする
	- `git add ファイル名` `git commit -m "きちっと書く"` `git push origin ブランチ名` でOK

1. pull requestする
	- ブラウザでgitのページへ飛び，リポジトリのcodeから黄色いバーの`Compare & pull request`をクリック
	- タイトルはわかりやすく 説明文はissueから#1とか#2とか該当するものを見つけて記載する
	- 例えば該当するissueの下に`#5 opened 12 minutes ago by Gitefu`みたいな感じで書かれていたら，説明文には`#5`と記載する

1. pull requestを許可して，masterブランチにmergeする
	- `Merge pull request`をクリック

1. 立てたissueをクローズする
	- issueから`Close issue`をクリックする

1. コマンドで作成したbranchを消す
	- 変更を反映するために， `git branch master`でmasterに戻り， `git pull`で変更を反映する．
	- `git branch -d ブランチ名`でブランチを削除する

1. ブラウザでgitのページへ飛び，不要なブランチを削除
	-他の人のかもしれないので，自身が削除したブランチだけ削除
