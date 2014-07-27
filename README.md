# ローカルリポジトリを作る作業
mkdir git-remote-test  # 任意のディレクトリ名
touch README.md
git init
git add README.md
git commit -m "first commit"

# GitHub上に同ディレクトリ名のリモートリポジトリを作成
## ！このとき何もチェック付けない

# ローカルリポジトリの内容をリモートリポジトリに登録する作業
## このローカルリポジトリのリモートリポジトリはhogeリポジトリだよってのを登録
git remote add origin git@github.com:kohi3/git-remote-test.git
## リモートリポジトリに現在のブランチのupstreamをmasterに送信
git push -u origin master
