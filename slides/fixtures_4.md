### Fixturesについて(4)

* 更にfixture用のヘルパーメソッドも定義可能 ※4.1から使用可能

```ruby
 module FixtureFileHelpers
   def file_sha(path)
     Digest::SHA2.hexdigest(File.read(Rails.root.join('test/fixtures', path)))
   end
 end
 ActiveRecord::FixtureSet.context_class.send :include, FixtureFileHelpers

```

```
 photo:
   name: kitten.png
   sha: <%= file_sha 'files/kitten.png' %>
```
