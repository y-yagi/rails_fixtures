### fixtureについて(1)

*  Fixtures are a way of organizing data that you want to test against; in short, sample data.
*  YAMLファイル
*  モデル毎に1ファイル
*  格納先は "<your-rails-app>/test/fixtures/" (ActiveSupport::TestCase.fixture_path で変更可能)

```ruby
# web_sites.yml
  rubyonrails:
    id: 1     # ID自動生成してくれるので、書かないでもOK
    name: Ruby on Rails
    url: http://www.rubyonrails.org

  google:
    id: 2
    name: Google
    url: http://www.google.com
```
