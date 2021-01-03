## sampleダウンロード
https://www.facebook.com/wordpress5book

見本サイト
https://wpbook-pacificmall.work/

# 20201023
p57
ディレクトリ構造が書いてあって参考になりそう。
p58
1つのページを分割する方法が書いてある。テンプレートファイルという。
p61
`<?php get_header(); ?>`で`header.php`が読み込めるらしい。
p66
`get_header()`は、`header.php`を読み込む。
`get_footer()`は、`footer.php`を読み込む。
`get_header('example')`は、`header-example.php`を読み込む。
また、
`get_template_part('header')`は、`get_header()`と同義であり、`header.php`を読み込む。
`get_template_part('footer-top')`は、`get_footer('top')`と同義であり、`footer-top.php`を読み込む。
p66
パーツテンプレートとは、他のテンプレートから呼び出されるテンプレート(例:`header.php`)
メインテーマテンプレートとは、WordPressから直接呼び出されるテンプレート(例:`index.php`)
ページ種類別テンプレートとは、上記2つ以外のテンプレート
p113参照せよ
p67
`wp_get_document_title()`は、サイトの名称に置換
`bloginfo('name')`は、WordPress管理画面の"設定>一般"で設定されたサイトタイトルを表示する。
`bloginfo('description')`は、キャッチフレーズを表示するテンプレートタグ

`wp_head()`と`wp_foot()`は、テーマ作成時に必ず必要なテンプレートタグ。
メタタグの出力、JavaScriptのライブラリ読み込み、WordPressのツールバー、WordPressがHTMLを出力するために必要。

## 参考文献
【基礎知識】ブロックレベル要素・インライン要素の性質と違い | Webmedia
https://www.itra.co.jp/webmedia/block-inline-difference.html

CSSに変数が使えるようになったらしい?
# 20201020
サイトのURLを決めないとな。

パーマリンク設定とは?

p48
`get_template_directory_uri()`メソッドは、現在有効化されているテーマディレクトリのpathを返す。ただし子テーマの場合は親テーマのpathを返す。

index.phpの中身が実質htmlで、`<?php なんとかかんとか ?>`って書くっぽい。
WordPressで利用可能なテーマを作成するのに最低限必要なのは、`index.php`と`style.css`
`index.php`は、空でも良い。

【キャメルケース】camelCase
単語の先頭を大文字にする命名規則です。全ての単語の先頭を大文字にするのがアッパーキャメルケースもしくはパスカルケースで、先頭の単語だけ小文字にするのがローワーキャメルケースと呼ばれます。PHPやjsなどの関数で使われることが多いようです。
【スネークケース】snake_case
単語の間をアンダーバーでつなぐ命名規則です。DBなどで扱われる値に使用されることが多いようです。
【ケバブケース】kebab-case
単語の間をハイフンでつなぐ命名規則です。HTMLではclass名であったり、ファイル名などでもよく見かけます。

キャメルケース → プログラミングでの関数や変数
スネークケース → DBなどで扱う値
ケバブケース → HTMLのclass名
