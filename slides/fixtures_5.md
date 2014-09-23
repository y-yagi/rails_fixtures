### Fixturesについて(5)

* アソシエーションはラベル名で定義出来る

```yaml
# authros.yml
hyuki:
  name: 結城浩
matz:
  name: まつもとゆきひろ
```

```yaml
# tags.yml
programming:
  name: プログラミング
ruby:
  name: ruby
```

```yaml
コードの未来:
  name: コードの未来
  published_at: 2012-05-12
  author: matz
  tags: programming, ruby

秘密の国のアリス:
  name: 秘密の国のアリス
  published_at: 2003-09-30
  author: hyuki
```
