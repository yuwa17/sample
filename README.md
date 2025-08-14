初期設定
・ローカルリポジトリの作成
mkdir github
cd github
mkdir [ローカルリポジトリの名前]
cd [ローカルリポジトリの名前] // ↑リポジトリの作成
git init // 作成したリポジトリをローカルリポジトリにする


基本的な使い方
・ローカルリポジトリにコミット
git add [ファイル名.拡張子] // 中期保存場所(インデックス)に追加
git commit -m "[Add] [ファイル名]" // インデックスに追加したファイルをコミット

・リモートリポジトリにプッシュ(ローカルリポジトリ配下で行う)
git remote add origin https://github.com/[ユーザ名]/[リモートリポジトリ名].git // ローカルリポジトリとリモートリポジトリを紐づける
git push origin master // 紐づけ完了後、プッシュを実行

・ブランチを作成(ブランチを切る)
git branch [ブランチ名] // ブランチを作成
git checkout [ブランチ名] // ブランチを移動

・ブランチにプッシュ(事前にプッシュしたいブランチに移動)
git add [ファイル名.拡張子]
git commit -m "[Add] [ファイル名]"
git push origin [ブランチ名]

・ブランチのマージを行う(事前にmasterのブランチへ移動)
git merge [マージするブランチ名]
git push origin master // GitHubにプッシュ



確認コマンド
git log // コミットメッセージを含む変更履歴が見れる
git branch // ブランチ一覧や、作業中のブランチを確認できる
