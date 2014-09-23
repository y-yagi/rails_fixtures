### Fixturesについて(2)

* テスト環境ではテスト実行前に自動でDBに格納される
  * テスト終了時にrollback. delete+insertにしたい場合は、場合は、 use_transactional_fixturesにfalseを設定
* データアクセス用のメソッドも用意されている
  * use_instantiated_fixtures を設定することで、インスタンスの生成も行われる

```yaml
# web_sites.yml
  rubyonrails:
    id: 1
    name: Ruby on Rails
    url: http://www.rubyonrails.org
```

```ruby
web_sites(:rubyonrails).name # => Ruby on Rails
```

