### FactoryGirl to Fixtures

* 今あるFactoryを元にFixturesをモクモクと作成
  * 動的生成の部分は極力固定データに
* `FactoryGirl.create`していた処理をアクセス用メソッドに書き換え
* `FactoryGirl.build`ついては普通のインスタンス生成処理に置換
  * 一部アクセス用メソッドでごまかした箇所もある
* テスト用のhelperファイルを整理
