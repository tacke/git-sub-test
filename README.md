# test-git-sub-module-tree

git submodule, git subtree のテスト

## コマンドのメモ

```sh
# Add submodule
$ git submodule add git@github.com:tacke/test-git-submodule.git test-git-submodule

# Add subtree
$ git subtree add --prefix=test-git-subtree git@github.com:tacke/test-git-subtree.git master

# Add subtree w/squash
$ git subtree add --prefix=test-git-subtree-squash git@github.com:tacke/test-git-subtree.git master --squash

# Remove submodule
$ git submodule deinit path/to/submodule
$ git rm path/to/submodule

# Remove subtree
# subtreeは普通に削除してコミットすればおｋ。その代わり履歴は残る。履歴を消すならgitの履歴を書き換えましょう。
```
