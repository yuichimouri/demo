# Gitbook側からの更新はgithubにどう反映されるのか

## gitbook -&gt; github

draftとして保存されるので、gitbook側のmergeボタンからマージするとgithubもgitbookの公開URLも反映される。  
fileのアップロードによるページの追加も可能。 releaseでversion管理ができる模様。新しくreleaseをつくるとgithubのほうで新規ブランチにcommitされ、ブランチごとにバージョンが管理される。 gitbookでmainに設定したverがgithubでmasterになるようにpull requestをだせる。 ver管理においてはmainの切り替えを繰り返し行うとconflictが起こる。まじでver管理以外には使わない方がいいかも。

編集のためにたくさんボタンがある。CMS的な管理が可。 編集後のアクションとして用意されているボタンは

* activity
* view changes
* archive
* merge

draftを残しておいて、管理者がmergeする体制になるか。

## github -&gt; gitbook

githubのほうでmdファイルを更新するとgitbookにすぐ反映される。

通常の開発のようにブランチを切ればpull requestも可能。管理者がマージするように一元管理するならgitbookの編集は使わない方針のほうがよいかも。

## そもそもsyncしないと

githubのrepositoryと接続していないときには更新するだけですぐ反映される。

