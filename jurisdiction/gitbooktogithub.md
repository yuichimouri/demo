# Gitbook側からの更新はgithubにどう反映されるのか

### gitbook -&gt; github

draftとして保存されるので、gitbook側のmergeボタンからマージするとgithubもgitbookの公開URLも反映される。  
fileのアップロードも可能。

用意されているボタンは

* activity
* view changes
* archive
* merge

draftを残しておいて、管理者がmergeする体制になるか。

### github -&gt; gitbook

githubのほうでmdファイルを更新するとgitbookにすぐ反映される。

通常の開発のようにブランチを切ればpull requestも可能。管理者がマージするように一元管理するならgitbookの編集は使わない方針のほうがよいかも。

### そもそもsyncしないと

githubのrepositoryと接続していないときには更新するだけですぐ反映される。

