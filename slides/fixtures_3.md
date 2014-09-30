### Fixturesについて(3)

* erb記法が使える

```yaml
# tags.yml
ruby:
  name: ruby
  created_at: <%= 3.days.ago %>

<% 10.times do |i| %>
tag_<%= i %>:
  name: tag<%= i %>
<% end %>
```
こんなんがいける
