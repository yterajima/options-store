#Options Store

##概要
WordPressのoptionsテーブルにデータを登録し、取り出すことができるだけのPluginです。

##データ登録方法
- 管理画面サイドバーの"Options Store"をクリック
- テキストエリアにデータを入力
- 変更を保存

##データ取得/表示
登録したデータを取り出す為に2つの関数を定義しています。

###get_osdata()
登録したデータを取得します。

###osdata()
登録したデータを表示します。
※esc_html()関数でエスケープ処理されたデータを出力します。


##具体的な例

###サイトのTopに使用するスライダーの画像を管理画面で管理する場合
- テキストエリアにスライダー表示したい画像のURLを入力(改行区切り)
- 出力部分でデータを取得し、配列に加工。
- フォーマットに従って出力処理

###API key管理
- 各種APIのkeyを"key_name:key_value"(改行区切りorカンマ区切り)で入力
- 必要な個所でデータを取得し、配列に加工
- 使いたいように使う
